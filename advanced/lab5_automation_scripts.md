---
layout: default
title: Lab 5 - Automation Scripts
---

# 🔹 Lab 5: Automate Getting Devices by Network

## 🎯 Objective:
Create a script that lists all devices in every network across an organization.

---

## 🧭 Step-by-Step Instructions:

```python
import meraki

API_KEY = 'your_api_key_here'
ORG_ID = 'your_org_id'

dashboard = meraki.DashboardAPI(api_key=API_KEY)

networks = dashboard.organizations.getOrganizationNetworks(ORG_ID)

for network in networks:
    devices = dashboard.networks.getNetworkDevices(network['id'])
    print(f"Network: {network['name']} - {len(devices)} devices")
```

---

## 🧠 Tip:
Use this pattern for backup, exports, and config inventory.

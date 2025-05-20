---
layout: default
title: Lab 6 - Error Handling
---

# 🔹 Lab 6: Add Logging and Error Handling

## 🎯 Objective:
Ensure your automation can handle failures gracefully.

---

## 🧭 Step-by-Step Instructions:

```python
import meraki
import logging

logging.basicConfig(filename='meraki.log', level=logging.INFO)

dashboard = meraki.DashboardAPI(api_key='your_api_key_here')

try:
    devices = dashboard.networks.getNetworkDevices("invalid_network_id")
except meraki.APIError as e:
    logging.error(f"API call failed: {e}")
    print("Something went wrong. Check logs.")
```

---

## 🧠 Tip:
Always log Meraki responses for audit and debugging.

---
layout: default
title: Lab 4 - Intro to Meraki Python SDK
---

# 🔹 Lab 4: Intro to Cisco Meraki Python SDK

## 🎯 Objective:
Get comfortable using Cisco’s official Meraki SDK, which simplifies endpoint usage and adds error handling.

---

## 🧭 Step-by-Step Instructions:

### 🛠 Step 1: Install the SDK

```bash
pip install meraki
```

---

### 📄 Step 2: Basic Script

```python
import meraki

dashboard = meraki.DashboardAPI(api_key='your_api_key_here')

orgs = dashboard.organizations.getOrganizations()

for org in orgs:
    print(f"{org['name']} - ID: {org['id']}")
```

---

### 🧠 Tip:
The SDK has built-in retry logic, rate limit handling, and documentation inline:
```bash
help(dashboard.organizations.getOrganizations)
```

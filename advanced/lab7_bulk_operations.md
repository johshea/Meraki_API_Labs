---
layout: default
title: Lab 7 - Bulk Configuration
---

# 🔹 Lab 7: Bulk Update Switch Ports

## 🎯 Objective:
Apply settings across multiple switches automatically.

---

## 🧭 Example:

```python
switch_serials = ['Q2XX-1111-2222', 'Q2XX-3333-4444']

for serial in switch_serials:
    dashboard.switch.updateDeviceSwitchPort(
        serial=serial,
        portId=1,
        enabled=True,
        name="Uplink Port",
        type="trunk",
        vlan=10
    )
```

---

## 🧠 Tip:
Use a CSV or JSON input file to scale.

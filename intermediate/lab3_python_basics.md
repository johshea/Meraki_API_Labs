---
layout: default
title: Lab 3 - Python Basics for Meraki API
---

# 🔹 Lab 3: Python Basics

```python
import requests

API_KEY = 'your_api_key'
headers = {"X-Cisco-Meraki-API-Key": API_KEY}
url = 'https://api.meraki.com/api/v1/organizations'

response = requests.get(url, headers=headers)
print(response.json())
```

---
layout: default
title: Lab 3 - Python Basics for Meraki API
---

# 🔹 Lab 3: Making Meraki API Calls with Python (Using `requests`)

## 🎯 Objective:
Learn how to use the Python `requests` library to send a basic GET request to the Meraki API, parse JSON responses, and prepare for more advanced automation.

---

## 🧰 Prerequisites:
- Python 3.8 or later installed
- A Meraki API key
- A code editor (e.g., VS Code, PyCharm)

---

## 🧭 Step-by-Step Instructions:

### 🐍 Step 1: Install Requests

```bash
pip install requests
```

---

### 📄 Step 2: Write Your First Script

Create a file called `get_organizations.py` and paste the following:

```python
import requests

API_KEY = 'your_api_key_here'
url = 'https://api.meraki.com/api/v1/organizations'

headers = {
    "X-Cisco-Meraki-API-Key": API_KEY
}

response = requests.get(url, headers=headers)
data = response.json()

print("Organizations:")
for org in data:
    print(f"- {org['name']} (ID: {org['id']})")
```

---

### 🧪 Step 3: Run the Script

```bash
python get_organizations.py
```

You should see a list of organizations returned by the API.

---

### 🧠 Tips:
- Use `json.dumps(data, indent=2)` for pretty output.
- Catch `requests.exceptions.RequestException` for robust handling.

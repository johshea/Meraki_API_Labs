---
layout: default
title: Lab 8 - Webhook Receiver
---

# 🔹 Lab 8: Receive Meraki Alerts via Webhooks

## 🎯 Objective:
Set up a lightweight server to receive real-time Meraki alerts.

---

## 🧭 Step-by-Step Instructions:

### 🔧 Flask Setup:

```bash
pip install flask
```

---

### 📝 Python Server:

```python
from flask import Flask, request

app = Flask(__name__)

@app.route('/webhook', methods=['POST'])
def webhook():
    alert = request.json
    print("Received webhook:")
    print(alert)
    return '', 200

if __name__ == '__main__':
    app.run(port=5001)
```

---

## 🧠 Tip:
Use Ngrok or similar to expose Flask on public URL for testing.

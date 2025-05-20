---
layout: default
title: Lab 2 - API Key Authentication
---

# 🔹 Lab 2: API Key Authentication and Exploring Endpoints

## 🎯 Objective:
Learn how to generate your Meraki API key and securely use it to access various API endpoints. You’ll also explore the Meraki API documentation and understand how endpoints are structured.

---

## 🧰 Prerequisites:
- A Cisco Meraki account with dashboard access
- Admin privileges to generate an API key

---

## 🧭 Step-by-Step Instructions:

### 🔐 Step 1: Enable API Access

1. Log into your Meraki Dashboard: [https://dashboard.meraki.com](https://dashboard.meraki.com)
2. Click on your avatar (top right corner) > **My Profile**
3. Scroll down to **API access**
4. Check the box: **Enable access to the Cisco Meraki Dashboard API**
5. Save changes

---

### 🔑 Step 2: Generate Your API Key

1. Still under **My Profile**, click **Generate new API key**
2. Copy and store this key securely — it will not be shown again!

---

### ⚠️ Security Tip:
- Never share your API key publicly.
- Treat your key like a password.
- Revoke and regenerate it if compromised.

---

### 🔎 Step 3: Review Meraki API Documentation

1. Visit the Meraki API reference: [https://developer.cisco.com/meraki/api-v1/](https://developer.cisco.com/meraki/api-v1/)
2. Notice the base URL: `https://api.meraki.com/api/v1/`
3. Explore endpoints such as:
   - `GET /organizations`
   - `GET /organizations/{orgId}/networks`
   - `GET /networks/{networkId}/devices`

You’ll use these in the next labs.

---

## 🧠 Tips:
- Use Postman’s **Environment Variables** to manage your API key for reuse.
- Use **Collection Variables** to share the API key across multiple requests.


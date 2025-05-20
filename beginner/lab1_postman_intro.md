---
layout: default
title: Lab 1 - Intro to Meraki API Using Postman
---

# 🔹 Lab 1: Intro to Meraki API Using Postman

## 🎯 Objective:
In this lab, you will install Postman, set up your first request to the Meraki API, and retrieve a list of organizations that your API key has access to. This is your first step into interacting with the Meraki cloud programmatically.

---

## 🧰 Prerequisites:
- A valid Cisco Meraki Dashboard account
- API access enabled on your account
- A generated Meraki API key from your profile
- Postman installed on your system (download from [https://www.postman.com/downloads/](https://www.postman.com/downloads/))

---

## 🧭 Step-by-Step Instructions:

### 🪟 Step 1: Launch Postman

Once installed, open the Postman application. You will see a workspace with tabs across the top, a sidebar on the left with "Collections" and "History", and a large request builder area.

---

### ➕ Step 2: Create a New Request

1. Click on the **+** button at the top to open a new request tab.
2. In the request builder URL field, enter:
   ```
   https://api.meraki.com/api/v1/organizations
   ```
3. To the left of the URL, click the dropdown and select **GET** (this is the default HTTP method used to retrieve information).

---

### 🧾 Step 3: Add the API Key to the Request

1. Click on the **Headers** tab below the URL bar.
2. In the first row of the key-value table, enter the following:
   - **Key**: `X-Cisco-Meraki-API-Key`
   - **Value**: Paste your API key (e.g., `1234abcd5678efgh`)
3. Make sure the checkbox on the left of the row is checked/enabled.

This header authenticates your request to the Meraki API.

---

### 📤 Step 4: Send the Request

1. Click the **Send** button (blue) on the right of the request builder.
2. You should receive a response in JSON format in the response pane below the request builder.
3. If successful, you will see an array of Meraki organizations your key has access to.

**Example Response:**
```json
[
  {
    "id": "123456",
    "name": "My Company Network",
    "url": "https://n123.meraki.com/o/ABC/dashboard"
  }
]
```

---

### 💾 Step 5: Save the Request (Recommended)

1. Click the **Save** button (floppy disk icon).
2. Create a new Collection called `Meraki API Labs`.
3. Save the current request as `Get Organizations`.

This helps you reuse requests in future labs.

---

## 🧠 Tips:

- If you see a `403 Forbidden` error, ensure API access is enabled in your Meraki dashboard and that your API key is correct.
- Use the **Pretty** tab in the response pane to make the JSON easier to read.
- Postman will remember your previous requests in the "History" tab on the left.

---


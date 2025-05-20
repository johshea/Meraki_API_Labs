---
layout: default
title: Lab 9 - Postman Runner Chaining Requests
---

# 🔹 Lab 9: Chaining API Requests with Postman Collection Runner

## 🎯 Objective:
Use Postman to automate a chain of API requests. Extract the `org_id` from one request and reuse it in the next.

---

## 🧭 Steps:

1. **Request 1**: `GET /organizations`
   - In Tests tab:
   ```javascript
   let jsonData = pm.response.json();
   pm.collectionVariables.set("org_id", jsonData[0].id);
   ```

2. **Request 2**: `GET /organizations/{{org_id}}/networks`
   - Uses the variable set by the first request.

3. **Run It**:
   - Click Collection Runner
   - Confirm order and variables
   - Click Run

---

## 🧠 Tip:
Use this pattern for dynamic data extraction and chaining.

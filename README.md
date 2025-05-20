---
layout: default
title: Meraki API Lab Guide
---

# 🧪 Meraki API Lab Guide

Welcome to the Cisco Meraki API Lab Guide — a complete, hands-on learning experience that takes you from the basics of API interaction using Postman to advanced automation with Python and the Meraki SDK. This guide is designed for IT professionals, network engineers, and developers who want to leverage the power of Meraki APIs for operational efficiency and integration.

---

## 🔍 What You Will Learn

- 📘 How to authenticate and make REST API calls using Postman
- 🧪 How to use Cisco’s official Python SDK to interact with Meraki infrastructure
- ⚙️ How to automate routine tasks like device discovery, configuration, and alerting
- 📦 How to chain API calls and use Postman’s collection runner for data-driven execution
- 🛠 Best practices for error handling, logging, and scalable scripting

---

## 🗂 Lab Structure

The labs are grouped into three progressive levels:

### 🟢 Beginner

| Lab | Title                       | Description |
|-----|-----------------------------|-------------|
| 1   | [Intro to Postman](beginner/lab1_postman_intro.md)       | Learn how to make your first API call using Postman |
| 2   | [API Key Authentication](beginner/lab2_api_key_auth.md) | Understand where to generate and use your API key in headers |

---

### 🟡 Intermediate

| Lab | Title                      | Description |
|-----|----------------------------|-------------|
| 3   | [Python + Requests](intermediate/lab3_python_basics.md) | Learn to make basic API calls using Python |
| 4   | [Intro to Meraki SDK](intermediate/lab4_meraki_sdk_intro.md) | Use Cisco's official Python SDK to simplify API tasks |

---

### 🔴 Advanced

| Lab | Title                        | Description |
|-----|------------------------------|-------------|
| 5   | [Automation Scripts](advanced/lab5_automation_scripts.md) | Write scripts to automate bulk API operations |
| 6   | [Error Handling](advanced/lab6_error_handling.md)         | Handle API failures gracefully using logging and exceptions |
| 7   | [Bulk Config Updates](advanced/lab7_bulk_operations.md)   | Push config updates across multiple devices or networks |
| 8   | [Webhook Receiver](advanced/lab8_webhooks.md)             | Receive Meraki alerts in real-time via Flask server |
| 9   | [Postman Runner](advanced/lab9_postman_runner_chained_requests.md) | Use dynamic variables across chained requests in Postman |

---

## 🧰 Tools Used

- **Postman** – GUI-based API testing platform
- **Python** – General purpose scripting
- **Meraki SDK** – Official Python library from Cisco
- **Flask** – Lightweight web server for webhooks

---

## 📎 Resources and Assets

- Screenshots and example data files: [`assets/`](assets/)
- Sample Postman Collection: [`meraki_postman_collection.json`](assets/meraki_postman_collection.json)

---

## 🌐 GitHub Pages Setup

1. Upload this project to a GitHub repository.
2. Enable GitHub Pages in the repository settings.
3. Select the root (`/`) of the `main` branch as the publishing source.
4. Set a Jekyll theme like `cayman` for clean rendering.

---

## 🧠 Tip for Learners

Take your time to explore each lab. Every lab builds on the previous one. Try modifying parameters and test how the APIs respond.


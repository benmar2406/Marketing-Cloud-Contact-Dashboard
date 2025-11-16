# Marketing Cloud Internal Dashboard

**A modular, customizable dashboard for Salesforce Marketing Cloud (MC) to visualize marketing contacts, subscriber info, and unsubscribe trends.**

---
## Overview
This repository provides **modular code snippets** for building an internal Marketing Cloud dashboard as a **CloudPage**. The dashboard:
- Visualizes **available marketing contacts**, **All Subscribers info**, and **unsubscribe trends** (in percent).
- Includes a **search form** to retrieve **summarized information about single subscribers** (status, engagement, custom marketing data).
- Uses **SSJS (Server-Side JavaScript)** and **AMPScript** for backend logic.
- Handles **user authentication** to ensure only logged-in MC users can access the data.

The dashboard serves as a **unified view** for:
- **Subscriber status** (e.g., active, unsubscribed, bounced).
- **Engagement data** (e.g., last email received, opens, clicks).
- **Custom marketing info** (from your Master Data Extension).

---
## Prerequisites
To use this dashboard, you need:
1. **Salesforce Marketing Cloud account** with access to CloudPages and Code Resources.
2. **Data Extensions (DEs)**:
   - A **Master DE** with subscriber data (e.g., `ContactId`, `Email`, custom attributes...).
   - A **DE for unsubscribe trends** (e.g., `Date`, `UnsubscribeCount`, `PercentageChange`).
3. **Code Resource** in Marketing Cloud to process backend requests (e.g., for single subscriber lookups).
4. Basic knowledge of **SSJS, AMPScript, and JavaScript (Fetch API)**.

---
## 📂 Repository Structure
The repository contains **individual code snippets** for easy integration and customization:

| Filename                          | Description                                      |
|-----------------------------------|--------------------------------------------------|
| bar-chart.js                      | Visualizes data as a bar chart.                  |
| calculate-unsub-rate              | Calculates the unsubscribe rate.                 |
| fetch-request                     |  fetch request to code ressource.                     |
| general-data-master-de-and-subscribers | General data lookup for Master Data Extension and subscribers. |
| handle-search-request-code-resource | Code Resource for processing search requests.   |
| info-box                          | UI component for information boxes.              |
| landing-page                      | Main landing page of the dashboard.              |
| pie-and-line-chart                | Combined pie and line chart.                     |
| search-form                       | Search form for individual contacts.             |
| user-login-auth


---
## Setup Instructions

### 1. Clone or Download
```bash
git clone https://github.com/your-username/mc-dashboard.git

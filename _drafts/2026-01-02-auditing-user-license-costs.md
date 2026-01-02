---
title: "Identifying User's Last Login Dates via FetchXML 📊"
date: 2026-01-02
categories: [Dataverse, Audit]
---

One common question and high-stakes task I have encountered throughout my 14-year career—from CRM 2011 to modern Cloud engineering—is generating a list of users alongside their last login date. 🕒 This is particularly useful for **license cost audits** to ensure organizations aren't overpaying for inactive seats.

### The Challenge 🔍
Standard User views in Dataverse do not natively expose the "Last Login" date in an aggregatable format. To solve this efficiently without manual exports, we must tap into the **Audit** entity.

### The Solution: Aggregated FetchXML 🛠️
By targeting the `audit` entity and filtering for the `action` value of **64**, we can group by the User and extract the maximum (most recent) date.

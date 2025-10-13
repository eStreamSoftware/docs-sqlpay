---
title: Why show error message dataset "CalendarInfo" does not exist when batch email using customize payslip format?
description: A guide to solve error message dataset "CalendarInfo" does not exist when batch email using customize payslip format
slug: /faq/error-calendarinfo
tags: ["SQL Payroll", "FAQ", "Error"]
---

## Issue

Error message prompt when try to **Export to E-Mail Client (Batch)** using **customize payslip format**.

![error-issue](../../static/img/faq/error-calendarinfo/error-issue.jpg)

## Solution

At payslip report designer, change the **[\<Profile."RegisterNo">]** to **[\<Profile."BRN">]**

![error-solution](../../static/img/faq/error-calendarinfo/error-solution.jpg)

**After correction**, it will be look like the screenshot below.

![error-result](../../static/img/faq/error-calendarinfo/error-result.jpg)
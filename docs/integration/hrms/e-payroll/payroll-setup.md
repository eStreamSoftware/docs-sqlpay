---
sidebar_position: 1
title: Payroll Setup
description: An E Payroll setup guide in SQL Payroll
---

## Maintain Announcement

**Step 1:** Human Resource | Maintain Announcement… | Create New  
**Step 2:** Enter Title and Remark
- Remark is optional and visible in maintenance view only
  
**Step 3:** Select a Category and Date for the duration the Announcement will be visible to the employees  
  
  ![maintain-announcement1](../../../../static/img/integration/hrms/e-payroll/maintain-announcement1.png)

**Step 4:** Edit Note | Enter Note | Close Form | Yes  
  
  ![maintain-announcement2](../../../../static/img/integration/hrms/e-payroll/maintain-announcement2.png)

**Step 5:** Add Attachments  
- Maximum of 2 attachments are allowed
- Attachment extensions that are allowed: .jpg, .jpeg, .png, .pdf

**Step 6:** Save  

## Sync Cloud

### Payroll

**Step 1:** Cloud Icon | Sync Cloud… | Payroll  
  
  ![sync-cloud](../../../../static/img/integration/hrms/e-payroll/sync-cloud.png)

- To sync payroll details and payslip
  - Check ***'Include Employee Payroll Info'***
  - Select Year and Month
  - Check ***'Upload Payslip'***
  - Select Report format  
  
  | **Year** | **Month** | **Upload Payslip** | **Explanation** |    
  | :------- | :-------- | :----------------- | :-------------- |  
  | 2025 | 2 | Checked | **Payroll Details:** All details up till Feb 2025 will synced <br/> **Payslip:** Payslip for Feb 2025 will be synced |  
  | 2025 | 2 | Unchecked | **Payroll Details:** All details up till Feb 2025 will synced <br/> **Payslip:** No payslip will be synced |
  
- To Sync EA form
  - Check ***'Include EA Form Info'***
  - Check ***'Upload Payslip'***
  - Select Year and Report format

:::info
The Year and Month selected next to Payroll Info is for **Payroll Details** and **Payslip** only (it's not applicable to EA Form)
:::

**Step 2:** Click ***'Sync All'***

:::warning
A warning message will be prompt when user wants to sync **Payslip** earlier than their last synced date  

![sync-payslip](../../../../static/img/integration/hrms/e-payroll/sync-payslip.png)

Proceeding will cause **newer Payslip** to be deleted and user will have to resync each month individually again
:::

### Announcement

**Step:** Cloud Icon | Sync Cloud… | Sync All  

:::info
Make sure to always ***'Sync Cloud'*** when new Announcement is added or if there are any changes to the existing Announcement to ensure both Payroll and SQL HRMS app are in sync with one another
:::

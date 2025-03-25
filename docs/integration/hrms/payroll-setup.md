---
sidebar_position: 1
title: Payroll Setup
description: A general payroll setup guide
---

## SQL Drive

:::info
May contact SQL support to register an email address

Make sure you are login into an ADMIN user before proceed with the steps below
:::

**Step 1:** File | Company Profile... | Cloud Icon  
  
  ![sql-drive1](../../../static/img/integration/hrms/payroll-setup/sql-drive1.png)

**Step 2:** Turn on Drive  
  
  ![sql-drive2](../../../static/img/integration/hrms/payroll-setup/sql-drive2.png)

**Step 3:** Log in | Log in with Google | Enter Gmail account + password | Grant access  
  
  ![sql-drive3](../../../static/img/integration/hrms/payroll-setup/sql-drive3.png)

**Step 4:** Save

## SMTP

Before entering the SMTP settings, the user needs to create an app password using his company email address. This app password will be used for authentication when sending email using external program. If user do not have a company address, user can choose to get the app password using a Gmail or a Microsoft account. 

**Step 1:** Company Profile | General tab  
**Step 2:** Enter email that will be used to generate app password  
  
  ![smtp1](../../../static/img/integration/hrms/payroll-setup/smtp1.png)

**Step 3:** Go to Email Settings tab and fill in the required fields  
- **Host**
- **Gmail**: smtp.gmail.com
- **Microsoft Account**: smtp.office365.com
- **Port No**: 587
- **User**: Email used to generate the app password
- **Password**: The 16-character password generated in the email setup
 - **Sender Name**: Name of the sender

**Step 4:** Click Test Email
- User will receive an email under the email address used to generate the password upon successful
  
  ![smtp2](../../../static/img/integration/hrms/payroll-setup/smtp2.png)

## Email Setup

### Google Account

**Step 1:** Login to Google account  
**Step 2:** Turn on two-step verification  
  
  ![google-setup1](../../../static/img/integration/hrms/payroll-setup/google-setup1.png)

**Step 3:** In the search bar, enter ***'app passwords'*** and choose ***'App passwords'*** under ***'Security'***  
  
  ![google-setup2](../../../static/img/integration/hrms/payroll-setup/google-setup2.png)

**Step 4:** Enter a name for the App and click the ***'Create'*** button  
  
  ![google-setup3](../../../static/img/integration/hrms/payroll-setup/google-setup3.png)

**Step 5:** A 16-charactor password will be generated and follow the instructions under the ***'How to use it'*** section  
  
  ![google-setup4](../../../static/img/integration/hrms/payroll-setup/google-setup4.png)

### Microsoft Account

**Step 1:** Login to user Microsoft account  
**Step 2:** Direct to ***'Security'*** tab and click on ***'Manage how I sign in'***  
  
  ![microsoft-setup1](../../../static/img/integration/hrms/payroll-setup/microsoft-setup1.png)  

**Step 3:** Turn on ***'Two-step verification'***  
  
  ![microsoft-setup2](../../../static/img/integration/hrms/payroll-setup/microsoft-setup2.png)  

**Step 4:** Still in the ***'Security'*** page, scroll down to ***'App passwords'*** and click on ***'Create a new app password'***  
  
  ![microsoft-setup3](../../../static/img/integration/hrms/payroll-setup/microsoft-setup3.png)

**Step 5:** A 16-charactor password is generated

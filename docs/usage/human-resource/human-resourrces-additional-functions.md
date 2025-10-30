---
sidebar_position: 2
title: Guide
description: Guide
slug: /usage/human-resource/guide
tags: ["SQL Payroll", "HR", "Functions"]
---

## Bulk Email With Password

:::note

- Not applicable for Export Email Client or Export to PDF
- For Email Client, 10 records in one PDF, email to 1 recipient, system unable to generate password due to not sure which password should get

:::

### Prerequisites

:::info
In order to use this, user’s computer must configure with window email first
:::

### Setup

1. Navigate to **Human Resource** > **Maintain Employee**

2. Key in the PDF password and enter the email address

   ![des-maintain-employee-1](../../../static/img/usage/human-resource/hr-function-images/maintain-employee-1.png)

3. Next, go to **Payroll** > **Print Payslip**. Choose the month End Payslip, Apply and Preview

4. Click on the 🔽 beside the excel export, click on **Export to Email Client (Batch)**

   ![des-export-to-email-client-batch](../../../static/img/usage/human-resource/hr-function-images/export-to-email-client-batch.png)

   :::tip
   For Testing purpose, you may activate the module at File > Customize Payroll Module and ticked **Batch Email**
   :::

   ![des-batch-email](../../../static/img/usage/human-resource/hr-function-images/batch-email.png)

   :::warning Error
   If you haven't configure your window email, you will see an error message as below. Make sure yo have configure your window email before doing these steps.
   :::

   ![des-error](../../../static/img/usage/human-resource/hr-function-images/error.png)

### Simple Steps To use IC as PDF Password

1. Navigate to **Human Resource** > **Maintain Employee**

2. Click on one employee record, hold the `Shift` key in the keyboard and click on the last record to highlight all

3. Click on 🔽 button beside More, select Batch Edit

4. From the columns, click on field Chooser and select **Name2**, **New IC**

5. Save the structure, copy and paste the New IC value to Name2 column

![des-ic-as-pdf-password-1](../../../static/img/usage/human-resource/hr-function-images/ic-as-pdf-password-1.png)

![des-ic-as-pdf-password-2](../../../static/img/usage/human-resource/hr-function-images/ic-as-pdf-password-2.png)

![des-ic-as-pdf-password-3](../../../static/img/usage/human-resource/hr-function-images/ic-as-pdf-password-3.png)

![des-ic-as-pdf-password-4](../../../static/img/usage/human-resource/hr-function-images/ic-as-pdf-password-4.png)

## Employee Login

:::info
This guide explains how to configure and create an account for the employee in SQL Payroll which allow the employee to view their details
:::

### Employee Login Setup

1. In SQL Payroll, go to **Human Resource** > **Maintain Employee**

2. Click on **Change Password**

   ![des-change-password](../../../static/img/usage/human-resource/hr-function-images/change-password.png)

3. Enter a new password for the employee

   ![des-enter-password](../../../static/img/usage/human-resource/hr-function-images/enter-password.png)

4. Next, ask the employee to open SQL Payroll, login into it by using the **Employee Code** and **Password** configured previously. That's it! 🥳

   ![des-login](../../../static/img/usage/human-resource/hr-function-images/login.png)

5. Finally, here's an example of employee view

   ![des-employee-view](../../../static/img/usage/human-resource/hr-function-images/employee-view.png)

## Print Letter

:::info
This guide explains how to print Appointment, Confirmation, Increment letter
:::

### Print Letter Setup

1. Navigate to the **Maintain Employee** panel

   ![des-v](../../../static/img/usage/human-resource/hr-function-images/navigate.png)

2. Select the employee

   ![des-select-employee](../../../static/img/usage/human-resource/hr-function-images/select-employee.png)

3. Click preview reports

   ![des-preview-report](../../../static/img/usage/human-resource/hr-function-images/preview-report.png)

4. Select the report you want by double clicking it

   ![des-select-report](../../../static/img/usage/human-resource/hr-function-images/select-report.png)

5. This is the example of the appointment letter

   ![des-letter-example](../../../static/img/usage/human-resource/hr-function-images/letter-example.png)

#### Increment Letter

:::note
For increment letter, make sure increment is set in **history** in order for the report to work
:::

1. Navigate to **Human Resource** > **Maintain Employee**

   ![des-navigate-1](../../../static/img/usage/human-resource/hr-function-images/navigate-1.png)

2. Alternatively, you can click on the **Maintain Employee** available in the homepage

   ![des-navigate-2](../../../static/img/usage/human-resource/hr-function-images/navigate-2.png)

3. Go to the employee details, click on History from the tab view

   ![des-inc-letter-select-employee](../../../static/img/usage/human-resource/hr-function-images/inc-letter-select-employee.png)

4. Click preview reports

   ![des-inc-letter-click-preview](../../../static/img/usage/human-resource/hr-function-images/inc-letter-click-preview.png)

5. Select the report you want to print

   ![des-inc-letter-select-report](../../../static/img/usage/human-resource/hr-function-images/inc-letter-select-report.png)

#### Increment letter setup in history

![des-increment-letter-setup](../../../static/img/usage/human-resource/hr-function-images/increment-letter-setup.png)

## Maintain Employee with MyKad Reader

### MyKad Reader Setup

1. Link your Smart Card Reader to your computer

2. Reader will turn red light when you success link to your computer

   ![des-reader](../../../static/img/usage/human-resource/hr-function-images/reader.png)

3. Put MyKard into reader

4. Reader will show blue light when success read your MyKad

   ![des-plug-in-mykad](../../../static/img/usage/human-resource/hr-function-images/plug-in-mykad.png)

5. Open your SQL Payroll New Employee Profile > **Read MyKad**

   ![des-read-mykad](../../../static/img/usage/human-resource/hr-function-images/read-mykad.png)

6. Select **Reader Devices** > **Click Read Card**

   ![des-read-card](../../../static/img/usage/human-resource/hr-function-images/read-card.png)

7. Click **Read MyKad**

   ![des-read-mykad-physical](../../../static/img/usage/human-resource/hr-function-images/read-mykad-physical.png)

8. Inside System will auto fill up MyKard Detail

   - **(NAME , ADDRESS , ID Number, D.O.B, GENDER)**

   ![des-result](../../../static/img/usage/human-resource/hr-function-images/result.png)

## Recurring Zakat

### Recurring Zakat Setup

1. Go to **Maintain Employee**:

   ![des-maintain-employee-button](../../../static/img/usage/human-resource/hr-function-images/maintain-employee-button.png)

2. Select the respective employee and go to Deduction

   ![des-deduction](../../../static/img/usage/human-resource/hr-function-images/deduction.png)

3. Enter a deduction and tick Zakat check box. You will notice that the other contribution checkbox will be unticked

   ![des-check-zakat](../../../static/img/usage/human-resource/hr-function-images/check-zakat.png)

4. Key in Rate and set the period of contribution in the Date From and Date To column.

   ![des-key-in-rate](../../../static/img/usage/human-resource/hr-function-images/key-in-rate.png)

5. Save and process your month end. You will see the amount in your Gross Zakat

   ![des-result-1](../../../static/img/usage/human-resource/hr-function-images/result-1.png)

   ![des-result-2](../../../static/img/usage/human-resource/hr-function-images/result-2.png)

## Loan

:::note NOTE:
This is a **Paid Module**
:::

For company which also provide a loan for their employee(s) that is expected to be paid back by deduct from the salary with interest.

## Maintain Loan

At here allow the user to setting up the loan for the Selected Employee...

### Maintain Loan Setup

Assuming we had the following scenario:

| Field Name                  | Properties        |
|-----------------------------|-------------------|
| Employee Code               | 0010              |
| Loan Amount                 | 50,000            |
| Loan Interest               | 2,000             |
| Number of Repayment (Months)| 60                |
| First Repayment Date        | 01 Mar 2013       |

#### Loan Amount & Interest Amount

1. Click **New** & Enter As Following.

   ![des-maintain-loan-step-1](../../../static/img/usage/human-resource/hr-function-images/maintain-loan-step-1.jpg)

2. Click **Schedule | Generate**... Button.

   ![des-maintain-loan-step-2](../../../static/img/usage/human-resource/hr-function-images/maintain-loan-step-2.jpg)

3. Click **Ok** button to confirm.

4. Click **Save**.

#### Auto Repayment

1. Go to process as normal at [New Payroll](/usage/payroll/general#create-payroll).

2. At the Selected Employee Paysheet Click **Loan**.

   ![des-auto-repayment-step-1](../../../static/img/usage/human-resource/hr-function-images/auto-repayment-step-1.jpg)

#### Advanced Repayments

1. At **Transaction** Tab

   ![des-advanced-repayment-step-1](../../../static/img/usage/human-resource/hr-function-images/advanced-repayment-step-1.jpg)

## Print Loan Repayment History

This is to generate/print the Ledger/History of Loan given by company for the selected/All Employees Report...

![des-loan-repayment-history-step-1](../../../static/img/usage/human-resource/hr-function-images/loan-repayment-history-step-1.jpg)

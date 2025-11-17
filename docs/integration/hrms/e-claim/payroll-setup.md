---
sidebar_position: 1
title: Payroll Setup
description: An E Claim setup guide in SQL Payroll
---

## Maintain Claim

1. Navigate to Payroll > Maintenance > Maintain Claim…, select a Claim or Create New
2. Set Yearly Limit and Monthly Limit

    Option 1: Maintain Claim

    ![maintain-claim1](../../../../static/img/integration/hrms/e-claim/maintain-claim1.png)

    Option 2: Maintain Employee > Claim Limit tab

    ![maintain-claim2](../../../../static/img/integration/hrms/e-claim/maintain-claim2.png)

:::info
SQL Payroll/SQL HRMS app will prioritize claim limit set in Maintain Employee over the claim limit in Maintain Claim
:::

## Notification Settings 

1. Navigate to Company Profile > E HRMS tab 

![notification-settings](../../../../static/img/integration/hrms/e-claim/notification-settings.png)

- ***'Send EClaim Email Notification' checkbox***: Checked to allow E HRMS app to send claim email notifications to managers

## Manager Authority Settings

1. Navigate to Maintain Employee > E HRMS tab

![manage-authority-settings](../../../../static/img/integration/hrms/e-claim/manage-authority-settings.png)

- **_'Manager' checkbox_**: Checked to make the employee a manager
- **Manager Authority**:
  - Can Approve: Able to approve team’s claim submissions and leave applications
  - Can Review: Only able to verify team’s claim submissions and leave applications
- **Manager Team**: Select branch and department that will be managed by the employee

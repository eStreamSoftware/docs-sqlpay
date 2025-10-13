---
title: Batch Email
description: A guide to do batch email (Email Client Batch & SMTP Batch)
slug: /usage/general/batch-email
tags: ["SQL Payroll", "Batch Email", "Email Client Batch", "SMTP Batch"]
---

:::info[note]
Make sure you had done setting the template in Maintain Employee.
:::

## Setting in Maintain Employee

You can [CLICK HERE](<https://wiki.sql.com.my/wiki/Fast_Report_-_E-Mail_Client_(Batch)_%26_E-Mail_(Native)#Version_1.2021.196.166_.26_above>) to go Batch Email Link

1. Click on 3.2.2 Version 1.2021.196.166 & above

   ![wiki-batch-email](../../../static/img/usage/batch-email/wiki-batch-email.png)

2. Scroll down until see this Sample E-Mail Template (Version 1.2021.196.166 & above) > Click on Expand

   ![template](../../../static/img/usage/batch-email/template.png)

3. Copy all

   ![copy-template](../../../static/img/usage/batch-email/copy-template.png)

4. Open your SQL Payroll System

5. Navigate to **Human Resource** > **Maintain Employee** and click New

   ![new](../../../static/img/usage/batch-email/new.png)

6. Click 🔽 beside **More**

   ![more-dropdown](../../../static/img/usage/batch-email/more-dropdown.png)

7. Click on Paste Employee

   ![paste-employee](../../../static/img/usage/batch-email/paste-employee.png)

8. After Paste Employee you will see Employee Code as **EMAIL** and the PDF Password Setting at **Note**

   ![paste-employee-result](../../../static/img/usage/batch-email/paste-employee-result.png)

## Setting PDF Password

### Scenario 1 : Setting Employee Name 2 as password

:::info[note]
Only available in Version 1.2021.2066.174 & above
:::

1. At Note Tab:

   - **[UseName2]** Put 1 to enable it
   - **[GlobalPassword]** and **[PrivatePassword]** make sure is empty

   ```txt
   [UseName2]
   1

   [GlobalPassword]

   [PrivatePassword]
   ```

   ![employee-name-2-pdf-password-1](../../../static/img/usage/batch-email/employee-name-2-pdf-password-1.png)

2. Under Employee profile set the password at **Name 2**

   > For Example : **_testing_** is the PDF Password

   ![employee-name-2-pdf-password-2](../../../static/img/usage/batch-email/employee-name-2-pdf-password-2.png)

### Scenario 2 : Setting Global PDF Password by UseName and ICPass

> **\_UseNameICPass** - This setting is to use Employee Name and IC set as PDF password

1. At Note Tab:

   - **[UseName2]** Put 0 to disable it
   - **[PrivatePassword]** is empty

   ```txt
   [UseName2]
   0

   [GlobalPassword]
   UseNameICPass

   [PrivatePassword]
   EmployeeCode=Password
   ```

2. The first character of Employee Name (In Uppercase)

3. Second character is @

4. The subsequent 6 characters is the last 6 digits of NRIC or Passport Number

   For example :

   > Name : LEE CHONG WEI
   >
   > NRIC : 961212-01-4321
   >
   > The password is : **L@014321**

   ![global-pdf-password-usename-ic-pass](../../../static/img/usage/batch-email/global-pdf-password-usename-ic-pass.png)

### Scenario 3 : Setting Global PDF Password

:::info
This settings configures **all employees** to have the same password
:::

1. At Note Tab:

   - **[UseName2]** Put 0 to disable it
   - **[PrivatePassword]** is empty

   ```txt
   [UseName2]
   0

   [GlobalPassword]
   BatchEmail

   [PrivatePassword]
   EmployeeCode=Password
   ```

2. set the PDF Password below **[Global Password]**

   For example as below :

   > The PDF Password is **_‘BatchEmail’_**

   ![pdf-password-global](../../../static/img/usage/batch-email/pdf-password-global.png)

### Scenario 4 : Setting Private/ Individual Password

:::info[note]
Private Password - Each Employees got their own PDF Password

Must set for all Employees
:::

1. At Note Tab:

   - **[UseName2]** Put 0 to disable it
   - **[GlobalPassword]** is empty

   ```txt
   [UseName2]
   0

   [GlobalPassword]

   [PrivatePassword]
   EmployeeCode=Password
   001=LEE
   002=KOO
   ```

2. Under **[PrivatePasssword]**, put employee code and their password following the format below:

   ```txt
   Format : EmployeeCode=Password
   ```

   For Example as below :

   ```txt
   001=LEE ('LEE' is the PDF Password)

   002=KOO ('KOO' is the PDF Password)

   ```

   ![pdf-password-individual](../../../static/img/usage/batch-email/pdf-password-individual.png)

## Send Payslip by Batch Email

### E-Mail Client (Batch)

:::info[note]
Make sure your pc had install window email (Ex : Outlook or Thunderbird)
:::

1. Go to Payroll > Print Pay Slip ...

   ![email-client-print-payslip](../../../static/img/usage/batch-email/email-client-print-payslip.png)

2. Filter your process you wish to batch email > Apply

   ![email-client-filter](../../../static/img/usage/batch-email/email-client-filter.png)

3. Click 🔽 Beside Printer icon

4. Click on Export to E-Mail Client (Batch)

   ![email-client-more](../../../static/img/usage/batch-email/email-client-more.png)

5. Select your payslip format > OK

   ![email-client-select-payslip](../../../static/img/usage/batch-email/email-client-select-payslip.png)

6. After click ok will prompt window and show has been sent to recipient email, mean success send out

   ![email-client-send](../../../static/img/usage/batch-email/email-client-send.png)

### E-Mail SMTP (Batch)

:::info[note]
Make Sure you had create App Password

- If you’re using Gmail , you can [CLICK HERE](https://support.google.com/accounts/answer/185833?hl=en) to create your App Password

:::

1. Go to **File** > **Company Profile**

   ![smtp-company-profile](../../../static/img/usage/batch-email/smtp-company-profile.png)

2. Select Email Setting from the tabs

3. Fill in your email detail

   > \*\*Password : Is your App Password

   ![smtp-app-password](../../../static/img/usage/batch-email/smtp-app-password.png)

4. Go to **Payroll**, click **Print Pay Slip**

   ![smtp-print-payslip](../../../static/img/usage/batch-email/smtp-print-payslip.png)

5. Filter your process you wish to batch email > Apply

   ![smtp-filter](../../../static/img/usage/batch-email/smtp-filter.png)

6. Click 🔽 Beside Printer icon

7. Click on Export to E-Mail SMTP (Batch)

   ![smtp-export](../../../static/img/usage/batch-email/smtp-export.png)

8. Select your payslip format > OK

    ![smtp-select-payslip](../../../static/img/usage/batch-email/smtp-select-payslip.png)

9. After click ok will prompt window and show has been sent to recipient email, mean success send out

    ![smtp-send](../../../static/img/usage/batch-email/smtp-send.png)

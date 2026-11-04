---
sidebar_position: 1
title: Setup
description: Setup
slug: /usage/human-resource/setup
tags: ["SQL Payroll", "HR"]
---

## Maintain Employee

When a new employee joins the company, use the Maintain Employee section to enter their details.

1. Navigate to the Maintain Employee panel.

   ![des-navigate-1](../../../static/img/usage/human-resource/hr-setup-images/navigate-1.png)

   **OR Click on "Maintain Employee" on the home page**

   ![des-navigate-2](../../../static/img/usage/human-resource/hr-setup-images/navigate-2.png)

2. Click New to create a new employee.

   ![des-new-employee](../../../static/img/usage/human-resource/hr-setup-images/new-employee.png)

3. Enter the employee’s personal details.

   ![des-personal-tab-1](../../../static/img/usage/human-resource/hr-setup-images/personal-tab-1.jpg)

### Personal

Click the _Change Password_ button and enter a password to allow the employee to log in and view their payroll data and reports.
Remember to uncheck the _Active_ checkbox for any employee who has resigned before processing the payroll.

![des-personal-tab-1](../../../static/img/usage/human-resource/hr-setup-images/personal-tab-1.jpg)

| Field Name      | Properties                                                                                                 |
| --------------- | ---------------------------------------------------------------------------------------------------------- |
| Code            | Definition: Employee code                                                                                  |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 30                                                                                                 |
| Job Title       | Definition: Employee Job Title                                                                             |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 60                                                                                                 |
| Name            | Definition: Full Employee Name                                                                             |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 160                                                                                                |
| Active          | Definition: Unchecked if the selected employee is resigned.                                                |
|                 | Field Type: Boolean                                                                                        |
| Gender          | Definition: The employee Sex                                                                               |
|                 | Data Options: Male or Female                                                                               |
| D.O.B           | Definition: The employee Date of Birth                                                                     |
|                 | Field Type: Date (dd/MM/YYYY)                                                                              |
| Address         | Definition: Employee Correspondence Address                                                                |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 60 (for Each Line)                                                                                 |
| Phone           | Definition: Employee Correspondence Phone Number                                                           |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 20 (for Each Line)                                                                                 |
| Mobile          | Definition: Employee Handphone Number                                                                      |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 20                                                                                                 |
| Email           | Definition: Employee E-Mail Address                                                                        |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 60                                                                                                 |
| New IC          | Definition: Employee New Identity Card Number                                                              |
|                 | Field Type: Numerical                                                                                      |
|                 | Length: 20 (XXXXXX-XX-XXXX)                                                                                |
| Old IC          | Definition: Employee Old Identity Card Number                                                              |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 20                                                                                                 |
| Passport        | Definition: Employee Passport Number                                                                       |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 20                                                                                                 |
| Immigration No  | Definition: Employee Immigration Number                                                                    |
|                 | Field Type: Alphanumerical                                                                                 |
|                 | Length: 20                                                                                                 |
| Change Password | Definition: A password for Employee so he/she can self login to print his/her report (Eg EA, payslip, etc) |
|                 | Field Type: Alphanumerical                                                                                 |

### Grouping

This tab is used for report grouping for the selected employee. It can be organized by:

- [Branch](#maintain-branch)
- [Department](#maintain-department)
- [Group](#maintain-group)
- [Category](#maintain-category)
- [Project](#maintain-project)
- [Job](#maintain-job)
- [Task](#maintain-task)
- [Race](#maintain-race)
- [History Type](#maintain-history-type)
- [Announcement](#maintain-announcement)

![des-grouping-tab-1](../../../static/img/usage/human-resource/hr-setup-images/grouping-tab-1.jpg)

### Family

This tab is used to store spouse/family information.
It is useful for emergency contact purposes.

![des-family-tab-1](../../../static/img/usage/human-resource/hr-setup-images/family-tab-1.jpg)

| Field Name     | Properties                                                    |
| -------------- | ------------------------------------------------------------- |
| Spouse Name    | Definition: Employee husband/wife full name                   |
|                | Field Type: Alphanumerical                                    |
|                | Length: 160                                                   |
| Spouse Address | Definition: Employee husband/wife Correspondence Address      |
|                | Field Type: Alphanumerical                                    |
|                | Length: 60 (for Each Line)                                    |
| Spouse Phone   | Definition: Employee husband/wife Correspondence Phone Number |
|                | Field Type: Alphanumerical                                    |
|                | Length: 20 (for Each Line)                                    |
| Spouse Mobile  | Definition: Employee husband/wife Handphone Number            |
|                | Field Type: Alphanumerical                                    |
|                | Length: 20                                                    |
| Tax Branch     | Definition: Employee husband/wife Tax Branch                  |
|                | Field Type: Alphanumerical                                    |
|                | Length: 40                                                    |
| Tax No         | Definition: Employee husband/wife Tax Number                  |
|                | Field Type: Alphanumerical                                    |
|                | Length: 20                                                    |
| Spouse IC No   | Definition: Employee husband/wife New Identity Card Number    |
|                | Field Type: Alphanumerical                                    |
|                | Length: 20                                                    |

### Payroll Info

![des-payroll-tab-1](../../../static/img/usage/human-resource/hr-setup-images/payroll-tab-1.jpg)

| Field Name      | Properties                                                                                                                                                       | Field Name            | Properties                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------- | ------------------------------------------------------------------------------------- |
| Wages Type      | Definition: Employee [Wages](../payroll/setup.md#maintain-wages) Category Type                                                                                   | SOCSO No              | Definition: Employee SOCSO Number                                                     |
|                 |                                                                                                                                                                  |                       | Field Type: Alphanumerical                                                            |
|                 |                                                                                                                                                                  |                       | Length: 20                                                                            |
| Wages           | Definition: Employee wages amount                                                                                                                                | SOCSO Type            | Definition: Employee SOCSO Category                                                   |
|                 | Field Type: Numerical                                                                                                                                            |                       | Data Options: First Category, Second Category or No SOCSO                             |
| Contribution    | Definition: Employee [Contribution](../payroll/setup.md#maintain-contribution) Type                                                                              | Tax Branch            | Definition: Employee Tax Branch                                                       |
|                 |                                                                                                                                                                  |                       | Field Type: Alphanumerical                                                            |
|                 |                                                                                                                                                                  |                       | Length: 40                                                                            |
| Frequency       | Definition: Employee payment [Frequency](../payroll/setup.md#maintain-frequency)                                                                                 | Tax No                | Definition: Employee Tax Number                                                       |
|                 |                                                                                                                                                                  |                       | Field Type: Alphanumerical                                                            |
|                 |                                                                                                                                                                  |                       | Length: 20                                                                            |
| Payment Method  | Definition: Employer [Payment Method](../payroll/setup.md#maintain-payment-method)                                                                               | Marital Status        | Definition: Employee marriage status                                                  |
|                 |                                                                                                                                                                  |                       | Data Options: Single, Married, Divorced or Widow                                      |
| Bank            | Definition: Employee Bank                                                                                                                                        | Spouse Working        | Definition: Tick if the Employee husband/wife is working                              |
|                 |                                                                                                                                                                  |                       | Field Type: Boolean                                                                   |
| Bank Account No | Definition: Employee Bank Account Number                                                                                                                         | Spouse Disabled       | Definition: Tick if the Employee husband/wife is disable person                       |
|                 | Field Type: Alphanumerical                                                                                                                                       |                       | Field Type: Boolean                                                                   |
|                 | Length: 20                                                                                                                                                       |                       |                                                                                       |
| Self Disabled   | Definition: Tick if the Employee is disable person                                                                                                               | Tax Category          | Definition: Employee Tax Category. Only can select if Override Tax Category is Tick.  |
|                 | Field Type: Boolean                                                                                                                                              |                       |                                                                                       |
| Resident        | Definition: Untick if the Employee Foreigner                                                                                                                     | Override Tax Category | Definition: Tick if don't wanted System Automatic Calculate the Employee Tax Category |
|                 | Field Type: Boolean                                                                                                                                              |                       | Field Type: Boolean                                                                   |
|                 | Non-Resident requirement and tax rate, refer to [Non-Resident](https://www.hasil.gov.my/en/individual/individual-life-cycle/how-to-declare-income/non-resident/) |                       |                                                                                       |
| EPF No          | Definition: Employee EPF(KWSP) Number                                                                                                                            | EA Serial No          | Definition: Employee EA Serial Number (Given by LHDN Department)                      |
|                 | Field Type: Alphanumerical                                                                                                                                       |                       | Field Type: Alphanumerical                                                            |
|                 | Length: 20                                                                                                                                                       |                       | Length: 8                                                                             |
| NK              | Definition: Employee NK Code (can be seen on EPF Borang A)                                                                                                       | Join Date             | Definition: Employee Join the Company Date                                            |
|                 | Field Type: Alphanumerical                                                                                                                                       |                       | Field Type: Date (dd/MM/yyyy)                                                         |
|                 | Length: 1                                                                                                                                                        |                       |                                                                                       |
| Initial         | Definition: Employee Initial Code (Given by EPF Department)                                                                                                      | Confirm Date          | Definition: Employee Confirmation Date                                                |
|                 | Field Type: Alphanumerical                                                                                                                                       |                       | Field Type: Date (dd/MM/yyyy)                                                         |
|                 | Length: 3                                                                                                                                                        |                       |                                                                                       |
|                 |                                                                                                                                                                  | Resign Date           | Definition: Employee Resign Date                                                      |
|                 |                                                                                                                                                                  |                       | Field Type: Date (dd/MM/yyyy)                                                         |

### Allowance

Use this tab to enter the Fixed [Allowance](../payroll/setup.md#maintain-allowance) entitled for each month for the selected employee.

![des-allowance-tab-1](../../../static/img/usage/human-resource/hr-setup-images/allowance-tab-1.jpg)

### Deduction

Use this tab to enter the Fixed [Deduction](../payroll/setup.md#maintain-deduction) entitled for each month for the selected employee.

![des-deduction-tab-1](../../../static/img/usage/human-resource/hr-setup-images/deduction-tab-1.jpg)

### Note

Use this tab to upload a photo and other information for the selected employee.
For the photo, please ensure:

1. It is saved as a JPEG file.
2. The JPEG file size is under 200KB.

![des-note-tab-1](../../../static/img/usage/human-resource/hr-setup-images/note-tab-1.jpg)

### History

This tab shows the history of changes for the selected employee.
Select "Increment" in the type column to print the Increment Letter (HR.Employee.Increment.Report).

![des-history-tab-1](../../../static/img/usage/human-resource/hr-setup-images/history-tab-1.jpg)

| Field Name  | Properties                                                 |
| ----------- | ---------------------------------------------------------- |
| Post Date   | Definition: Date of the data changes                       |
|             | Field Type: Date                                           |
| Type        | Definition: Changes [History Type](#maintain-history-type) |
| Description | Definition: Detail of Data changes                         |

### Child

This tab lists all tax-deductible children.

![des-child-tab-1](../../../static/img/usage/human-resource/hr-setup-images/child-tab-1.jpg)

| Field Name         | Properties                                                                                        |
| ------------------ | ------------------------------------------------------------------------------------------------- |
| Name               | Definition: Employee Tax Deductable Children full name                                            |
|                    | Field Type: Alphanumerical                                                                        |
|                    | Length: 160                                                                                       |
| D.O.B.             | Definition: Employee Tax Deductable Children date of birth.                                       |
|                    | Field Type: Date (dd/MM/yyyy)                                                                     |
|                    | Data Option: Optional (i.e. may leave it empty if don't wanted system calculate the Children Age) |
| Tax Code           | Definition: Tax Deductable Children code.                                                         |
| Rate               | Definition: Rate for Tax Deductable                                                               |
|                    | Field Type: Numerical                                                                             |
|                    | Data Options: 1 or 0.5                                                                            |
| Number of Children | Definition: Number of Children is use for Tax Calculation. (Auto Calculate)                       |

### Attachments

Attach files related to the selected employee (e.g., Letter of Offer).
Ensure the file is stored on the server, as the system only stores the file path.

![des-attachments-tab-1](../../../static/img/usage/human-resource/hr-setup-images/attachments-tab-1.jpg)

## Maintain Branch

This is useful for companies with multiple branches where the salary is paid from HQ.

![des-maintain-branch-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-branch-1.jpg)

| Field Name     | Properties                                                                                                                         |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Branch Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Branch (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected branch code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Branch Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Department

A division of an organization, such as Accounts, Marketing, etc.

![des-maintain-department-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-department-1.jpg)

| Field Name     | Properties                                                                                                                             |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Department Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Department (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Department code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Department Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Group

Another method for grouping employees in reports.

![des-maintain-group-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-group-1.jpg)

| Field Name     | Properties                                                                                                                        |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Group Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Group (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Group code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Group Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Category

Divide employees by class or division.

![des-maintain-category-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-category-1.jpg)

| Field Name     | Properties                                                                                                                           |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Code           | A Category Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Category (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Category Code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Category Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Project

Group employees by the project they are working on.

![des-maintain-project-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-project-1.jpg)

| Field Name     | Properties                                                                                                                          |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Project Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Project (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Project Code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Project Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Job

Group employees by job type for reporting.

![des-maintain-job-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-job-1.jpg)

| Field Name     | Properties                                                                                                                      |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Job Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Job (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Job Code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Job Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Task

Divide employees by specific tasks.

![des-maintain-task-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-task-1.jpg)

| Field Name     | Properties                                                                                                                       |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Project Code (Max 20 Characters)                                                                                               |
| Description    | A Full Description for Task (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Task Code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Task Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain Race

Group employees by race for reporting.

![des-maintain-race-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-race-1.jpg)

| Field Name     | Properties                                                                                                                       |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A Race Code (Max 20 Characters)                                                                                                  |
| Description    | A Full Description for Race (Max 160 Characters)                                                                                 |
| Active         | Uncheck if the selected Race Code is unavailable                                                                                 |
| Set as Default | Click this button to automatically assign this Race Code when creating a new employee at [Maintain Employee](#maintain-employee) |

## Maintain History Type

Allows users to group changes made in Maintain Employee.

![des-maintain-history-type-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-history-type-1.jpg)

| Field Name     | Properties                                                                                                                          |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| Code           | A History Type Code (Max 20 Characters)                                                                                             |
| Description    | A Full Description for History Type (Max 160 Characters)                                                                            |
| Active         | Uncheck if the selected History Type Code is unavailable                                                                            |
| Set as Default | Click this button to automatically assign this History Type Code when making new changes at [Maintain Employee](#maintain-employee) |

## Maintain Announcement

Used to create, manage, and distribute company-wide or employee-specific announcements within the payroll and HR system, allowing users to share information, updates, or important reminders with their team.

![des-maintain-announcement-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-announcement-1.png)

| Field Name | Properties                                                                        |
| ---------- | --------------------------------------------------------------------------------- |
| Title      | The title or subject of the announcement.                                         |
| Date From  | The start date when the announcement becomes active.                              |
| Date To    | The end date when the announcement expires or becomes inactive.                   |
| Category   | The classification or type of announcement (e.g., General, System Update, Event). |
| Remark     | Additional notes or comments related to the announcement.                         |

## Contract Stamp Duty

Stamp duty is a tax imposed on certain legal documents to make them officially recognized for legal purposes. In Malaysia, employment agreements are considered a type of agreement document that may require stamping under the Stamp Act 1949.

Once stamped, the contract can be used as legal evidence in court if disputes arise.

#### Key Details for 2025-2026

1. **Contracts Signed Before 1 Jan 2025**
   - Exempt from stamp duty
   - Late stamping penalties are also waived
2. **Contracts Signed Between 1 Jan 2025 – 31 Dec 2025**
   - Stamp duty is still required (RM10 per contract)
   - Late stamping penalties are waived if the contract is stamped on or before 31 Dec 2025
3. **Contracts Signed From 1 Jan 2026 Onwards**
   - Stamp duty applies (RM10 per contract)
   - Must be stamped within the stipulated period
   - Late stamping penalties will be enforced

For employment agreements, stamp duty is generally:

- RM10 per copy of the agreement

Each stamped copy is treated as a separate document.

Stamp duty should be paid:

- Within 30 days after the agreement is signed in Malaysia, or
- Within 30 days after the document is received in Malaysia if signed overseas.

Stamp duty can be submitted through the STAMP system managed by Lembaga Hasil Dalam Negeri Malaysia (LHDN).

Submission methods include:

- Online via STAMP system (e-Stamp Duty)
- Physical submission at LHDN stamp duty offices

#### Stamp Duty Late Penalty

If a document is not stamped within the stipulated period, the following penalties may apply:

| Delay Period | Penalty |
| --- | --- |
| Within 3 months after the due date | RM50.00 or 10% of the deficient duty, whichever is higher |
| More than 3 months after the due date | RM100.00 or 20% of the deficient duty, whichever is higher |

The Stamp Duty function is available from SQL version 296.236 onwards.

### Mandatory Fields Before Stamp Duty

Fill in the mandatory information below before processing the stamp duty.

1. Company Profile - File | Company Profile

   ![Company Profile fields for contract stamp duty](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-company-profile.png)

2. Employee Profile - Human Resources | Maintain Employee

   ![Employee Profile fields for contract stamp duty](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-employee-profile.png)

Once done filling all the information above, you can start creating the Contract Stamp Duty in SQL Payroll.

### Steps to Generate Stamp Duty

1. Go to Human Resource | Contract Stamp Duty

   ![Navigate to Contract Stamp Duty](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-navigate.png)

2. Click New to create a contract for the newly joined staff

   ![Create a new contract stamp duty record](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-new.png)

3. Select the Employee Code

   ![Select the employee code](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-select-employee.png)

4. Enter the Contract Date, Title, Details, and Salary Amount

   ![Enter contract details](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-enter-details.png)

5. Attach the employment contract file such as Offer Letter (must signed by the employee)

   * must at least attach min 1 attachment

   ![Attach the signed employment contract](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-attach-contract.png)

6. Click Save to complete the entry

   ![Save the contract stamp duty record](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-save.png)

7. Go to Human Resource | Print Contract Stamp Duty Listing

   ![Open Print Contract Stamp Duty Listing](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-print-listing.png)

8. Select the Date Period and click Apply to display the records

   ![Apply the date period](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-apply-period.png)

8. Click the Save to File icon to download the stamp duty upload file

   ![Export the stamp duty upload file](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-export-file.png)

7. Once the download is completed, the system will generate an XML file for the contract stamp duty submission

   ![Download the generated XML file](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-xml-download.png)

   ![Generated contract stamp duty XML file](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-xml-file.png)

### Stamp Duty Submission

1. Login E-Stamp Duty via MyTax portal

   ![Sign in to e-Stamp Duty through MyTax](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-mytax-login.png)

2. Click Continue to proceed further

   ![Continue in e-Stamp Duty](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-continue.png)

3. Select Company Role

   ![Select the company role](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-company-role.png)

4. Login as your company agent

   ![Sign in as the company agent](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-company-agent.png)

5. Go to Borong Permohonan | Penyeteman Berkelompok

   ![Open Penyeteman Berkelompok](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-borang-permohonan.png)

6. Click Choose File to upload the XML file exported from SQL

   ![Choose the exported XML file](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-choose-file.png)

7. Once done, click Muat Naik to upload

   ![Upload the XML file](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-upload.png)

8. Employee list are shown as below

   ![Review the employee list](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-employee-list.png)

9. Fill in the information at the above and tick the agreement

   ![Complete agreement details](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-agreement-details.png)

10. Click Proses to continue

   ![Process the submission](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-proses.png)

11. Make sure the information is correct, and click Teruskan to proceed

   ![Continue the submission](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-teruskan.png)

12. After receiving the Batch Number for the stamping submission, wait for verification by LHDN

   ![Batch number after submission](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-batch-number.png)

13. Go to Senarai | Penyeteman Berkelompok

14. Click the Batch Number that has not been submitted yet

   ![Select an unsubmitted batch number](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-select-batch.png)

15. Once the status changes to “Taksir Sendiri Duti”, the stamp duty and penalty amount will be displayed

   ![Review self-assessed duty and penalty](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-self-assess.png)

16. Tick the Certificate checkbox to confirm the submission

   ![Confirm the submission certificate](../../../static/img/usage/human-resource/hr-setup-images/contract-stamp-duty-confirm-certificate.png)

17. Proceed to make the stamp duty payment

## Print History Listing

This provides a comprehensive record of all past history types for employees. You can filter, sort, and group employees using the fields below.

![des-print-history-listing-1](../../../static/img/usage/human-resource/hr-setup-images/print-history-listing-1.png)

This is how the generated report will look:

![des-print-history-listing-2](../../../static/img/usage/human-resource/hr-setup-images/print-history-listing-2.png)

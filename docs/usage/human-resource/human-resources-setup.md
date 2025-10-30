---
sidebar_position: 1
title: Setup
description: Setup
slug: /usage/human-resource/setup
tags: ["SQL Payroll", "HR"]
---

## Maintain Employee

Whenever a new staff/worker/person/crew enter the company, Maintain Employee is the place where user needs to key in the details

1. Navigate yourself to the Maintain Employee panel

   ![des-navigate-1](../../../static/img/usage/human-resource/hr-setup-images/navigate-1.png)

   \*OR Click on the home page "Maintain Employee"\*\*

   ![des-navigate-2](../../../static/img/usage/human-resource/hr-setup-images/navigate-2.png)

2. Click new to create new employee

   ![des-new-employee](../../../static/img/usage/human-resource/hr-setup-images/new-employee.png)

3. Key in the employee’s personal details

   ![des-personal-tab-1](../../../static/img/usage/human-resource/hr-setup-images/personal-tab-1.jpg)

### Personal

Click the *Change Password* button & enter the password if you wanted to allow the Employee to login to see his/her own payroll data & report
Remember to untick the *Active* for any employee had resign before process the payroll.

![des-personal-tab-1](../../../static/img/usage/human-resource/hr-setup-images/personal-tab-1.jpg)

| Field Name      | Properties |
|-----------------|------------|
| Code            | Definition: Employee code |
|                 | Field Type: Alphanumerical |
|                 | Length: 30 |
| Job Title       | Definition: Employee Job Title |
|                 | Field Type: Alphanumerical |
|                 | Length: 60 |
| Name            | Definition: Full Employee Name |
|                 | Field Type: Alphanumerical |
|                 | Length: 160 |
| Active          | Definition: Unchecked if the selected employee is resigned. |
|                 | Field Type: Boolean |
| Gender          | Definition: The employee Sex |
|                 | Data Options: Male or Female |
| D.O.B           | Definition: The employee Date of Birth |
|                 | Field Type: Date (dd/MM/YYYY) |
| Address         | Definition: Employee Correspondence Address |
|                 | Field Type: Alphanumerical |
|                 | Length: 60 (for Each Line) |
| Phone           | Definition: Employee Correspondence Phone Number |
|                 | Field Type: Alphanumerical |
|                 | Length: 20 (for Each Line) |
| Mobile          | Definition: Employee Handphone Number |
|                 | Field Type: Alphanumerical |
|                 | Length: 20 |
| Email           | Definition: Employee E-Mail Address |
|                 | Field Type: Alphanumerical |
|                 | Length: 60 |
| New IC          | Definition: Employee New Identity Card Number |
|                 | Field Type: Numerical |
|                 | Length: 20 (XXXXXX-XX-XXXX) |
| Old IC          | Definition: Employee Old Identity Card Number |
|                 | Field Type: Alphanumerical |
|                 | Length: 20 |
| Passport        | Definition: Employee Passport Number |
|                 | Field Type: Alphanumerical |
|                 | Length: 20 |
| Immigration No  | Definition: Employee Immigration Number |
|                 | Field Type: Alphanumerical |
|                 | Length: 20 |
| Change Password | Definition: A password for Employee so he/she can self login to print his/her report (Eg EA, payslip, etc) |
|                 | Field Type: Alphanumerical |

### Grouping

In this tab is use for report grouping for the selected employee. It can be either by

- [Branch](../../usage/human-resource/human-resources-setup.md#maintain-branch)
- [Department](../../usage/human-resource/human-resources-setup.md#maintain-department)
- [Group](../../usage/human-resource/human-resources-setup.md#maintain-group)
- [Category](../../usage/human-resource/human-resources-setup.md#maintain-category)
- [Project](../../usage/human-resource/human-resources-setup.md#maintain-project)
- [Job](../../usage/human-resource/human-resources-setup.md#maintain-job)
- [Task](../../usage/human-resource/human-resources-setup.md#maintain-task)
- [Race](../../usage/human-resource/human-resources-setup.md#maintain-race)
- [History Type](../../usage/human-resource/human-resources-setup.md#maintain-history-type)
- [Announcement](../../usage/human-resource/human-resources-setup.md#maintain-announcement)

![des-grouping-tab-1](../../../static/img/usage/human-resource/hr-setup-images/grouping-tab-1.jpg)

### Family

In this tab is use to keep the his/her spouse/family information.
It is useful in case anything happen to the employee we able to inform/contact his/her spouse/family

![des-family-tab-1](../../../static/img/usage/human-resource/hr-setup-images/family-tab-1.jpg)

| Field Name     | Properties |
|----------------|------------|
| Spouse Name    | Definition: Employee husband/wife full name |
|                | Field Type: Alphanumerical                  |
|                | Length: 160                                 |
| Spouse Address | Definition: Employee husband/wife Correspondence Address |
|                | Field Type: Alphanumerical                  |
|                | Length: 60 (for Each Line)                  |
| Spouse Phone   | Definition: Employee husband/wife Correspondence Phone Number |
|                | Field Type: Alphanumerical                  |
|                | Length: 20 (for Each Line)                  |
| Spouse Mobile  | Definition: Employee husband/wife Handphone Number |
|                | Field Type: Alphanumerical                  |
|                | Length: 20                                  |
| Tax Branch     | Definition: Employee husband/wife Tax Branch |
|                | Field Type: Alphanumerical                  |
|                | Length: 40                                  |
| Tax No         | Definition: Employee husband/wife Tax Number |
|                | Field Type: Alphanumerical                  |
|                | Length: 20                                  |
| Spouse IC No   | Definition: Employee husband/wife New Identity Card Number |
|                | Field Type: Alphanumerical                  |
|                | Length: 20                                  |

### Payroll Info

![des-payroll-tab-1](../../../static/img/usage/human-resource/hr-setup-images/payroll-tab-1.jpg)

| Field Name       | Properties | Field Name       | Properties |
|------------------|------------|------------------|------------|
| Wages Type       | Definition: Employee [Wages](/usage/payroll/setup#maintain-wages) Category Type | SOCSO No        | Definition: Employee SOCSO Number |
|                  |            |                  | Field Type: Alphanumerical |
|                  |            |                  | Length: 20 |
| Wages            | Definition: Employee wages amount | SOCSO Type      | Definition: Employee SOCSO Category |
|                  | Field Type: Numerical |                  | Data Options: First Category, Second Category or No SOCSO |
| Contribution     | Definition: Employee [Contribution](/usage/payroll/setup#maintain-contribution) Type | Tax Branch      | Definition: Employee Tax Branch |
|                  |            |                  | Field Type: Alphanumerical |
|                  |            |                  | Length: 40 |
| Frequency        | Definition: Employee payment [Frequency](/usage/payroll/setup#maintain-frequency) | Tax No          | Definition: Employee Tax Number |
|                  |            |                  | Field Type: Alphanumerical |
|                  |            |                  | Length: 20 |
| Payment Method   | Definition: Employer [Payment Method](/usage/payroll/setup#maintain-payment-method) | Marital Status   | Definition: Employee marriage status |
|                  |            |                  | Data Options: Single, Married, Divorced or Widow |
| Bank             | Definition: Employee Bank | Spouse Working  | Definition: Tick if the Employee husband/wife is working |
|                  |            |                  | Field Type: Boolean |
| Bank Account No  | Definition: Employee Bank Account Number | Spouse Disabled | Definition: Tick if the Employee husband/wife is disable person |
|                  | Field Type: Alphanumerical |                  | Field Type: Boolean |
|                  | Length: 20 |                  | |
| Self Disabled    | Definition: Tick if the Employee is disable person | Tax Category    | Definition: Employee Tax Category. Only can select if Override Tax Category is Tick. |
|                  | Field Type: Boolean |                  | |
| Resident         | Definition: Untick if the Employee Foreigner | Override Tax Category | Definition: Tick if don't wanted System Automatic Calculate the Employee Tax Category |
|                  | Field Type: Boolean |                  | Field Type: Boolean |
|                  | Non-Resident requirement and tax rate, refer to [Non-Resident](https://www.hasil.gov.my/en/individual/individual-life-cycle/how-to-declare-income/non-resident/) |                  | |
| EPF No           | Definition: Employee EPF(KWSP) Number | EA Serial No    | Definition: Employee EA Serial Number (Given by LHDN Department) |
|                  | Field Type: Alphanumerical |                  | Field Type: Alphanumerical |
|                  | Length: 20 |                  | Length: 8 |
| NK               | Definition: Employee NK Code (can be seen on EPF Borang A) | Join Date       | Definition: Employee Join the Company Date |
|                  | Field Type: Alphanumerical |                  | Field Type: Date (dd/MM/yyyy) |
|                  | Length: 1 |                  | |
| Initial          | Definition: Employee Initial Code (Given by EPF Department) | Confirm Date    | Definition: Employee Confirmation Date |
|                  | Field Type: Alphanumerical |                  | Field Type: Date (dd/MM/yyyy) |
|                  | Length: 3 |                  | |
|                  |           |     Resign Date             |Definition: Employee Resign Date |
|       |  |                  | Field Type: Date (dd/MM/yyyy) |

### Allowance

In this Tab is to enter the Fixed [Allowance](/usage/payroll/setup#maintain-allowance) entitled for each month for selected Employee.

![des-allowance-tab-1](../../../static/img/usage/human-resource/hr-setup-images/allowance-tab-1.jpg)

### Deduction

In this Tab is to enter the Fixed [Deduction](/usage/payroll/setup#maintain-deduction) entitled for each month for selected Employee.

![des-deduction-tab-1](../../../static/img/usage/human-resource/hr-setup-images/deduction-tab-1.jpg)

### Note

In this Tab user can load the Photo & other Information for the selected Employee.
For Photo please try

   1. Save in Jpeg file.
   2. The Jpeg file size limit as 200KB

![des-note-tab-1](../../../static/img/usage/human-resource/hr-setup-images/note-tab-1.jpg)

### History

In this tab is to show the list of history changes in this selected Employee.
Select the Increment at the type column in order to print the Increment Letter (HR.Employee.Increment.Report).

![des-history-tab-1](../../../static/img/usage/human-resource/hr-setup-images/history-tab-1.jpg)

| Field Name   | Properties                          |
|--------------|-------------------------------------|
| Post Date    | Definition: Date of the data changes |
|              | Field Type: Date                    |
| Type         | Definition: Changes [History Type](../../usage/human-resource/setup#maintain-history-type)    |
| Description  | Definition: Detail of Data changes  |

### Child

In this tab is to list out all taxable children(s).

![des-child-tab-1](../../../static/img/usage/human-resource/hr-setup-images/child-tab-1.jpg)

| Field Name         | Properties                                                                                           |
|--------------------|------------------------------------------------------------------------------------------------------|
| Name               | Definition: Employee Tax Deductable Children full name                                                |
|                    | Field Type: Alphanumerical                                                                            |
|                    | Length: 160                                                                                          |
| D.O.B.             | Definition: Employee Tax Deductable Children date of birth.                                           |
|                    | Field Type: Date (dd/MM/yyyy)                                                                         |
|                    | Data Option: Optional (i.e. may leave it empty if don't wanted system calculate the Children Age)     |
| Tax Code           | Definition: Tax Deductable Children code.                                                             |
| Rate               | Definition: Rate for Tax Deductable                                                                   |
|                    | Field Type: Numerical                                                                                 |
|                    | Data Options: 1 or 0.5                                                                                |
| Number of Children | Definition: Number of Children is use for Tax Calculation. (Auto Calculate)                           |

### Attachments

Here user can attach the file to selected employee (eg Letter of Offer).
Make sure the file is keep in the server as the system only keep the file link/path only.

![des-attachments-tab-1](../../../static/img/usage/human-resource/hr-setup-images/attachments-tab-1.jpg)

## Maintain Branch

This is useful for user had many branch company but the salary is paid from HQ.

![des-maintain-branch-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-branch-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Branch Code (Max 20 Character)                                           |
| Description    | A Full Description for Branch (Max 160 Character)                         |
| Active         | Untick it if the selected branch code is unavailable                       |
| Set as Default | Click This button if wanted the selected Branch Code to be Auto Assign this Branch Code on New at [Maintain Employee](/usage/human-resource/setup#maintain-employee) |

## Maintain Department

A division of a large organization such as Account, Marketing & etc.

![des-maintain-department-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-department-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Department Code (Max 20 Character)                                       |
| Description    | A Full Description for Department (Max 160 Character)                      |
| Active         | Untick it if the selected Department code is unavailable                   |
| Set as Default | Click This button if wanted the selected Department Code to be Auto Assign this Department Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Group

This is another type of report grouping by Group type.

![des-maintain-group-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-group-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Group Code (Max 20 Character)                                            |
| Description    | A Full Description for Group (Max 160 Character)                          |
| Active         | Untick it if the selected Group code is unavailable                        |
| Set as Default | Click This button if wanted the selected Group Code to be Auto Assign this Group Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Category

User also can divide the employee by class or division.

![des-maintain-category-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-category-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Category Code (Max 20 Character)                                         |
| Description    | A Full Description for Category (Max 160 Character)                        |
| Active         | Untick it if the selected Category Code is unavailable                     |
| Set as Default | Click This button if wanted the selected Category Code to be Auto Assign this Category Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Project

User also can Group the employee by Project which the employee work at.

![des-maintain-project-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-project-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Project Code (Max 20 Character)                                          |
| Description    | A Full Description for Project (Max 160 Character)                         |
| Active         | Untick it if the selected Project Code is unavailable                      |
| Set as Default | Click This button if wanted the selected Project Code to be Auto Assign this Project Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Job

User also can Group the employee by Job Type in report.

![des-maintain-job-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-job-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Job Code (Max 20 Character)                                              |
| Description    | A Full Description for Job (Max 160 Character)                             |
| Active         | Untick it if the selected Job Code is unavailable                          |
| Set as Default | Click This button if wanted the selected Job Code to be Auto Assign this Job Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Task

User also can divide the employee by piece of work to be done or undertaken.

![des-maintain-task-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-task-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Project Code (Max 20 Character)                                          |
| Description    | A Full Description for Task (Max 160 Character)                            |
| Active         | Untick it if the selected Task Code is unavailable                         |
| Set as Default | Click This button if wanted the selected Task Code to be Auto Assign this Task Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Race

User also can Group the employee by Race Type in report.

![des-maintain-race-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-race-1.jpg)

| Field Name     | Properties                                                                 |
|----------------|----------------------------------------------------------------------------|
| Code           | A Race Code (Max 20 Character)                                             |
| Description    | A Full Description for Race (Max 160 Character)                            |
| Active         | Untick it if the selected Race Code is unavailable                         |
| Set as Default | Click This button if wanted the selected Race Code to be Auto Assign this Race Code on New at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain History Type

This is to use to allow user to Group the Changes in the Maintain Employee

![des-maintain-history-type-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-history-type-1.jpg)

| Field Name     | Properties                                                                                     |
|----------------|------------------------------------------------------------------------------------------------|
| Code           | A History Type Code (Max 20 Character)                                                         |
| Description    | A Full Description for History Type (Max 160 Character)                                        |
| Active         | Untick it if the selected History Type Code is unavailable                                     |
| Set as Default | Click This button if wanted the selected History Type Code to be Auto Assign this History Type Code on New Changes at [Maintain Employee](../../usage/human-resource/setup#maintain-employee) |

## Maintain Announcement

This is to used to create, manage, and distribute company-wide or employee-specific announcements within the payroll and HR system, allowing users to share information, updates, or important reminders with their team

![des-maintain-announcement-1](../../../static/img/usage/human-resource/hr-setup-images/maintain-announcement-1.png)

| Field Name | Properties |
|-------------|-------------|
| Title | The title or subject of the announcement. |
| Date From | The start date when the announcement becomes active. |
| Date To | The end date when the announcement expires or becomes inactive. |
| Category | The classification or type of announcement (e.g., General, System Update, Event). |
| Remark | Additional notes or comments related to the announcement. |

## Print History Lisitng

This provides a comprehensive record of all past history types for employees, and is able to furthur and filter, sort and group the employees witth the fields below

![des-print-history-listing-1](../../../static/img/usage/human-resource/hr-setup-images/print-history-listing-1.png)

This is how the report generated will look like

![des-print-history-listing-2](../../../static/img/usage/human-resource/hr-setup-images/print-history-listing-2.png)

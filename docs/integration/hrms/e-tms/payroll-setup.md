---
sidebar_position: 1
title: Payroll Setup
description: An E TMS setup guide in SQL Payroll
---

## Time Zone

1. Navigate to Company Profile > General > Time Zone and select your country time zone

   ![maintain-timezone](../../../../static/img/integration/hrms/e-tms/maintain-timezone.png)

2. Save

## Maintain Branch

1. Navigate to Human Resource > Maintain Branch…, select a Branch/Create a new one

   ![maintain-branch1](../../../../static/img/integration/hrms/e-tms/maintain-branch1.png)

2. Go to Map, enter the branch address, search and confirm

   ![maintain-branch2](../../../../static/img/integration/hrms/e-tms/maintain-branch2.png)

   :::tip
   User may click on the map to get a more accurate position
   :::

3. Enter the restriction radius and click save

   > by default min: 5m, max: 60m

   ![maintain-branch3](../../../../static/img/integration/hrms/e-tms/maintain-branch3.png)

## Maintain Public Holiday

1. Navigate to Leave > Maintain Public Holiday Calendar… and select a Public Holiday Calendar/Create New

    ![maintain-public-holiday1](../../../../static/img/integration/hrms/e-tms/maintain-public-holiday1.png)

2. Set public holidays

    > User may import default Malaysia public holiday calendar or set manually

    Option 1: Global Icon | Select a State | OK

        ![maintain-public-holiday2](../../../../static/img/integration/hrms/e-tms/maintain-public-holiday2.png)

    :::info
    User may check or uncheck the dates
    :::

    Option 2: Click on **_'P' button_** | Select date

        ![maintain-public-holiday3](../../../../static/img/integration/hrms/e-tms/maintain-public-holiday3.png)

3. Save

:::info
For more Public Holiday options, user may click on the **_'≣'_** on the grid to reveal the **_'Day Type'_** column

   ![maintain-public-holiday4](../../../../static/img/integration/hrms/e-tms/maintain-public-holiday4.png)

   - Public Holiday options:
     - Special Rate 1
     - Special Rate 2
:::

## Maintain Work Session

1. Navigate to Time Attendance > Maintain Work Session…, select a Work Session/Create New

   ![maintain-work-session](../../../../static/img/integration/hrms/e-tms/maintain-work-session.png)

2. Enter Work Start, Work End and Buffer

   > by default is 0 min

   - **_'Late In Buffer':_** Can be late by how many minutes
   - **_'Early Out Buffer':_** Can leave early by how many minutes

3. Enter Break Time

   - May add up to 3 break times

4. Select a Clock Method
   :::info

   - Only one clock method can be selected. However, if none of the clock method is selected, then the clock in / out button in SQL HRMS app will be disabled and employee does not require to clock in / out.
   - Clock Method on days without work session, public holiday and rest day is by default **GPS**.

   :::

   - **_'GPS' checkbox:_** Clock in / out using employee's location in SQL HRMS app
   - **_'QR' checkbox:_** Clock in / out using QR Code generated from SQL HRMS app and scan it on SQL Clock In app

5. Select Rules

   :::info
   **_'GPS Monitoring'_** and **_'Site Photo'_** will be disabled if **_'QR'_** or **_no clock method_** is selected
   :::

   - **_'GPS Monitoring' checkbox:_** Post status update if employee left work location
   - **_'Site Photo' checkbox:_** Requires to take photo before clock in / out (User cannot upload picture from album)

6. Save

### Optional

- User may select **_'Leave Rules'_** if applicable

:::info
Make sure that the work session is set based on the time zone maintained in Company Profile (refer to [timezone](#time-zone))
:::

## Maintain Work OT

1. Navigate to Time Attendance > Maintain Work OT…, select a Work OT/Create New

   ![maintain-work-ot1](../../../../static/img/integration/hrms/e-tms/maintain-work-ot1.png)

2. Click on **_'+' button_** | Select Day Type
3. Select OT Period
4. Select Work Session

   | **Day Type**                                                                                                    | **OT Period**                                 | **Work Session**        |
   | :-------------------------------------------------------------------------------------------------------------- | :-------------------------------------------- | :---------------------- |
   | Rest Day <br/> Rest Day (Special Rate 1 / 2 / 3) <br/> Public Holiday <br/> Public Holiday (Special Rate 1 / 2) | All Day                                       | 												 |                         
   | Work Day                                                                                                        | Before Work <br/> Break Time <br/> After Work | _Select a Work Session_ |

5. Set OT Rule by clicking on the **_'…' button_**

   **Standard Rule - Clock Time:**

   ![maintain-work-ot2](../../../../static/img/integration/hrms/e-tms/maintain-work-ot2.png)

   - **'Min OT':** Require to have at least 30 minutes of OT to be eligible for this rule
   - **'Max OT':** Maximum claimable OT minutes is 180 minutes (3 hours)
   - **'Allow AdHoc OT':** Any OT before 6:00pm will also be calculated

   | **Period** | **OT Start** | **OT** | **Explanation**                               |
   | :--------- | :----------- | :----- | :-------------------------------------------- |
   | 1          | 6:00pm       | ----   | 6:00pm - 7:00pm, Entitled to OT Code ----     |
   | 2          | 7:00pm       | HW15   | From 7:00pm onwards, Entitled to OT Code HW15 |

   **Explanation:** If employee start OT at 7:00pm, employee is entitled to OT Code HW15 and can claim up to 180 minutes

   **Standard Rule - Tier:**

   ![maintain-work-ot3](../../../../static/img/integration/hrms/e-tms/maintain-work-ot3.png)

   - **_'OT Start':_** Allow to start OT at 9:00am
   - **_'Min OT':_** Require to have at least 60 minutes of OT to be eligible for rule
   - **_'Allow AdHoc OT':_** Any OT before 9:00am will also be calculated

   | **Tier** | **Max OT** | **OT** | **Explanation**                             | **Example**      |
   | :------- | :--------- | :----- | :------------------------------------------ | :--------------- |
   | 1        | 120        | DR15   | First 120 minutes, Eligible to OT Code DR15 | 9:00am - 11:00am |
   | 2        | 240        | DR20   | Next 240 minutes, Eligible to OT Code DR20  | 11:00am - 3:00pm |
   | 3        | 240        | DR25   | Last 240 minutes, Eligible to OT Code DR25  | 3:00pm - 7:00pm  |

   :::info
   For Custom Rule, may contact SQL Support for customization
   :::

6. Save

## Maintain Calendar

1. Navigate to Time Attendance > Maintain Calendar…

   ![maintain-calendar](../../../../static/img/integration/hrms/e-tms/maintain-calendar.png)

### View Schedule

1. Click **_'View Schedule' button_**

   ![view-schedule](../../../../static/img/integration/hrms/e-tms/view-schedule.png)

**Work Session Calendar:**

- **Red box:** Public Holiday assigned from Maintain Public Holiday Calendar
- **Orange font:** Rest Day
- **Black font:** Work Day with Session
- **Grey font:** No schedule is assigned

**Set Work Session:**

- User may click on **_'R' button_** or **_'W' button_** and select date from calendar
- Use **_'C' button_** to clear Work Session/Rest Day
  - Alternatively, user may use **_'Clear All' button_** to clear all Rest Day and Work Session within the date range
- User cannot assign work sessions or change work sessions on dates before summary last processed date
- On days without work session assigned, no summary will be processed unless there are clock in/clock out logs on that day

### Wizard

1. Select Employee(s) and go to Wizard

   ![calendar-wizard1](../../../../static/img/integration/hrms/e-tms/calendar-wizard1.png)

   - **_'Delete & Replace Schedule' checkbox:_** Any previously assigned Work Session will be deleted and replace
     - Only apply to assigned work session on future dates
   - Hover **'Rest Day'** for more rest day options:
     - Special Rate 1
     - Special Rate 2
     - Special Rate 3

2. Select a schedule

   | **Schedule** | **Explanation**                                                             |
   | :----------- | :-------------------------------------------------------------------------- |
   | By Months    | Assign to every selected day of every selected week of every selected month |
   | Custom       | Assign to selected dates                                                    |

3. Next, select a Session

   ![calendar-wizard2](../../../../static/img/integration/hrms/e-tms/calendar-wizard2.png)

   - **_'Skip Rest Day' checkbox:_** Previously assigned Rest Day will not be replaced with Work Session
     - Only apply to assigned work session on future dates
   - **_'Delete & Replace Schedule' checkbox:_** Any previously assigned schedule will be deleted and replace
     - Only apply to assigned work session on future dates

4. Select schedule type

   | **Schedule**     | **Explanation**                                                             |
   | :--------------- | :-------------------------------------------------------------------------- |
   | By Months        | Assign to every selected day of every selected week of every selected month |
   | By Days of Month | Assign to every selected day of every selected month                        |
   | By Weeks         | Assign to every selected day of every selected weeks of the year            |
   | Custom           | Assign to selected dates                                                    |

5. Process

:::warning
User cannot assign work sessions or change work sessions on dates before summary last processed date
:::

### Copy Calendar from Employee

1. Select employee(s), click on the "Wizard" dropdown ▼, click "Copy From"
2. Select date range and employee to copy from and press "OK"

   ![copy-calendar](../../../../static/img/integration/hrms/e-tms/copy-calendar.png)

**Explanation:** Copy Employee 00005 schedule (Work Session and Rest Day) from 20/5/2024 to 31/12/2024 to Employee 00006

:::info
Date From need to be after summary last processed date to future dates (dates before summary last processed date are not allowed to copy)
:::

### Clear All Schedule

1. Select employee(s) click on the "Wizard" dropdown ▼, click "Clear All"
2. Select date range to delete and press "OK"

   ![clear-all-schedule](../../../../static/img/integration/hrms/e-tms/clear-all-schedule.png)

**Explanation:** Delete all schedule (Work Session and Rest Day) of Employee 00006 from 20/5/2024 to 31/12/2024

:::info
Date From need to be after summary last processed date to future dates (dates before summary last processed date are not allowed to delete)
:::

## Maintain Traveller Location

1. Navigate to Time Attendance > Maintain Traveller Location…

   ![maintain-traveller-location](../../../../static/img/integration/hrms/e-tms/maintain-traveller-location.png)

:::info
Only employees who is a **'Traveller'** will be listed (refer [Maintain Employee](#maintain-employee))
:::

### View Location

1. Click View Location

   ![view-location](../../../../static/img/integration/hrms/e-tms/view-location.png)

- **Red box:** Public Holiday assigned from Maintain Public Holiday Calendar
- **Orange font:** Rest Day
- **Black font:** Work Day with session
- **Grey font:** No schedule is assigned
- **Purple box:** Work locations allocated
- To clear a work location, focus a record on the grid and click **_'-' button_**
  - User may click on **_'Clear All' button_** to clear all work locations within the date range

### Wizard

1. Select Employee(s), and go to Wizard

    ![location-wizard1](../../../../static/img/integration/hrms/e-tms/location-wizard1.png)

2. Select a Schedule

    | **Schedule**     | **Explanation**                                                             |
    | :--------------- | :-------------------------------------------------------------------------- |
    | By Months        | Assign to every selected day of every selected week of every selected month |
    | By Days of Month | Assign to every selected day of every selected month                        |
    | By Weeks         | Assign to every selected day of every selected week of the year             |
    | Custom           | Assign to selected dates                                                    |

3. Click on **_'+' button_**  Map
4. Select a GPS Type | Enter radius (by default is 60m and min is 5m) and description | Confirm

    | **GPS Type** | **Explanation**                                           |
    | :----------- | :-------------------------------------------------------- |
    | Branch       | Select from a list of branches created in Maintain Branch |
    | Custom       | Search by address                                         |

    ![location-wizard2](../../../../static/img/integration/hrms/e-tms/location-wizard2.png)

    :::tip
    User may pin on the map to get a more accurate position
    :::

5. Process

    ![location-wizard3](../../../../static/img/integration/hrms/e-tms/location-wizard3.png)

### Copy Work Location from Employee

1. Select Employee(s), go to "Wizard" dropdown ▼, press "Copy From"
2. Select date range and employee to copy from and press "OK"

    ![copy-location](../../../../static/img/integration/hrms/e-tms/copy-location.png)

**Explanation:** Copy Employee 00012 locations from 20/5/2024 to 31/12/2024 to Employee 00007

:::info
Date From need to be current date to future dates (past dates are not allowed to copy)
:::

### Clear All Work Locations

1. Select Employee(s), go to "Wizard" dropdown ▼, press "Clear All"

    ![clear-all-location](../../../../static/img/integration/hrms/e-tms/clear-all-location.png)

2. Select Date Range and press "OK"
**Explanation:** Delete all locations of Employee 00007 from 20/5/2024 to 31/12/2024

:::info
Date From need to be current date to future dates (past dates are not allowed to delete)
:::

## Maintain Employee

1. Navigate to Human Resource > Maintain Employee…, select an Employee/Create New, next go to Personal tab and enter the email

    ![maintain-employee1](../../../../static/img/integration/hrms/e-tms/maintain-employee1.png)

2. In the Grouping, select a Branch
3. Select a Public Holiday Calendar
4. Select a Work OT
5. Save

    ![maintain-employee2](../../../../static/img/integration/hrms/e-tms/maintain-employee2.png)

:::info[Optional]

- Employees who are entitled to Attendance Reward, may select an **'Attendance Reward'**
- Employees who are travellers (Eg. Salesperson / Delivery Person / Doctor), may check the **_'Traveller' checkbox_**

:::

## Sync Cloud

1. Navigate to ☁️, go to "Sync Cloud…", click on "Sync All"

:::info
Make sure to always **'Sync Cloud'** after all maintenance are done or if there are any changes to the Time Attendance Setup to ensure settings on both Payroll and SQL HRMS app are in sync with one another
:::

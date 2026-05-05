---
sidebar_position: 3
title: Sync Cloud
description: An E TMS sync cloud guide in SQL Payroll
---

1. Click on the ☁️ > Sync Cloud… > Time Attendance, press "Sync All"

    ![sync-cloud1](../../../../static/img/integration/hrms/e-tms/sync-cloud1.png)

2. After all necessary adjustments are made, click "Update Payroll"

    - Alternatively, user may click on the **_'Update TMS' button_** under **_'Update Payroll' dropdown_** to only update TMS data to server
    - After **_'Update Payroll'_**, all OT / Leave trans that has been assigned action will no longer appear on the grid. User may view it under [Time Attendance Unassigned Listing report](payroll-report.md#time-attendance-unassigned-listing)

:::info
The **'ETMS updated to dd/mm/yyyy'** is the date of the latest TMS summary processed. Any attendance logs before the updated date will no longer allowed to be adjusted from SQL HRMS app.

The **Log synced to dd/mm/yyyy hh:nn** is the date time SQL Payroll will sync attendance log to. Any attendance logs before this time (due to manager clock on behalf) will no longer be synced to SQL Payroll

| **Scenario**             | **Sync Up To**   |
| :----------------------- | :--------------- |
| Before 9am on 24/09/2025 | 23/09/2025 23:59 |
| After 9am on 24/09/2025  | 24/09/2025 08:59 |

:::

## Attendance Log Error

This dialog box will only prompt if there are any incomplete log pairs (missing clock in / clock out) that requires attention

    ![log-error](../../../../static/img/integration/hrms/e-tms/log-error.png)

- The logs are grouped by the date and employee with alternating **green** and **white** highlights
- **Green cells:** Missing time which needs to be filled in
- Editable columns: 
  - Clock In 
  - Clock Out 
  - Is OT 
  - Break Time
- **_'Recalculate' button_** will enabled once changes are made to perform recalculation on the attendance logs
- **Batch Edit:** _Ctrl_ + select the rows you want to edit then right click and select _Batch Edit_
  - Note that you can only select records with missing clock in / clock out time and only either one at a time
  - Supported column: Clock In / Clock Out (depends on the type of record selected)
  
    ![log-error](../../../../static/img/integration/hrms/e-tms/batch-edit-error-log.png)
    
    - The date will automatically follow the record's date
    - If the time belongs to the next day, then you'll need to check the _'Overnight' checkbox_

      | **Selected Record Dates** |  **Overnight** | **Result**                               |
      | :------------------------ | :------------- | :--------------------------------------- |
      | 2/4/2025<br/>31/7/2025    | Not Checked    | 2/4/2025 06:00 PM<br/>31/7/2025 06:00 PM |
      | 3/4/2025                  | Checked        | 4/4/2025 06:00 PM                        |

## Log

This tab shows the processed TMS summary with employees' log details after processed

    ![log](../../../../static/img/integration/hrms/e-tms/log.png)

### Location Map

User can click on the **_'Map' button_** in tab to show the employee's log location (Clock In, Clock Out, Status Update) on a map

    ![location-map](../../../../static/img/integration/hrms/e-tms/location-map.png)

- Map icon identifier:

  | **Icon**                                                                  | **Description** |
  | :------------------------------------------------------------------------ | :-------------- |
  | ![map-icon1](../../../../static/img/integration/hrms/e-tms/map-icon1.png) | Clock In        |
  | ![map-icon2](../../../../static/img/integration/hrms/e-tms/map-icon2.png) | Status Update   |
  | ![map-icon3](../../../../static/img/integration/hrms/e-tms/map-icon3.png) | Clock Out       |

### Edit Mode

Right-click on the grid, select "Edit"

    ![log-edit-mode](../../../../static/img/integration/hrms/e-tms/log-edit-mode.png)

- The logs are grouped by the date and employee with alternating **green** and **white** highlights
- Editable columns: 
  - Clock In 
  - Clock Out 
  - Is OT 
  - Break Time
- **_'Recalculate' button_** will enabled once changes are made to perform recalculation on the attendance logs
- The **_'Work Duration'_** calculated after the log is adjusted is the difference between the **_'Adjusted Clock Out'_** and **_'Adjusted Clock In'_**
  - An accurate **_'Work Duration'_** will be calculated after the **_'Recalculate' button_** is clicked
- **Batch Edit:** _Ctrl_ + select the rows you want to edit then right click and select _Batch Edit_
  - Supported columns:
    - Is OT
    - Break Time

## OT

    ![ot](../../../../static/img/integration/hrms/e-tms/ot.png)

- Editable columns:
  - Post Date
  - Remark
  - Break Time
  - Claimable
  - Action:
    - Unassigned
    - Overtime: Record will be posted to Pending Overtime
    - Cancelled: Record will be ignored
  - OT Code
- **_'Show Log' button_** is to show all employee's attendance logs on that date
- **Batch Edit:** _Ctrl_ + select the rows you want to edit then right click and select _Batch Edit_
  - Supported columns:
    - Post Date
    - Remark
    - Break Time
    - Claimable
    - Action
    - OT Code

## Leave

    ![leave](../../../../static/img/integration/hrms/e-tms/leave.png)

- Editable columns:
  - Post Date
  - Remark
  - Deductible
  - Action:
    - Unassigned
    - Leave: Records will be posted to Leave Application
    - Unpaid Leave: Record will be posted to Leave Application
    - Cancelled: Record will be ignored
  - Leave Type: Value changes based on chosen action
- User need to assign a leave code in order to post it to Leave Application
- **_'Show Log' button:_** Show all employee's logs on that date
- **Batch Edit:** _Ctrl_ + select the rows you want to edit then right click and select _Batch Edit_
  - Supported columns:
    - Post Date
    - Remark
    - Deductible
    - Action

## Generate Calendar Reminder

    ![generate-calendar-reminder](../../../../static/img/integration/hrms/e-tms/generate-calendar-reminder.png)

- A generate calendar reminder for next year will be prompted starting from **October** each year
- The reminder will be prompt on condition where there is work session assigned on current year
- Options:
  - **Go To Calendar:** User will be directed to [Maintain Calendar](payroll-setup/#maintain-calendar)
  - **Generate Work Schedule without Session:** System will generate a whole year of work days without session
  - **Later:** Nothing will happen and the reminder will prompt again the next time user Sync Cloud

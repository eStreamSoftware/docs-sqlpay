---
sidebar_position: 3
title: App Usage
description: An E TMS features in SQL HRMS app guide
---

:::info
Enable **Autostart** for SQL HRMS to ensure E TMS features work accordingly (refer [Autostart](../autostart.md))
:::

## Dashboard

    ![dashboard](../../../../static/img/integration/hrms/e-tms/dashboard.png)

- **Session Card:** User's work session shift time
  - Icon on the top right corner (green box) indicates the clock method (by GPS or QR) of the day. If there is no icon displayed, it means that user is not required to clock for that day
	- Tap on the icon to navigate to [Work Session Calendar](#work-session-calendar)
  - It shows user's first Clock In and last Clock Out of the day with an estimated calculation of late in and early out
  - User can tap on the card to direct to User's Attendance Log
  - User can tap on the **_'Clock In / Out' button_** to direct to Clock In / Clock Out page
    - If no work session is assigned or no clock method is selected, the button will be disabled
- **Upcoming Holiday:** User's upcoming public holidays

## Clock In / Clock Out

### By GPS

| **Button**                                                                        | **Explanation**                                                                                                                                                                                                                                                                        |
| :-------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![clock-button1](../../../../static/img/integration/hrms/e-tms/clock-button1.png) | SQL HRMS app's Location service is unable to start. This may due to the following reasons: <br/><br/> 1. User's location service is not enabled <br/> 2. The required location permission is not allowed <br/><br/> Refer [Location Service and Permission](../permission.md#location) |
| ![clock-button2](../../../../static/img/integration/hrms/e-tms/clock-button2.png) | SQL HRMS app is trying to get user's current location                                                                                                                                                                                                                                  |
| ![clock-button3](../../../../static/img/integration/hrms/e-tms/clock-button3.png) | User is not within work location. However, if user is really within their work location, SQL HRMS app will continuously try to get a more accurate position so that user will be able to Clock In / Clock Out                                                                          |
| ![clock-button4](../../../../static/img/integration/hrms/e-tms/clock-button4.png) | User's location is mocked and is not allowed to Clock In / Out                                                                                                                                                                                                                         |
| ![clock-button5](../../../../static/img/integration/hrms/e-tms/clock-button5.png) | User is within work location and is allowed to Clock In                                                                                                                                                                                                                                |
| ![clock-button6](../../../../static/img/integration/hrms/e-tms/clock-button6.png) | User is within work location and is allowed to Clock Out                                                                                                                                                                                                                               |

**Clock In:**

    ![clock-in1](../../../../static/img/integration/hrms/e-tms/clock-in1.png)

    - User who is a traveller will show a **'Traveller'** with green check

:::info
If user forget to clock out, the app will reset the time tracking after 10 hours (600 mins) after Session Work End time and last Clock In time
    ![clock-in2](../../../../static/img/integration/hrms/e-tms/clock-in2.png)

:::

**Clock Out:**

    ![clock-out1](../../../../static/img/integration/hrms/e-tms/clock-out1.png)

    - If **_'Claim OT' switch_** is turned on - The **'OT Break Time (min)'** will be visible

  	![clock-out2](../../../../static/img/integration/hrms/e-tms/clock-out2.png)

    - **_'Claim As Leave' switch_** will only be visible on Rest Day and Public Holiday
    - If **_'Claim As Leave' switch_** is turned on
        - An earn replacement leave application will be posted when employee clocked out
        - When employee tap the **_'Clock Out' button_**, a **'Claim As Leave'** dialog will be prompt that allows the employee to pick the leave type that they want to claim

  ![clock-out3](../../../../static/img/integration/hrms/e-tms/clock-out3.png)

### By QR

| **Button**                                                                        | **Explanation**                                                                                                                                                                                                                                                                                                              |
| :-------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![clock-button7](../../../../static/img/integration/hrms/e-tms/clock-button7.png) | SQL HRMS app's Bluetooth service is unable to start. This may due to the following reasons: <br/><br/> 1. User's Bluetooth service is not enabled <br/> 2. The required nearby devices permission is not allowed <br/><br/> Refer [Bluetooth Service and Nearby Devices Permission](../permission#nearby-devices--bluetooth) |
| ![clock-button5](../../../../static/img/integration/hrms/e-tms/clock-button5.png) | User is allowed to Clock In                                                                                                                                                                                                                                                                                                  |
| ![clock-button6](../../../../static/img/integration/hrms/e-tms/clock-button6.png) | User is allowed to Clock Out                                                                                                                                                                                                                                                                                                 |

**Clock In:**

    ![clock-in3](../../../../static/img/integration/hrms/e-tms/clock-in3.png)

    - **'Attachments'** field will not be available
    - Proceed to Clock In will generate a QR Code that will be scanned by SQL Clock In app
      - User can adjust the brightness of the screen with the slider
      - The QR Code will only be valid for 20s before user will need to regenerate a new QR Code

**Clock Out:**

    ![clock-out4](../../../../static/img/integration/hrms/e-tms/clock-out4.png)

    - If **_'Claim OT' switch_** is turned on, it will go through similar OT validations as _By GPS_ before QR Code is generated

:::warning
Screenshotting the QR Code is not allowed!
:::

### Work Location

1. Tap on the **_'View Work Location' label button_**

    ![work-location](../../../../static/img/integration/hrms/e-tms/work-location.png)

    - 👤: Employee's current location
    - ✅: Location that the employee is currently in

:::info
Multiple work locations with the same coordinate will be considered as one
:::

## Work Session Calendar

### My Work Session

User can view his own work session in calendar view

    ![my-work-session](../../../../static/img/integration/hrms/e-tms/my-work-session.png)

- **Red font with purple box:** Public Holiday
- **Purple box:** Rest Day
- **Icon (bottom right corner):** Clock Method
- **Whole card:** Direct to [Work Location](#work-location) page to view locations where the user is allowed to clock in / clock out on that day

### Team Work Session

User can view employee's team member's work session and work session of the employees that the manager is managing

    ![team-work-session](../../../../static/img/integration/hrms/e-tms/team-work-session.png)

## Log

### Processed Log

    ![processed-log1](../../../../static/img/integration/hrms/e-tms/processed-log1.png)

- The bar chart shows employee summary of a week
  - **Blue bar (480 minutes):** Employee fulfilled expected work duration
  - **Purple bar (397 minutes):** Employee did not fulfill expected work duration
- On Behalf indicates the log is clock by whom
  - **Admin:** Log filled in from SQL Payroll
  - **Manager:** Manager clock on behalf through SQL HRMS app
  - **'-' symbol:** Employee clock by themselves through SQL HRMS app
- Tap on the bar or date to view the summary and attendance logs
- **_'Leave Status' button_** is to view all leave applications applied on that date

  ![processed-log2](../../../../static/img/integration/hrms/e-tms/processed-log2.png)

- **_'Timeline' button_** will direct to Attendance Timeline to view user's locations (refer [Timeline](#timeline) for more details)

  ![processed-log3](../../../../static/img/integration/hrms/e-tms/processed-log3.png)

### Unprocessed Log

    ![unprocessed-log](../../../../static/img/integration/hrms/e-tms/unprocessed-log.png)

- Rough calculation on late in, early out and overtime will be calculated on those log that are not synced and processed in SQL Payroll
- User are encouraged to process the logs on SQL Payroll in order to obtain a more accurate results on late in, early out and overtime

## Timeline

    ![timeline](../../../../static/img/integration/hrms/e-tms/timeline.png)

- **Employee List** will only be visible to managers, employees will be directed into their own timeline
- Timeline plots the user's clock in, clock out and status update locations on a map
- User can view the remark and attachments of each log if available
  - Paper Clip icon will only appear if there's attachment for that log
  - If there are more than one attachment attached, tapping on the Paper Clip icon a pop up will appear with a list of attachments
- User can tap on each log card to focus on the log's location in the map
- Icon identifiers:

  |               | **Log Icon**                                                              | **Map Icon**                                                              |
  | :------------ | :------------------------------------------------------------------------ | :------------------------------------------------------------------------ |
  | Clock In      | ![log-icon1](../../../../static/img/integration/hrms/e-tms/log-icon1.png) | ![map-icon1](../../../../static/img/integration/hrms/e-tms/map-icon1.png) |
  | Status Update | ![log-icon2](../../../../static/img/integration/hrms/e-tms/log-icon2.png) | ![map-icon2](../../../../static/img/integration/hrms/e-tms/map-icon2.png) |
  | Clock Out     | ![log-icon3](../../../../static/img/integration/hrms/e-tms/log-icon3.png) | ![map-icon3](../../../../static/img/integration/hrms/e-tms/map-icon3.png) |

## Work OT

Shows the employee's OT entitlement

    ![work-ot](../../../../static/img/integration/hrms/e-tms/work-ot.png)

## Team Log

### My Summary

    ![my-summary](../../../../static/img/integration/hrms/e-tms/my-summary.png)

- User can view his own time attendance summary
- User can tap on the card to direct to [**Attendance Log**](#log) to view detailed summary

### Team Summary

    ![team-summary](../../../../static/img/integration/hrms/e-tms/team-summary.png)

- User can view his team member's time attendance summary
- **Only manager that is managing that employee** can tap on the card to direct to [**Attendance Log**](#log) for more detailed summary
- **_'Clock on Behalf' button_** will be visible only to manager on current date and previous dates where time attendance summaries have not been process
- Filtering chips can be used to filter the summary:
  - Late In
  - Early Out
  - Absence
  - No Out
  - OT
  - Leave

### Clock On Behalf (Manager only)

Managers are allowed to clock in on behalf for his team by tapping on the **_'Clock on Behalf' button_**

    ![clock-on-behalf1](../../../../static/img/integration/hrms/e-tms/clock-on-behalf1.png)

- After choosing an employee, the manager is directed to the [**Attendance Log**](#log) where a Right Arrow icon on each log and a **_'Clock In' button_** is visible
- Tap on the Right Arrow icon to direct to Attendance Log Detail

- **Clock On Behalf**

  ![clock-on-behalf2](../../../../static/img/integration/hrms/e-tms/clock-on-behalf2.png)

| **Button**                                                                        | **Explanation**                                                                                                                                                                                                                                                                  |
| :-------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![clock-button1](../../../../static/img/integration/hrms/e-tms/clock-button1.png) | SQL HRMS app's location service is unable to start. This may due to the following reasons: <br/><br/> 1. User's device GPS is not enabled <br/> 2. The required location permission is not allowed <br/><br/> Refer [Location Service and Permission](../permission.md#location) |
| ![clock-button2](../../../../static/img/integration/hrms/e-tms/clock-button2.png) | SQL HRMS app is trying to get user's current location                                                                                                                                                                                                                            |
| ![clock-button4](../../../../static/img/integration/hrms/e-tms/clock-button4.png) | User's location is mocked and is not allowed to Clock In / Out                                                                                                                                                                                                                   |
| ![clock-button5](../../../../static/img/integration/hrms/e-tms/clock-button5.png) | User's location is detected and is allowed to Clock In                                                                                                                                                                                                                           |
| ![clock-button6](../../../../static/img/integration/hrms/e-tms/clock-button6.png) | User's location is detected and is allowed to Clock Out                                                                                                                                                                                                                          |

- Manager's location will be captured when help to clock on behalf
- Manager can adjust the employee's clocking time and checked **_'Claim OT'_** or **_'Claim As Leave'_** if needed
- Manager are not allowed to clock out on behalf if employee already clocked out on the next day
- Manager are not allowed to clock on behalf earlier than the stated last processed date and time
- **View Attendance Log Detail (Right Arrow Icon)**

    ![attendance-log-detail](../../../../static/img/integration/hrms/e-tms/attendance-log-detail.png)

- A **_Pencil icon_** will be visible next to the time if the log is allowed to be adjusted
- Any date and time earlier than the stated last processed date and time cannot be adjusted

## Notification

### Geofence Service

The notification will appear after employee clocked in and has **_'GPS Monitoring'_** enable for their [Work Session](payroll-setup.md#maintain-work-session)

    ![geofence-service](../../../../static/img/integration/hrms/e-tms/geofence-service.png)

### Clock In/Out Reminder

1. Remind user to clock in when he is within work location

   ![reminder1](../../../../static/img/integration/hrms/e-tms/reminder1.png)

2. Remind employee to clock out it's work end

   ![reminder2](../../../../static/img/integration/hrms/e-tms/reminder2.png)

### Status Update

- Managers will receive their managing employees' status update
- Types of status update:

  - Location service off

    ![status-update-notification1](../../../../static/img/integration/hrms/e-tms/status-update-notification1.png)

  - Employee outside work location

    ![status-update-notification2](../../../../static/img/integration/hrms/e-tms/status-update-notification2.png)

  - Mock/Fake location

    ![status-update-notification3](../../../../static/img/integration/hrms/e-tms/status-update-notification3.png)

### Clock On Behalf

- The manager themselves and other managers managing the same employee will receive the following notifications once they clock on behalf for an employee

  - App Notification

        ![clock-on-behalf-notification1](../../../../static/img/integration/hrms/e-tms/clock-on-behalf-notification1.png)

  - Email Notification

        ![clock-on-behalf-notification2](../../../../static/img/integration/hrms/e-tms/clock-on-behalf-notification2.png)

- The employee will receive the following notifications once their manager clock on behalf for them

  - App Notification

        ![clock-on-behalf-notification3](../../../../static/img/integration/hrms/e-tms/clock-on-behalf-notification3.png)

  - Email Notification

        ![clock-on-behalf-notification4](../../../../static/img/integration/hrms/e-tms/clock-on-behalf-notification4.png)

### Adjusted Attendance Log

- The manager themselves and other managers managing the same employee will receive the following notifications once they adjusted an employee's attendance log

  - App Notification

        ![adjusted-log-notification1](../../../../static/img/integration/hrms/e-tms/adjusted-log-notification1.png)

  - Email Notification

        ![adjusted-log-notification2](../../../../static/img/integration/hrms/e-tms/adjusted-log-notification2.png)

- The employee will receive the following notifications once their manager adjusted their attendance log

  - App Notification

        ![adjusted-log-notification3](../../../../static/img/integration/hrms/e-tms/adjusted-log-notification3.png)

  - Email Notification

        ![adjusted-log-notification4](../../../../static/img/integration/hrms/e-tms/adjusted-log-notification4.png)

### Employee login from a different device

- Managers will receive an email notification when his team use a different device to login to the app
- The purpose is to help manager keep track if there are any employees that might help their friends to clock in/out
  ![different-device-notification](../../../../static/img/integration/hrms/e-tms/different-device-notification.png)

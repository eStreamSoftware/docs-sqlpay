---
title: Guide
sidebar_position: 1
description: A guide of leave for SQL Payroll
slug: /usage/leave/guide
tags: ["SQL Payroll", "Leave", "Report"]
---

## Introduction

The Leave module is used to monitor employee leave, manage the company calendar, and print attendance reports. It consists of four sections:

1. **Maintenance**
2. **Leave Entitlement Processor**
3. **Leave Application**
4. **Reports**

## Leave Application

- **Records leave applied for by each employee. You can input any type of leave defined in Maintain Leave Type.**
- **You can assign a calendar to individual employees in Maintain Employee. This will load the employee's leave application.**
- It monitors leave applications based on the up-to-date leave entitlement.

    For example:

    1. **Annual Leave Entitlement = 12 days**
    2. **Average Annual Leave Entitlement = 1 day per month**
    3. **Annual Leave applied for a month:**
        - **January = 0 days**
        - **February = 1 day**
        - **March = 0 days**

    In this scenario, the total annual leave entitled up to April is 4 days (including April).

    This means the remaining annual leave is (4 – 1) = 3 days.

    If the employee applies for 4 days of leave in April, the system will prompt the warning: “You’ve taken 5.0 days of Annual Leave, but Annual Leave limit for April is 4.0 days.”

    You can then choose to Allow, Not Allow, or treat it as Unpaid Leave.
    :::

1. Navigate to **Leave** > **Leave Application**.

    ![leave-application](../../../static/img/usage/leave-module/leave-application.png)

2. Select the year (e.g., 2015).

    ![leave-application-year](../../../static/img/usage/leave-module/leave-application-year.png)

3. Select the employee (e.g., Lee Chong Wai).

    ![leave-application-employee](../../../static/img/usage/leave-module/leave-application-employee.png)

4. Click the **+** button. A row will appear where you can select the date, leave type, and number of days applied. Click **Save** once completed.

    ![leave-application-date](../../../static/img/usage/leave-module/leave-application-date.png)
    ![leave-application-save](../../../static/img/usage/leave-module/leave-application-save.png)

5. If the employee applies for half-day leave or hourly leave, use the **Day As Time** column (1 working day = 8 working hours).

    ![leave-application-halfday](../../../static/img/usage/leave-module/leave-application-halfday.png)

6. Enter the duration (e.g., 3 hours). The system will automatically calculate the number of days (e.g., 0.38 days).

    ![leave-application-hours](../../../static/img/usage/leave-module/leave-application-hours.png)

### Hourly Leave Application

1. Go to **Leave** > **Leave Application** > **New Leave Application**.

    ![hour-leave-new](../../../static/img/usage/leave-module/hour-leave-new.png)

2. Select the employee's name, then click **Apply Leave**.

    ![hour-leave-select-employee](../../../static/img/usage/leave-module/hour-leave-select-employee.png)

3. Enable the **Day As Time** column.

    ![hour-leave-day-as-time](../../../static/img/usage/leave-module/hour-leave-day-as-time.png)

4. Select the leave type and date.

    - The **Day** column represents the number of days, while the **Day As Time** column represents the hours.
      :::tip Example:
      - Day = 1.00 (1 day of leave)
      - Day As Time = 8.00 (HH:MM, 8 hours in 1 day)
      :::

    ![hour-leave-select-type](../../../static/img/usage/leave-module/hour-leave-select-type.png)

5. Apply Hourly Leave.

    - If a staff member wants to apply for 2 hours of Annual Leave, enter `02:00` in the **Day As Time** column and press **Enter**.

    - The **Day** column will automatically update to `0.25`.

    ![hour-leave-apply](../../../static/img/usage/leave-module/hour-leave-apply.png)

6. Save.

    - Click the **Save** icon. The save is complete when the icon turns grey.

    ![hour-leave-save](../../../static/img/usage/leave-module/hour-leave-save.png)

7. This method can be used for all leave types.

## Leave Entitlement Processor

**It processes annual leave entitlement for each employee based on their leave group.**

1. The leave entitlement process is typically performed once a year. Navigate to **Leave** > **Leave Entitlement Processor**.

    ![leave-entitlement-processor](../../../static/img/usage/leave-module/leave-entitlement-processor.png)

2. Select the Transaction Posting Year (e.g., 2015) and click **Process**.

    ![leave-entitlement-processor-process](../../../static/img/usage/leave-module/leave-entitlement-processor-process.png)

3. A table will display the leave entitlement for each employee for the selected year.

    ![leave-entitlement-processor-details](../../../static/img/usage/leave-module/leave-entitlement-processor-details.png)

4. You can edit the number of days if necessary. Click **Save** when finished.

    ![leave-entitlement-processor-save](../../../static/img/usage/leave-module/leave-entitlement-processor-save.png)

## Maintain Public Holiday Calendar

**Step 1:** Go to **Leave** > **Maintain Public Holiday Calendar...**. Select a calendar or create a new one.

    ![maintain-public-holiday1](../../../static/img/integration/hrms/e-tms/maintain-public-holiday1.png)

**Step 2: Set public holidays**
You can import the default Malaysia public holiday calendar or set it manually.

Option 1: Click the **Global** icon, select a state, and click **OK**.

    ![maintain-public-holiday2](../../../static/img/integration/hrms/e-tms/maintain-public-holiday2.png)

:::info
You can check or uncheck specific dates.
:::

Option 2: Click the **'P'** button and select a date.
![maintain-public-holiday3](../../../static/img/integration/hrms/e-tms/maintain-public-holiday3.png)

**Step 3:** Click **Save**.

## Maintain Leave Type

**Maintain Leave Type** defines the types of leave, such as annual leave, medical leave, maternity leave, unpaid leave, etc. You can also configure settings such as:

- Is Entitled
- Is Unpaid
- Brought Forward

:::info
Before assigning a leave group to an employee, ensure that Leave Types and Leave Groups are maintained. **Leave Type** defines the nature of the leave, while **Leave Group** groups employees according to their leave entitlement.
:::

1. Navigate to **Leave** > **Maintain Leave Type**.

    ![maintain-leave-type](../../../static/img/usage/leave-module/maintain-leave-type.png)

2. Click the **New** button in the top right corner to create a new leave type.

    ![maintain-leave-type-new](../../../static/img/usage/leave-module/maintain-leave-type-new.png)

3. Assign a code for the leave type.

    :::tip Example
    `MaL` for Maternity Leave:

    - Check the relevant pay entitlement.
    - Click **Save**.
      :::

    ![maintain-leave-type-save](../../../static/img/usage/leave-module/maintain-leave-type-save.png)

4. The new leave type is created.

    ![maintain-leave-type-result](../../../static/img/usage/leave-module/maintain-leave-type-result.png)

### Brought Forward Leave

Ensure **Brought Forward (BF)** is checked in **Maintain Leave Type**.

1. Go to **Leave** > **Maintain Leave Type**
    ![maintain-leave-type](../../../static/img/usage/leave-module/maintain-leave-type.png)

    ![enable-bf-leave-2](../../../static/img/usage/leave-module/enable-bf-leave-2.png)

    Ensure there is a calculation for the amount of leave brought forward in **Maintain Leave Group**.

2. Go to **Leave** > **Maintain Leave Group**
    ![maintain-leave-group](../../../static/img/usage/leave-module/maintain-leave-group.png)

3. Make sure the BF column is ticked
    ![bf-leave-calculation-1](../../../static/img/usage/leave-module/bf-leave-calculation-1.png)

4. Click **Edit**
    ![bf-leave-calculation-2](../../../static/img/usage/leave-module/bf-leave-calculation-2.png)

5. Click the **tree-dot icon** to set the Leave B/F rule
    ![bf-leave-calculation-3](../../../static/img/usage/leave-module/bf-leave-calculation-3.png)

    At here, you can choose to use:
    - Standard Calculation, or
    - Custom Calculation (script customization)

    ![bf-leave-calculation-4](../../../static/img/usage/leave-module/bf-leave-calculation-4.png)

    <details>
    <summary>Standard vs Custom Calculation</summary>

    **Standard Calculation**

    An easy-to-use interface that allows users to configure BF Leave, including setting a fixed
    maximum number of carry-forward days and defining a special expiry date by which the BF
    leave must be utilized.

    1. Tick this option and set the maximum days allowed carry forward to the next year. 
        ![bf-leave-calculation-5](../../../static/img/usage/leave-module/bf-leave-calculation-5.png)
        > Tips: If you do not have the BF limit, you may ignore this step.

    2. Tick the option to set the expiry date, and select the Month and Day
        ![bf-leave-calculation-6](../../../static/img/usage/leave-module/bf-leave-calculation-6.png)
        BF Leave balance will be considered forfeit at the next day of the expiry date.
        For this sample : Leave Expiry Date - 31/03, Leave Forfeit - 01/04
        > Tips: If you do not have Bring Forward leave with an expiry date, you may ignore this step.

    **Custom Calculation**

    Extensive BF leave calculation logic is implemented through scripting and is generally
    developed by a programmer.

    1. Select this calculation method, and click the dropdown icon to load in the script
        ![bf-leave-calculation-7](../../../static/img/usage/leave-module/bf-leave-calculation-7.png)

    </details>

### Process B/F Leave & Forfeit

1. Go to leave entitlement (refer to [Leave Entitlement Processor](#leave-entitlement-processor)).
    ![bf-leave-entitlement-process-1](../../../static/img/usage/leave-module/bf-leave-entitlement-process-1.png)

2. Select the Leave Year, and click **Process**
    ![bf-leave-entitlement-process-2](../../../static/img/usage/leave-module/bf-leave-entitlement-process-2.png)

3. Click **Open** when showing this message
    ![bf-leave-entitlement-process-3](../../../static/img/usage/leave-module/bf-leave-entitlement-process-3.png)

4. Leave BF involves 3 columns: BF Ori, BF Forfeit, and BF
    - **BF Ori**: Original brought-forward leave from last year
    - **BF Forfeit**: Unused B/F leave forfeited after expiry
    - **BF**: Remaining B/F balance after forfeiture

    ![bf-leave-entitlement-process-4](../../../static/img/usage/leave-module/bf-leave-entitlement-process-4.png)

5. **Right click** and choose **Select All**, or use **Ctrl+A** to select all employees
    ![bf-leave-entitlement-process-5](../../../static/img/usage/leave-module/bf-leave-entitlement-process-5.png)

6. Click **Calculate Forfeited BF**
    ![bf-leave-entitlement-process-6](../../../static/img/usage/leave-module/bf-leave-entitlement-process-6.png)

7. A notification will prompt out and update the Leave B/F Forfeit until the latest expiry date
    :::info Changes will only take effect once the leave expiry date is reached.
        Example: if the Leave Expiry Date is 31/3 and the current computer date is 26 Jan, no any Leave will be forfeited
    :::
    ![bf-leave-entitlement-process-7](../../../static/img/usage/leave-module/bf-leave-entitlement-process-7.png)

8. Click **Yes** to continue
    ![bf-leave-entitlement-process-8](../../../static/img/usage/leave-module/bf-leave-entitlement-process-8.png)

9. System will auto recalculate the **BF Leave Forfeit**
    :::note
    Only unused B/F leave will be forfeited after the expiry date
    :::
    ![bf-leave-entitlement-process-9](../../../static/img/usage/leave-module/bf-leave-entitlement-process-9.png)

10. Click **Save** once done
    ![bf-leave-entitlement-process-10](../../../static/img/usage/leave-module/bf-leave-entitlement-process-10.png)

## Maintain Leave Group

:::info Features

- Allows you to customize leave policies for different employee levels.
- You can customize scripts (under **Tools** > **Maintain Script**) and apply them to the leave group.

:::

1. Navigate to **Leave** > **Maintain Leave Group**.

    ![maintain-leave-group](../../../static/img/usage/leave-module/maintain-leave-group.png)

2. Click the **New** button in the top right corner.

    ![maintain-leave-group-new](../../../static/img/usage/leave-module/maintain-leave-group-new.png)

3. Assign a code for the new leave group.

    :::tip Example
    `FW` for Foreign Worker.

    Click the **+** button to select the entitled leave types for this group.
    :::

    ![maintain-leave-group-code](../../../static/img/usage/leave-module/maintain-leave-group-code.png)

4. Taking **Annual Leave (AL)** as an example:

    - By default, the calculation for Annual Leave is:

    | Year of Service (Years) | Day of Leave Entitled (Days) |
    | ----------------------- | ---------------------------- |
    | 1 to 2                  | 8                            |
    | 3 to 4                  | 12                           |
    | >4                      | 16                           |

    ![maintain-leave-default-al](../../../static/img/usage/leave-module/maintain-leave-default-al.png)

    If your company follows this default policy, go to the **Entitle** tab and select **Annual Leave Entitlement Policy**. The calculation will follow the default setting.

    ![maintain-leave-group-policy](../../../static/img/usage/leave-module/maintain-leave-group-policy.png)

    Click **Save**.

5. If your company uses a different policy, click **Edit**, then click the **...** button beside the **Entitle** column to customize the calculation.

    ![maintain-leave-group-entitle](../../../static/img/usage/leave-module/maintain-leave-group-entitle.png)

6. For example, if your company uses the following calculation:

    | Year of Service (Years) | Day of Leave Entitled (Days) |
    | ----------------------- | ---------------------------- |
    | 1 to 2                  | 8                            |
    | 3 to 5                  | 12                           |
    | >5                      | 18                           |

    Enter the table as follows:

    | Year From | Year To | Days |
    | --------- | ------- | ---- |
    | 1         | 2       | 8    |
    | 3         | 5       | 12   |
    | 1         | 99      | 18   |

    ![maintain-leave-group-entitilement-new](../../../static/img/usage/leave-module/maintain-leave-group-entitilement-new.png)

7. Click **OK** to finish. 🥳

### Employee Leave Group Assignment

1. Navigate to **Human Resource** > **Maintain Employee**.

    ![employee-leave-group](../../../static/img/usage/leave-module/employee-leave-group.png)

2. Select the relevant employee (e.g., Nicole) and click **Edit**.

    ![employee-leave-group-edit](../../../static/img/usage/leave-module/employee-leave-group-edit.png)

3. Click the **Grouping** tab. You will see **Leave Group** in the last panel.

    ![employee-leave-group-grouping](../../../static/img/usage/leave-module/employee-leave-group-grouping.png)

4. Assign the relevant leave group.

    :::tip Example
    Foreign Worker (FW).
    Click **Save**.
    :::

    ![employee-leave-group-assign](../../../static/img/usage/leave-module/employee-leave-group-assign.png)
    ![employee-leave-group-save](../../../static/img/usage/leave-module/employee-leave-group-save.png)

## Leave Report

| Report                   | Description                                                                                                |
| ------------------------ | ---------------------------------------------------------------------------------------------------------- |
| Leave Application Report | Generates detailed leave taken by each employee for a year.                                                |
| Attendance Report        | Generates attendance performance in percentage.                                                            |
| Leave Balance Report     | Analyzes the number of days taken for annual leave, medical leave, etc.                                    |
| Yearly Leave Report      | Generates a 12-month summary of total leave taken for each leave type (e.g., annual leave, unpaid leave).  |

### Print Leave Application Report

![print-leave-application-report](../../../static/img/usage/leave-module/print-leave-application-report.png)

### Print Attendance Report

![print-attendance-report](../../../static/img/usage/leave-module/print-attendance-report.png)

### Print Leave Balance Report

![print-leave-balance-report](../../../static/img/usage/leave-module/print-leave-balance-report.png)

### Print Yearly Leave Report

![print-yearly-leave-report](../../../static/img/usage/leave-module/print-yearly-leave-report.png)

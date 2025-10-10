---
sidebar_position: 1
title: Setup
description: A setup for payroll maintenance
slug: /usage/payroll/setup
tags: ["SQL Payroll", "Setup"]
---

## Maintain Allowance

:::info Features

- Setting up maintain allowance helps you to categorize the type of allowance that employee entitle.
- This would affect the types of contribution that they need to provide (EPF/SOCSO/PCB & etc)
- This is especially useful if you have different types of allowance like Petrol, Handphone, Meal Allowance base on different company different entitlement.

:::

1. Navigate to **Payroll** > **Maintenance** > **Maintain Allowance**

   ![navigate](../../../static/img/usage/payroll/maintenance/maintain-allowance/navigate.png)

2. Click New to generate a New Allowance

   ![new](../../../static/img/usage/payroll/maintenance/maintain-allowance/new.png)

3. Insert the info that you want to set in maintain allowance

   ![insert](../../../static/img/usage/payroll/maintenance/maintain-allowance/insert.png)

   1. Insert the Code of the Allowance that you want to generate.
   2. Insert the Description of the allowance.
   3. Insert the fixed amount for the allowance, eg: Handphone allowance is fixed RM 300 for every employee then you can insert the rate of RM 300 but if there is not then you can left it blank.
   4. If the allowance is tax exempted then you may insert the tax exempted code.
   5. Tick or un-tick the contribution of the allowance.

4. After create the master file of Allowance, then you can add the fixed allowance for certain employee which have the allowance monthly

   ![add-fixed-allowance](../../../static/img/usage/payroll/maintenance/maintain-allowance/add-fixed-allowance.png)

5. Alternatively, you can insert the allowance after process month end.

   ![process-month-end-add-allowance](../../../static/img/usage/payroll/maintenance/maintain-allowance/process-month-end-add-allowance.png)

   1. Click on the "**Overtime**"
   2. CLick on the ➕ to add the employee then fill in the overtime

6. Allowance feature is same with deduction feature, all the allowance is not compulsory just depend on company policy.

## Maintain Claim

:::info Feature

- Maintain Claim is used to define the types of claims available to employees, as well as set default amounts and limits.
- For example, for travel claims, accommodation expenses, and communication expenses, you can set monthly or per-claim limits, set fixed amounts, or leave them blank for employees to fill in.
- This can impact the reimbursement process, monthly reimbursement review, and payroll calculations.

:::

1. Navigate to **Payroll** > **Maintenance** > **Maintain claim**

    ![navigate](../../../static/img/usage/payroll/maintenance/maintain-claim/navigate.png)

2. Click New to generate a New Claim

    ![new](../../../static/img/usage/payroll/maintenance/maintain-claim/new.png)

3. Insert the info that you want to set in maintain claim

    ![insert](../../../static/img/usage/payroll/maintenance/maintain-claim/insert.png)
    
    1. Insert the Code of the Claim that you want to generate.
    2. Insert the Description of the claim.
    3. Insert the Yearly Limit for the claim, eg: RM 2000 for every employee then you can insert the rate of RM 2000 but if there is no limit then you can left it blank as Unlimited by click the 'Set as Unlimited' button.
    4. Insert the Monthly Limit for the claim, eg: RM 200 for every employee then you can insert the rate of RM 200 but if there is no limit then you can left it blank as Unlimited by click the 'Set as Unlimited' button.

4. After create the master file of Claim, then you can add the fixed claim's Yearly Limit and Monthly Limit for certain employee which have the claim.

    ![add-fixed-claim-limit](../../../static/img/usage/payroll/maintenance/maintain-claim/add-fixed-claim.png)

5. Alternatively, you can insert the claim after process month end.

    ![process-month-end-add-claim](../../../static/img/usage/payroll/maintenance/maintain-claim/process-month-end-add-claim.png)

    1. Click on the "**Claim**"
    2. CLick on the ➕ to add the employee then fill in the claim

## Maintain Commission

1. Set the commission for employee

    - Navigate to **Payroll** > **Maintenance** > **Maintain Commission**
    - Create new for a new commission rate

    ![maintain-commision](../../../static/img/usage/payroll/maintenance/maintain-commission/maintain-commission.png)

2. Open pending payroll for commission

    - Payroll/Open pending payroll/Commission
    - Insert the employee and amount

    ![pending-payroll](../../../static/img/usage/payroll/maintenance/maintain-commission/pending-payroll.png)

3. Process month end

    1. Method 1 : Final Payroll Process

        - Navigate to **Payroll** > **New payroll** > **Process**

        ![process-month-end-1](../../../static/img/usage/payroll/maintenance/maintain-commission/process-month-end-1.png)

    2. Method 2 : Process Adhoc

       - Tick EPF & PCB & Monthly Fixed Allowance/Pending Payroll

       ![process-month-end-2](../../../static/img/usage/payroll/maintenance/maintain-commission/process-month-end-2.png)

    3. Tick Commission

    ![tick-comm](../../../static/img/usage/payroll/maintenance/maintain-commission/tick-comm.png)

4. Double click the employee that you gave commission

    ![check-employee](../../../static/img/usage/payroll/maintenance/maintain-commission/check-employee.png)

5. Refer to commission column

    ![result](../../../static/img/usage/payroll/maintenance/maintain-commission/result.png)

## Maintain Contribution

:::info
Learn how to set the Employee/Employer EPF rate, OT calculation and Tax calculation following this guide
:::

- Setting up maintain contribution helps you to categorise the type of contribution an employee received
- This would affect the types of contribution that they need to provide (EPF/SOCSO/PCB & etc)
- This is especially useful if you have different types of worker such as permanent worker, contract worker, foreign worker & etc

1. Navigate to **Payroll** > **Maintenance** > **Maintain Contribution**

   ![navigate](../../../static/img/usage/payroll/maintenance/maintain-contribution/navigate.png)

2. Click new to create new contribution

   ![new](../../../static/img/usage/payroll/maintenance/maintain-contribution/new.png)

3. Key in the info and tick the contribution needed

![key-in-1](../../../static/img/usage/payroll/maintenance/maintain-contribution/key-in-1.png)
![key-in-2](../../../static/img/usage/payroll/maintenance/maintain-contribution/key-in-2.png)

### Common contribution setup

| Local Permanent Workers                                                              | Foreign Workers                                                      |
| ------------------------------------------------------------------------------------ | -------------------------------------------------------------------- |
| ![local-permanent](../../../static/img/usage/payroll/maintenance/maintain-contribution/local-permanent.png) | ![foreign](../../../static/img/usage/payroll/maintenance/maintain-contribution/foreign.png) |

### Explanation of terms in Maintain Contribution panel

![explanation-1](../../../static/img/usage/payroll/maintenance/maintain-contribution/explanation-1.png)

![explanation-2](../../../static/img/usage/payroll/maintenance/maintain-contribution/explanation-2.png)

![explanation-3](../../../static/img/usage/payroll/maintenance/maintain-contribution/explanation-3.png)

## Maintain Deduction

:::info Features

Maintain Deductions is used to configure employee payroll deductions, such as personal loan deductions, company advance deductions, lateness deductions, and restaurant deductions.

Deductions can be fixed amounts or percentages; once configured, they are automatically deducted from payroll.

Deductions may affect net pay, tax calculations, and the inclusion or exclusion of contributions such as EPF/SOCSO. These settings should be based on company policies and regulations.

:::

1. Navigate to **Payroll** > **Maintenance** > **Maintain Deduction**

   ![navigate](../../../static/img/usage/payroll/maintenance/maintain-deduction/navigate.png)

2. Click New to generate a New Deduction

   ![new](../../../static/img/usage/payroll/maintenance/maintain-deduction/new.png)

3. Insert the info that you want to set in maintain deduction

   ![insert](../../../static/img/usage/payroll/maintenance/maintain-deduction/insert.png)

   1. Insert the Code of the Deduction that you want to generate.
   2. Insert the Description of the deduction.
   3. Insert the fixed amount for the deduction, eg: Loan deduction is fixed RM 100 for every employee then you can insert the rate of RM 100 but if there is not then you can left it blank.
   4. Select the type of the deduction you want (General / Zakat / Tabung Haji / PTPTN).
   5. Tick or un-tick the contribution of the deduction.

4. After create the master file of Deduction, then you can add the fixed deduction for certain employee which have the deduction monthly

   ![add-fixed-deduction](../../../static/img/usage/payroll/maintenance/maintain-deduction/add-fixed-deduction.png)

5. Alternatively, you can insert the deduction after process month end.

   ![process-month-end-add-deduction](../../../static/img/usage/payroll/maintenance/maintain-deduction/process-month-end-add-deduction.png)

   1. Click on the "**Deduction**"
   2. CLick on the ➕ to add the employee then fill in the deduction

6. Deduction feature is same with allowance feature, all the deduction is not compulsory just depend on company policy.

## Maintain Employee's Opening Balance

- Maintain employee’s opening balance is done when the respective employee enter the company in a month **later than January**.
- The previous PCB amount is **needed to key in so that the system can correctly calculate** the PCB amount that’s needed to pay every month.

1. Navigate to the **Open Payroll**

   ![navigate](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/navigate.png)

2. Double click the year in Open Payroll

   ![open-payroll](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/open-payroll.png)

3. Double click the transaction under ‘Opening’

   ![open-txn](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/open-txn.png)

4. Select the employee by double clicking on the name

   ![select-employee](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/select-employee.png)

5. Key in all the employee’s opening balance information

   ![key-in-employee-details](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/key-in-employee-details.png)

### Mapping of SQL 'opening' to EA form

![mapping](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/mapping.png)

### Special note for additional EPF and additional PCB

- Additional EPF and additional PCB are used when additional remuneration (bonus, commission, paid leave) is given.
- In the EA form, normal EPF and additional EPF is group into one.
- However, SQL recommend users to split the amount for a more detail input.

![notes](../../../static/img/usage/payroll/maintenance/maintain-employee-opening-balance/notes.png)

:::info
Frequency – Where one company will pay salary **twice or more times** in **a Month**.
:::

## Maintain Frequency

1. Navigate to **Payroll** > **Maintenance** > **Maintain Frequency**

    ![maintain-frequency](../../../static/img/usage/payroll/maintenance/maintain-frequency/maintain-frequency.png)

2. Click on **New** to preset your contribution.

    ![new](../../../static/img/usage/payroll/maintenance/maintain-frequency/new.png)

3. Go to **Human Resource** > **Maintain Employee**, Select the particular Employee and then Go to **Payroll Info Tab** and set the Frequency According to the Maintenance Frequency respectively.

    ![set-freq-1](../../../static/img/usage/payroll/maintenance/maintain-frequency/set-freq-1.png)

4. After save, you can check the allowance the employee is having. In this example, the employee Nicole has an Fixed Allowance of RM 230.

    ![set-freq-2](../../../static/img/usage/payroll/maintenance/maintain-frequency/set-freq-2.png)

5. Next, go to **Payroll** > **New payroll** > **Frequency**

    ![frequency](../../../static/img/usage/payroll/maintenance/maintain-frequency/frequency.png)

    1 Select the Frequency as you Set in Maintenance Frequency (EG: Half).

    2 The Employee/s that u have set as the Frequency type in Maintain Employee will show in this column

    3 Tick the Sequence that u wan to process.

    4 Click PROCESS

6. The following result below will show in the **HALF MONTH FREQUENCY PAYROLL**.

    ![result-1](../../../static/img/usage/payroll/maintenance/maintain-frequency/result-1.png)

7. When it is time to do month end, click on Payroll, look for New Payroll and click on Final Month End to process.

    ![result-2](../../../static/img/usage/payroll/maintenance/maintain-frequency/result-2.png)

8. Select the Employee ( Nicole ) that you’ve process Frequency. The following is an example result of the Employee that had process Frequency.

   - Wages - [2800 (Basic) – 1400 (Frequency) = 1400 ]
   - Allowance - [ 230 (Fixed) – 115 (Frequency) = 115 ]

    ![final-result](../../../static/img/usage/payroll/maintenance/maintain-frequency/final-result.png)

## Maintain Overtime

:::info Features

- Setting up maintain overtime helps you to categorize the type of overtime that company have.
- This would affect the types of contribution that they need to provide (EPF/SOCSO/PCB & etc)
- This setting will bring impact of the calculation of overtime.

:::

### Process Overtime After Month End

1. Click on **Payroll** > **Maintenance** > **Maintain Overtime**

   ![after-maintain-overtime](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-maintain-overtime.png)

2. In the list, you can find some default overtime settings. Click on **New** to generate a custom one

   ![after-new](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-new.png)

3. Key-in Overtime details as below

   ![after-enter-details](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-enter-details.png)

   - Insert the **Code** and **Description** of the overtime that you want to generate.
   - Insert the **Rate** of the overtime, eg : the overtime rate is 1.5 as per overtime amount or double, triple of the overtime amount.
   - **Unit Type** is to set the overtime calculation by hourly or by daily.
     -Set the contribution of overtime with EPF, SOCSO, PCB, EIS etc.

4. After that, when we need to process the payroll at the month end. Navigate to **Payroll** > **New Payroll**

   ![after-navigate-new-payroll](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-navigate-new-payroll.png)

5. Click **Final**, and click on **Process**

   ![after-click-process](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-click-process.png)

6. Click on any employee

   ![after-click-employee](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-click-employee.png)

7. Click on the "**Overtime**"

   ![after-click-overtime](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-click-overtime.png)

8. Click on the ➕ to add the info you want

   ![after-click-plus](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-click-plus.png)

9. Click on the "**Code**" to choose the overtime type

   ![after-select-code](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-select-code.png)

10. Key in the work unit as overtime hour, for example if Lee hong Wai overtime for 2 hours on that particular day, just key in numbering as 2 will do

    ![after-key-overtime-hour](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-key-overtime-hour.png)

11. Alternatively, you can click on the button beside Trans Date, and tick the column name Work Unit As Time

    ![after-tick-column](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-tick-column.png)

12. After call out the column of Work Unit As Time, you may key in he overtime minutes also (eg: 2 hours and 09 mins)
    ![after-key-overtime-minutes](../../../static/img/usage/payroll/maintenance/maintain-overtime/after-key-overtime-minutes.png)

### Process Overtime Before Month End

1. Click on payroll, open pending payroll.

   ![before-open-pending](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-open-pending.png)

2. Double Click on **Overtime**

   ![before-open](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-open.png)

3. Click on Append icon

   ![before-append-1](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-append-1.png)

   ![before-append-2](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-append-2.png)

4. Select employee

   ![before-select-employee](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-select-employee.png)

5. Select **Overtime Code**

   ![before-select-code](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-select-code.png)

6. Tick and enable the **Work Unit As Time**

   ![before-enable-work-unit-as-time](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-enable-work-unit-as-time.png)

7. Enter the time in the work unit as time, for example Lee Chong Wai worked overtime for 2hours and 30minutes, key in as shown below

   ![before-enter-time](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-enter-time.png)

8. Repeat the same steps as shown above for the other overtime records and save after all done

   ![before-repeat](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-repeat.png)

9. During month end,

   ![before-month-end-1](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-month-end-1.png)

   ![before-month-end-2](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-month-end-2.png)

10. Double click on the employee’s name or code

    ![before-click-employee](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-click-employee.png)

11. Click on the blue **Overtime** words

    ![before-click-overtime](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-click-overtime.png)

12. The overtime records entered in pending payroll will be shown

    ![before-overtime-records](../../../static/img/usage/payroll/maintenance/maintain-overtime/before-overtime-records.png)

### Import Excel Overtime Format into SQL Payroll

1. Prepare a table in Microsoft Excel as shown in the image below

   ![import-excel](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-excel.png)

   :::tip

   - **Date**: Trans Date
   - **Employee**: Code of Employee
   - **OT**: Code of Overtime that created in Maintain Overtime
   - **Unit**: Work Unit (count 2.50 = 150 minutes/2 and a half hours)
   :::

2. After done the table, go to file

   ![import-go-to-file](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-go-to-file.png)

3. Click on Save as

   ![import-save-as](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-save-as.png)

4. Select CSV file type

   ![import-select-csv](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-select-csv.png)

5. Click Save

   ![import-save](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-save.png)

6. Go to SQL Payroll > Payroll > Open Pending Payroll...

   ![import-open-pending-payroll](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-open-pending-payroll.png)

7. Double click on the Overtime

   ![import-click-overtime](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-click-overtime.png)

8. Click on the Import Data icon

   ![import-click-data](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-click-data.png)

9. Click on the … (3 dots button) to select your data source,

   ![import-click-dots-button](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-click-dots-button.png)

10. Select the csv file to import

    ![import-select-csv-file](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-select-csv-file.png)

11. Click on the Next button

    ![import-next](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-next.png)

12. Import from row 1, select Comma, select " for the text delimiter

    ![import-import](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-import.png)

13. Select the field for every column

    ![import-select-field-1](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-select-field-1.png)

14. Make sure you have select all the fields for the date, employee, code & workunit.

    ![import-select-field-2](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-select-field-2.png)

15. Change the Import from row to **2** and click the finish button

    ![import-finish](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-finish.png)

16. Click on the Close button after done importing the data

    ![import-close](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-close.png)

17. Click on the Save icon

    ![import-last-save](../../../static/img/usage/payroll/maintenance/maintain-overtime/import-last-save.png)

## Maintain Payment Method

- Maintain Payment Method helps you to categorise how you want to pay your employee
- This is useful when you have different type of banks (MBB, HLB & etc) and method of paying (Cash, Cheque, Transfer)
- At here, we can also set the **auto rounding** so that all payout is round to the nearest 5 cent

  - eg: Employee total pay = RM1234.**56**
  - After auto rounding, it will become RM1234.**55**

1. Navigate to the maintain payment method panel

   ![navigate](../../../static/img/usage/payroll/maintenance/maintain-payment-method/navigate.png)

2. Click new to create new payment method

   ![new](../../../static/img/usage/payroll/maintenance/maintain-payment-method/new.png)

3. Key in the information needed (Click save after configured)

   ![key-in-1](../../../static/img/usage/payroll/maintenance/maintain-payment-method/key-in-1.png)

   ![key-in-2](../../../static/img/usage/payroll/maintenance/maintain-payment-method/key-in-2.png)

### Explanation of auto rounding

**Without auto rounding**

![5](../../../static/img/usage/payroll/maintenance/maintain-payment-method/5.png)

- After month end will show **no adjustment**
- However, adjustment can be manually change by clicking the up/down arrow beside it

![6](../../../static/img/usage/payroll/maintenance/maintain-payment-method/6.png)

**With auto rounding**

- After month end will have **auto adjustment** to nearest 5 cents

![7](../../../static/img/usage/payroll/maintenance/maintain-payment-method/7.png)

## Maintain Wages

:::info Features

- Enable to set different other contribution for Bonus, Director Fee, Pay Leave and Unpaid Leave.
- Maintain the Employee & Employer EPF Rate.
- Maintain the working hour and day per month.
- Enable the Overtime Calculation base on Maintain Employee Setting. It will calculate the OT based on Wages amount in Maintain Employee.

:::

- Setting up maintain wages helps you to categorise the type of wages an employee received.
- This would affect the types of contribution that they need to provide (EPF/SOCSO/PCB & etc)
- This is especially useful if you have different types of worker such as
  permanent worker, contract worker, foreign worker & etc

1. Navigate to **Payroll** > **Maintenance** > **Maintain Wages**

   ![maintain-wages](../../../static/img/usage/payroll/maintenance/maintain-wages/maintain-wages.png)

2. Click new to create new wages type

   ![new](../../../static/img/usage/payroll/maintenance/maintain-wages/new.png)

3. Key in the info and tick the contribution needed

   ![fill-in-1](../../../static/img/usage/payroll/maintenance/maintain-wages/fill-in-1.png)
   ![fill-in-2](../../../static/img/usage/payroll/maintenance/maintain-wages/fill-in-2.png)

### Common wages setup

| Local Permanent Workers                                                       | Foreign Workers                                               |
| ----------------------------------------------------------------------------- | ------------------------------------------------------------- |
| ![local-permanent](../../../static/img/usage/payroll/maintenance/maintain-wages/local-permanent.png) | ![foreign](../../../static/img/usage/payroll/maintenance/maintain-wages/foreign.png) |

---
sidebar_position: 2
title: Guide
description: A guide to maintain payroll
slug: /usage/payroll/general
tags: ["SQL Payroll", "Payroll", "Month End", "Pending Payroll"]
---

## Create Payroll

### Maintain Employee's Opening Balance

- Maintain employee’s opening balance is done when the respective employee enter the company in a month **later than January**.
- The previous PCB amount is **needed to key in so that the system can correctly calculate** the PCB amount that’s needed to pay every month.

1. Navigate to the **Open Payroll**

   ![navigate](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/navigate.png)

2. Double click the year in Open Payroll

   ![open-payroll](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/open-payroll.png)

3. Double click the transaction under ‘Opening’

   ![open-txn](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/open-txn.png)

4. Select the employee by double clicking on the name

   ![select-employee](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/select-employee.png)

5. Key in all the employee’s opening balance information

   ![key-in-employee-details](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/key-in-employee-details.png)

#### Mapping of SQL 'opening' to EA form

![mapping](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/mapping.png)

#### Special note for additional EPF and additional PCB

- Additional EPF and additional PCB are used when additional remuneration (bonus, commission, paid leave) is given.
- In the EA form, normal EPF and additional EPF is group into one.
- However, SQL recommend users to split the amount for a more detail input.

![notes](../../../static/img/usage/payroll/setup/maintain-employee-opening-balance/notes.png)

:::info
Frequency – Where one company will pay salary **twice or more times** in **a Month**.
:::

### Final Process

Enable to process the Month Pay Salary and Final Pay Salary.

1. Click into **Payroll** and look for **New Payroll**.

   :::tip
   Certain company their payroll cut off date will not in the month end, some of the company will according to the 26th of the month, so you can preset your own company payroll cut off date through the "..." button.
   :::

   ![month-end](../../../static/img/usage/payroll/guide/create.png)

2. Click on the **Process** option.

### Frequency Process

To process mid month salary payroll. The salary payout is based on average % of the Fixed Salary.

Not the last Pay of the Month.

![pay-frequency](../../../static/img/usage/payroll/guide/pay-frequency.png)

### Ad Hoc Process

To process Mid Month Ad Hoc Payroll

![pay-adhoc](../../../static/img/usage/payroll/guide/pay-adhoc.png)

![pay-adhoc-bonusallow](../../../static/img/usage/payroll/guide/pay-adhoc-bonus-allowance.png)

Default this option

- All(PCB,Socso,EPF) Contribution for Fixed Transaction will be 0
- Value will be 0 (Zero) & user need to self enter a value for All/Selected Employee

![pay-adhoc-monthlyFA](../../../static/img/usage/payroll/guide/pay-adhoc-montly-fixed-allowance.png)

In this option allow the user to self control the Contribution (default 100%) for Fixed Transaction.

In other word if (eg Bonus with PCB (A) only just set Contribution to 0%)

## Open Payroll

:::info
Once you have created the payroll and you wish to view whatever you have did, then you can make some amendment.
:::

1. Navigate to **Payroll** > **Open Payroll**. Alternatively, access it from the home page by clicking **Open Payroll**

   ![open-navigate](../../../static/img/usage/payroll/guide/open-navigate.png)

2. Select employee, double click your employee name to check on its individual’s amount

   ![open-select-employee](../../../static/img/usage/payroll/guide/open-select-employee.png)

   :::info
   You can process 2 month end in the same day also. Initially, you can choose to tick those first batch employees.

   While processing the 2nd batch, you can tick the 2nd batch of users.

   Example:

   **BATCH 1**

   ![batch-1-payroll](../../../static/img/usage/payroll/guide/batch-1-payroll.png)

   ![batch-1-employees](../../../static/img/usage/payroll/guide/batch-1-employees.png)

   **BATCH 2**

   ![batch-2-payroll](../../../static/img/usage/payroll/guide/batch-2-payroll.png)

   ![batch-2-employees](../../../static/img/usage/payroll/guide/batch-2-employees.png)
   :::

## Open Pending Payroll

:::tip
Before you process the month end, you can use open pending payroll to key-in all others add hoc info like extra allowance, overtime, claim etc.
:::

- This is for the user to prepare the transaction (eg Overtime, Deduction) before Processing the Payroll...
- Available Pending Type Transactions:

  - Wages, Allowance, Tax Deduction, Overtime
  - Deduction, Advance Paid, Claims, Loan
  - CP38, Advance Deduct, Bonus, Paid Leave
  - Director Fees, Unpaid Leave, Tax Benefit, Commission

- After all the Pending had enter user may go either below step to for next step except Pending Advance Paid
  - New Payroll | Final Process
  - New_Payroll | Ad Hoc Process
- For Pending Advance Paid must use New_Payroll | Ad Hoc Process then only can use New Payroll | Final Process

### Steps

1. Go to **Payroll** > **Open Pending Payroll**.

    ![navigate](../../../static/img/usage/payroll/guide/navigate.png)

2. Double Click on the info that you want to input, eg: Overtime.

    ![pending-click-overtime](../../../static/img/usage/payroll/guide/pending-click-overtime.png)

3. Insert the overtime info accordingly

    1. Press on the ➕ button to add new overtime.

        ![pending-add-new-overtime](../../../static/img/usage/payroll/guide/pending-add-new-overtime.png)

    2. Insert the info accordingly like employee, overtime code, work unit etc

        ![pending-insert-info](../../../static/img/usage/payroll/guide/pending-insert-info.png)

    3. Once update accordingly then save.

        ![pending-overtime-save](../../../static/img/usage/payroll/guide/pending-overtime-save.png)

4. Once finish the update you may process the month end and observe the result.

    ![pending-result](../../../static/img/usage/payroll/guide/pending-result.png)

### Pending YYYY

- YYYY represents the Year (e.g. if in 2013 will show as Pending 2013).
- To show the pending in Monthly (with & without Transactions).

![open-pending-payroll-02](../../../static/img/usage/payroll/guide/open-pending-payroll-pending-yyyy.png)

### Pending Navigator

Show which Pending Type had transactions in the day view.

![open-pending-payroll-03](../../../static/img/usage/payroll/guide/open-pending-payroll-pending-navigator.png)

### Show all Pending Payroll

To show the pending in Yearly (with Transactions).

![open-pending-payroll-04](../../../static/img/usage/payroll/guide/open-pending-payroll-show-all-pending-payroll.png)

## Pending Transactions Types

1. Just click the + button on top of the Screen (The Green + and Money icon) to Insert record(s).

2. After done just Click the Blue Diskette icon on top of the Screen to save the record.

### Pending Wages

This is useful for employees to be paid by the number of days they work (i.e. users can add the day when the selected employee comes to work).

![pending-wages](../../../static/img/usage/payroll/guide/open-pending-payroll-wages.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Wages transaction date | Date |
| Post Date | Wages posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Wages type | Alphanumerical, length 20 |
| Description | Wages type description | Alphanumerical, length 160 |
| Amount | Wages amount | Decimal, length 18, precision 2 |

### Pending Overtime

![pending-overtime](../../../static/img/usage/payroll/guide/open-pending-payroll-overtime.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Overtime transaction date | Date |
| Post Date | Overtime posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Overtime type | Alphanumerical, length 20 |
| Description | Overtime type description | Alphanumerical, length 160 |
| Work Unit | It can be in Hours or Day depend what Overtime Type selected and Unit type is set at Maintain Overtime | Decimal, length 18, precision 8 |
| Rate | Overtime rate | Decimal, length 18, precision 8 |
| Day Type | It follow the Post Date to determine the Day Type which is set at Maintain Calender | Alpha, length 1 |
| Work Unit As Time | Overtime entered as time (HH:MM:SS) | Time |

### Pending Paid Leave

![pending-paid-leave](../../../static/img/usage/payroll/guide/open-pending-payroll-paid-leave.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Paid leave transaction date | Date |
| Post Date | Paid leave posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Description | Paid leave description | Alphanumerical, length 160 |
| Amount | Paid leave amount | Decimal, length 18, precision 2 |

### Pending Unpaid Leave

![pending-unpaid-leave](../../../static/img/usage/payroll/guide/open-pending-payroll-unpaid-leave.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Unpaid leave transaction date | Date |
| Post Date | Unpaid leave posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Unpaid leave type | Alphanumerical, length 20 |
| Description | Unpaid leave type description | Alphanumerical, length 160 |
| Leave Day | Number of unpaid leave days | Decimal, length 18, precision 8 |
| Amount | Unpaid leave amount (Leave blank if want calculated by system) | Decimal, length 18, precision 2 |

### Pending Claim

![pending-claim](../../../static/img/usage/payroll/guide/open-pending-payroll-claim.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Claim transaction date | Date |
| Post Date | Claim posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Claim type | Alphanumerical, length 20 |
| Description | Claim type description | Alphanumerical, length 160 |
| Ref1 | Claim reference 1 | Alphanumerical, length 20 |
| Ref2 | Claim reference 2 | Alphanumerical, length 20 |
| Amount | Claim amount | Decimal, length 18, precision 2 |

### Pending CP38

This is generally towards settlement of outstanding taxes.

![pending-cp38-01](../../../static/img/usage/payroll/guide/open-pending-payroll-cp3801.png)

![pending-cp38-02](../../../static/img/usage/payroll/guide/open-pending-payroll-cp3802.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | CP38 transaction date | Date |
| Post Date | CP38 posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Description | CP38 description | Alphanumerical, length 160 |
| Ref1 | Reference 1 | Alphanumerical, length 20 |
| Ref2 | Reference 2 | Alphanumerical, length 20 |
| Amount | CP38 amount | Decimal, length 18, precision 2 |
| Generate Button | For Batch Generate CP38 | |

### Pending Allowance

![pending-allowance](../../../static/img/usage/payroll/guide/open-pending-payroll-allowance.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Allowance transaction date | Date |
| Post Date | Allowance posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Allowance type | Alphanumerical, length 20 |
| Tax Code | Tax exemption code | Alphanumerical, length 20 |
| Description | Allowance type description | Alphanumerical, length 160 |
| Work Unit | Allowance unit | Decimal, length 18, precision 8 |
| Rate | Allowance rate | Decimal, length 18, precision 8 |
| Amount | Allowance total amount | Decimal, length 18, precision 2 |

### Pending Deduction & Pending Commission

Below Example information is applicable for

- Pending Deduction
- Pending Commission

![pending-deduction-commission](../../../static/img/usage/payroll/guide/open-pending-payroll-deduction.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Deduction / Commission transaction date | Date |
| Post Date | Deduction / Commission posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Deduction / Commission type | Alphanumerical, length 20 |
| Description | Deduction / Commission description | Alphanumerical, length 160 |
| Work Unit | Deduction unit | Decimal, length 18, precision 8 |
| Rate | Deduction rate | Decimal, length 18, precision 8 |
| Amount | Deduction total amount | Decimal, length 18, precision 2 |

### Pending Bonus & Pending Director Fees

Below Example information is applicable for

- Pending Bonus
- Pending Director Fees

![pending-bonus-director-fees](../../../static/img/usage/payroll/guide/open-pending-payroll-bonus.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Bonus / Director fees transaction date | Date |
| Post Date | Bonus / Director fees posting date | Date |
| Pay Year | Bonus year (Default is same year as Post Date) | Integer |
| Employee | Employee code | Alphanumerical, length 30 |
| Tax Category | Employee tax category | Alphanumerical, length 10 |
| EPF Rate | Bonus EPF rate | Alphanumerical, length 10 |
| Wages | Employee wages amount | Decimal, length 18, precision 2 |
| Amount | Bonus / Director fees amount | Decimal, length 18, precision 2 |

### Pending Advance Paid, Pending Advance Deduct & Pending Loan

Below Example information is applicable for

- Pending Advance Paid
- Pending Advance Deduct (Only View because it derive from Advance Paid after Ad Hoc Process)
- Pending Commission

![pending-advance-paid-advance-deduct-commission](../../../static/img/usage/payroll/guide/open-pending-payroll-advance-paid.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Advance / Loan transaction date | Date |
| Post Date | Advance / Loan posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Description | Description | Alphanumerical, length 160 |
| Ref1 | Reference 1 | Alphanumerical, length 20 |
| Ref2 | Reference 2 | Alphanumerical, length 20 |
| Amount | Advance paid amount | Decimal, length 18, precision 2 |

### Pending Tax Benefit & Pending Tax Deduction

Below Example information is applicable for

- Pending Tax Benefit
- Pending Tax Deduction

![pending-tax-benefit-tax-deduction](../../../static/img/usage/payroll/guide/open-pending-payroll-tax-deduct.png)

| Field Name | Description | Type / Length / Precision |
|---|---|---|
| Trans Date | Tax deduction / benefit transaction date | Date |
| Post Date | Tax deduction / benefit posting date | Date |
| Employee | Employee code | Alphanumerical, length 30 |
| Code | Tax deduction code | Alphanumerical, length 20 |
| Description | Tax deduction description | Alphanumerical, length 160 |
| Ref1 | Reference 1 | Alphanumerical, length 20 |
| Ref2 | Reference 2 | Alphanumerical, length 20 |
| Amount | Tax deduction description | Decimal, length 18, precision 2 |

## Example of create open pending payroll

### Advance Paid

:::info
Employee request advance salary before month end
:::

1. Navigate to **Payroll > Open Pending Payroll**

2. **Select Advance Paid**

    ![select-advance-paid](../../../static/img/usage/payroll/guide/select-advance-paid.png)

3. **Key in accordingly**

    >***Trans date*** = date apply advance paid
    >
    >***Employee*** = which employee
    >
    >***Amount*** = amount advance paid

    ![fill-in](../../../static/img/usage/payroll/guide/fill-in.png)

4. Go to Payroll > New Payroll

5. Choose Ad Hoc

6. Set the date when your employee take advance paid

7. Under Process > select Monthly Fixed Allowance / Pending Payroll (will come out the dialog box as pic attached)

8. Tick "Advanced Paid"

    ![config](../../../static/img/usage/payroll/guide/config.png)

9. Process

    ![process](../../../static/img/usage/payroll/guide/process.png)

10. Process Month end Payroll as usual, you will found there is advance deduct at the month end.

    ![result](../../../static/img/usage/payroll/guide/result.png)

### Bonus

1. Navigate to **Payroll** > **Open Pending Payroll**

   ![navigate](../../../static/img/usage/payroll/guide/navigate.png)

2. Click on Bonus

   ![click-bonus](../../../static/img/usage/payroll/guide/click-bonus.png)

3. Next, adjust the bonus of your employee

   ![adjust-employee](../../../static/img/usage/payroll/guide/adjust-employee.png)

   1. Click “Add”
   2. Select your employee
   3. Key in amount
   4. Save

4. Go to **Payroll** > **New Payroll** and click on **Ad Hoc**

   ![adhoc](../../../static/img/usage/payroll/guide/adhoc.png)

5. Tick **EPF** if you want to deduct **EPF**, Tick **PCB** if you want to deduct **PCB**

   ![epf-pcb](../../../static/img/usage/payroll/guide/epf-pcb.png)

6. Tick Bonus / Allowance (To input your amount)

   ![tick-bonus](../../../static/img/usage/payroll/guide/tick-bonus.png)

7. Change the Description (Optional) and tick the employee you rewarded with bonus

   ![change-desc](../../../static/img/usage/payroll/guide/change-desc.png)

8. Complete and check the payslip

   ![result](../../../static/img/usage/payroll/guide/result.png)

### CP38

- CP38 is a **instruction** to Deduct Salary which **issued by LHDN**. This CP38 instruction requires that the employer **make additional deductions in monthly installments** from the salary of the taxpayer (other than a Monthly Tax Deduction) towards settlement of taxpayer’s income tax arrears.
- The Salary Deduction Order (CP38) for tax payment in instalments aims to ease the burden **of the taxpayer** who should be paying the tax arrears in one lump sum under the Income Tax Act 1967.

1. **Open Pending Payroll** and choose **CP38**

    ![select-cp38](../../../static/img/usage/payroll/guide/select-cp38.png)

2. Press **GENERATE** on the top left of the window.

    ![generate](../../../static/img/usage/payroll/guide/generate.png)

3. Key in the Amount you receive from LHDN Letter, for example this employee ( 00001- Lucious ) had to pay CP38 on **June ( RM450 )** and July **( RM550 )**. Press **GENERATE**.

    ![fill-in-details](../../../static/img/usage/payroll/guide/fill-in-details.png)

4. Press **SAVE**

    ![save](../../../static/img/usage/payroll/guide/save.png)

5. This **pending** task only needs to be completed **once**. It will impact **both the June and July month-end processes**. The following pictures below will illustrate the end result :

    ![result](../../../static/img/usage/payroll/guide/result.png)

## Generate Payment Voucher / Journal Entry

:::success[note]
This is **Additional Module** (Payroll Accounting (SQL Payroll))
:::

1. To generate the monthly payroll data converted into double entry and get post into SQL Account.

2. It is available in **SQL Payroll version 129** and above.

3. It is available to import payroll data in **SQL Account version 745** and above.

    ![export-import-as-pv-je](../../../static/img/usage/payroll/guide/export-import-as-pv-je.jpg)

### Overview of the Process Flow

![overview-process-flow](../../../static/img/usage/payroll/guide/overview-process-flow.jpg)

### Configure Payroll Accounting (1 time setup)

Go to **Menu : Payroll | Generate Payment Voucher / Journal Entry...**

1. At Generate Payment Voucher / Journal Entry, click on **Configure Payroll Accounting.**

    ![insert-process-and-date](../../../static/img/usage/payroll/guide/insert-process-and-date.jpg)

2. Overview of the Configure Payroll Accounting settings screen.

    ![configure-payroll-accounting](../../../static/img/usage/payroll/guide/configure-payroll-accounting.jpg)

#### Step 1: Save GL Account to File (SQL Account)

1. Login the SQL Account database.

2. Go to **File | Import | (SQL Payroll) Import Payment Voucher / Journal Entry | Save GL Account File**

    ![navigate-import-payment-voucher](../../../static/img/usage/payroll/guide/navigate-import-payment-voucher.png)

    ![save-gl-account-to-file](../../../static/img/usage/payroll/guide/save-gl-account-to-file.png)

3. Save SQL Account file to Desktop.

    ![save-gl-to-file](../../../static/img/usage/payroll/guide/save-gl-to-file.jpg)

#### Step 2: SQL Account GL Code

1. Click on **Load From File**.

    ![load-from-sql-account](../../../static/img/usage/payroll/guide/load-from-sql-account.jpg)

2. Select a **SQL Account file (*.txt)** and click **Open**.

    ![load-sql-account-file](../../../static/img/usage/payroll/guide/load-sql-account-file.jpg)

3. After the SQL Account GL Code has loaded, the company name will be display and last saved date and time.

    ![display-company-name-and-last-saved-date-and-time](../../../static/img/usage/payroll/guide/display-company-name-and-last-saved-date-and-time.jpg)

4. Click Remove File button if you wish to load the new chart of account.

#### Step 3: GL Account Mapping

1. After load the chart of accounts (in step 2), you are able to lookup and **map the GL Account code** to wages, allowance, overtime, bonus, etc accordingly.

    ![gl-account-mapping](../../../static/img/usage/payroll/guide/gl-account-mapping.jpg)

2. Example of the account mapping:

    ![account-mapping-table](../../../static/img/usage/payroll/guide/account-mapping-table.png)

#### Step 4: Posting Method

1. Generate posting entry by **Payment Voucher** or by **Journal Entry**.

2. Group by **Employee** (available in payment voucher), **Branch, Department, HR group, or Category**.

3. Tick to **With Project Code** to post the entry with project code.

4. OPTIONAL: Generate Journal Entry for Employer EPF, SOCSO Accrual **(by default is untick)**. For some company might charge the Employer EPF and SOCSO accrual in next month.

    ![posting-method](../../../static/img/usage/payroll/guide/posting-method.jpg)

### Generate Payment Voucher / Journal Entry (Export)

    To generate the Payment Voucher or Journal Entry from SQL Payroll. Click on **Generate**.

    ![generate-pv-je](../../../static/img/usage/payroll/guide/generate-pv-je.jpg)

### Import Payment Voucher / Journal Entry (Import)

1. Login the SQL Account database.

2. Go to **File | Import | (SQL Payroll) Import Payment Voucher / Journal Entry...**

3. Click on **Select File** from the Payment Voucher/Journal Entry (payroll data) generate from SQL Payroll.

    ![import-pv-je](../../../static/img/usage/payroll/guide/import-pv-je.jpg)

4. Click on **Execute**.

    ![import-pv-je-successful](../../../static/img/usage/payroll/guide/import-pv-je-successful.jpg)

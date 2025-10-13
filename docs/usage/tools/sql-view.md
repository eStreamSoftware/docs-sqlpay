---
sidebar_position: 1
title: SQL View
description: A guide of setting user view on certain records and data
slug: /usage/tools/sql-view
tags: ["SQL Payroll", "SQL View"]
---

:::info
SQL view module is to lock certain user to view from all employees, in other word only allow handling a group of employee.

If you haven’t register, you may try by turn on SQL View module under :
File > Customize SQL Payroll Module.
:::

## Setup

:::note Example
In this example scenario, the goal is allowing KL User to view/ edit only the employee in KL branch.
:::

1. Navigate to Tools > DIY > Maintain DIY

   1. Go to **View Template** tab

   2. Right Click **Employee** > Select **New View Template**

      ![new-template](../../../static/img/usage/tools/sql-view/new-template.png)

   3. Press New

   4. Enter description, enter condition and save

      ![save-template](../../../static/img/usage/tools/sql-view/save-template.png)

   5. Right click the new created view template > select **User View**

      ![user-view](../../../static/img/usage/tools/sql-view/user-view.png)

   6. Assign user view to this group of employee

      ![assign-user-view](../../../static/img/usage/tools/sql-view/assign-user-view.png)

   7. Logon as KL User.

2. Result:

   - Before:

     ![result-before](../../../static/img/usage/tools/sql-view/result-before.png)

   - After:

     ![result-after](../../../static/img/usage/tools/sql-view/result-after.png)

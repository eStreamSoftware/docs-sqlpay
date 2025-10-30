---
sidebar_position: 3
---

# Create Target

Target is a quantitative mission (countable data). E.g. Sales Target, Input Data.

:::info[Note]

This feature is only available to **manager**.

:::

## Step 1 - Target Information

![target](../../../../../../static/img/integration/vision/mi_creation/t-1.png)

| Properties                   | Description                                                                        | Note     |
|:-----------------------------|:-----------------------------------------------------------------------------------|:--------:|
| **Title**                | The title of the mission.                                                          | Required |
| **Description**          | A detailed description of the mission.                                             | - |
| **Start Date**           | The date when the mission begins.                                                  | Required |
| **End Date**             | The date when the mission ends. The end date must be later than the start date.    | Required |
| **Clear**                | Clears all content on the current page.                                            | -        |
| **Next**                 | Navigates to the next page.                                                        | -        |

## Step 2 - Rewards Information

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.jpg)

| Properties                          | Description                                                                              | Note         |
|:------------------------------------|:-----------------------------------------------------------------------------------------|:------------:|
| **[Grouping Type](#grouping-type)** | Section to select the target grouping type, either *Individual* or *Team*.               | Required     |
| **[Strategy](#strategy)**           | Section to select the target strategy, with options predefined in **Company Configuration**. | Required     |
| **[Condition](#condition)**         | Section to select the target condition. *(e.g., Between, More than)*                  | Required     |
| **[Target and Rewards](#target-and-rewards)**| Section to enter details about the targets and their associated rewards.        | At least one |
| **[Payment By](#payment-by)**       | Section to select the payment method and specify the payout month.                       | Required     |
| **Clear**                           | Clears all content on the current page.                                                  | -            |
| **Back**                            | Navigates to the previous page.                                                          | -            |
| **Next**                            | Navigates to the next page.                                                              | -            |

### Grouping Type

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.1.png)

There are two types of **Grouping Types**:

1. **Individual:**
   - Selecting Individual means that the targets and rewards **apply to each participant** added or who joins this target mission.
   - **Example:** If the target is RM 10,000 and the reward is 1%, each participant will have a target of RM 10,000 and a reward of 1%.

2. **Team:**

   - Selecting Team means that the targets and rewards apply **only to the Team Leader** assigned to this target mission.
   - **Example:** If the target is RM 50,000 and the reward is 5%, the team leader receives the reward only when the combined target achieved by all team members exceeds RM 50,000.

:::info[Note]

Team option is not available for quests.

:::

:::tip Tips to create a Team Target Mission

To set up a team target, create two identical missions: one with the **Individual** setting and the other with the **Team** setting.

1. Add the team leader to the Team target and their team members to both the Team and Individual targets.

2. The team leader’s target will now reflect the collective achievements of the entire team and include a unique reward, while each member will have their own individual targets and rewards!

:::

### Strategy

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.2.png)

**Strategy** refers to the formula that helps managers and the application determine which specific target a mission belongs to. This formula allows the application to accurately retrieve the target amount from the SQL Account. For more details, see [**Linking to SQL Account | Strategy**](../../../linking-to-account.md#strategy).

:::tip Example Scenario

Suppose you’re managing a Sales Department and want to track Q1 sales targets:

1. For the mission **"Achieve Q1 Sales Target"**, assign the **"Invoice Based Strategy"** strategy.

2. With this setup, managers can update sales progress daily in SQL Vision by using SQL Vision Sync tool, mapping it to the correct Strategy ID. Managers can then view the updated progress daily in SQL Vision.

:::

### Condition

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3.png)

**Condition** specifies the criteria for calculating target rewards.

#### A. Between

The "Between" condition is designed to allocate rewards based on an employee’s achievement falling within a defined range. Specifically, rewards are granted when an employee's achievement meets the following criteria:

- It is greater than the lower boundary (X amount).
- It is less than or equal to the upper boundary (Y amount).

It is essential to ensure the upper limit (Y) of one target matches the lower limit (X) of the subsequent target to ensure continuity and avoid gaps.

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3-example.png)

1. If an employee achieves **RM15,000**, the employee will fall in **Target 1** and receive **2%** reward.
2. If an employee achieves **RM25,000**, the employee will fall in **Target 2** and receive **3%** reward.

#### B. More Than

The "More Than" condition is used to grant rewards when an employee surpasses a specified target amount (X). The rewards are granted according to the below criteria:

- Each reward is granted only **once**, regardless of how far the employee's achievement exceeds the target.
- Achieving a higher target **excludes rewards for lower targets**, ensuring that only the highest applicable reward is granted.

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3-example2.png)

1. If an employee achieves **RM15,000**, they will receive **2%** reward because their achievement **exceeds RM10,000 but does not surpass RM20,000**.
2. If an employee achieves **RM25,000**, they will receive **3%** reward because their achievement **exceeds RM20,000**, which excludes the reward for the lower target (2% Reward).

#### C. Less Than

The "Less Than" condition is designed to grant rewards when an employee achieves a result below a specified target amount (X). This condition is typically applied in scenarios where lower values are preferable, such as reducing errors or minimizing return stock. The rewards are granted according to the below criteria:

- Each reward is granted only **once**, based on the smallest qualifying target achieved.
- Achieving a lower target amount **excludes rewards for higher targets**.

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3-example3.png)

1. If an employee has **2 return stock**, they will receive **RM3,000 & 10,000 coins** because their performance is **below 3**, which excludes the second target reward.
2. If an employee has **4 return stock**, they will receive **RM1,000 & 5,000 coins** bacause their performance is **below 10 but above or equal 3**, therfore not qualified for the reward in Target 1.

#### D. More Than and Equal

The "More Than and Equal" condition grants rewards when an employee’s achievement meets or exceeds a specified target amount (X). The rewards are granted according to the below criteria:

- Each reward is granted only **once**, corresponding to the highest applicable target achieved.
- Achieving a higher target automatically **excludes rewards for lower targets**.

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3-example4.png)

1. If an employee achieves **5 new customers**, they will receive **RM1,000 & 5,000 coins** because their achievement is **5 or more customers** but does not meet the next threshold of 10 or more customers.
2. If an employee achieves **12 new customers**, they will receive **RM3,000 and 10,000 coins** because their achievement is **10 or more customers**, which excludes first target rewards.

#### E. Less Than and Equal

The "Less Than and Equal" condition is applied to reward employees who achieve results at or below a specified target amount (X). The rewards are granted according to the below criteria:

- Each reward is granted only **once**, based on the smallest qualifying target achieved.
- Achieving a smaller target automatically **excludes rewards for higher targets**.

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.3-example5.png)

1. If an employee has **3 return stock**, they will receive **RM3,000 & 10,000 coins** because their performance is **3 or less**, which excludes rewards for any higher targets.
2. If an employee has **4 return stock**, they will receive **RM1,000 & 5,000 coins** because their performance is **10 or less but above 3**, making them ineligible for Target 1's reward.

### Target and Rewards

![target](../../../../../../static/img/integration/vision/mi_creation/t-2.4.png)

| Properties  | Description                                                                                              |
|-------------|----------------------------------------------------------------------------------------------------------|
| **Target**  | Text field to input the target amount. (Note: Only the **Between** condition will have two text fields.) |
| **Rewards** | Text field to enter the rewards available to the achievers of the particular target. There are 3 types of rewards: <br/> &nbsp;&nbsp; 1. **Percentage (%):** A percentage of the target amount awarded to the members *(e.g., 2%)*. <br/> &nbsp;&nbsp; 2. **Cash (RM):** Commission or allowance provided through the SQL Account on the payout date. <br/> &nbsp;&nbsp; 3. **Coins:** Digital coins that can be used to redeem gifts in SQL Vision via [**Gift**](../../../gift/introduction.md). |
| **Add**     | Adds a new target along with its respective rewards.                                                     |
| **Delete**  | Deletes a specific target and its associated rewards.                                                    |

### Payment By

:::info[Note]

The payment method applies only to **Cash**. All coins will be paid immediately upon entitlement.

:::

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.3.png)

There are two types of payment methods:

1. **Payment Terms:**
   - The payout month, which occurs X months after the entitled month.

      *E.g., If set to 3 months, the reward will be paid 3 months after the employee becomes entitled to it.*

2. **Settlement Month:**
   - Entitled cash will be accumulated until a specific month for payout, which can be either inclusive or exclusive of that month.
   - **Inclusive Setting:** *If January and August are set as inclusive months, rewards entitled from February to August will be paid in August, while rewards entitled from September to January will be paid in January.*
   - **Exclusive Setting:** *If January and August are set as exclusive months, rewards entitled from January to July will be paid in August, and rewards entitled from August to December will be paid in January.*

## Step 3 - Participants Information

### Participant Role

The participant role in **Team and Individual Target** are different and works differently:

#### Admin

- **Admin** is authorized to **manage and edit** the task.
- Admin does not perform the task and therefore **is not entitled to any rewards**.
- By default, the creator will be added as Admin and cannot be removed by anyone. *(Employee with yellow crown, as shown in image below, is the creator.)*

#### Team Leader *(Team only)*

- The **Team Leader** is responsible for **leading the mission**.
- A **leader is required** in a team target.
- The leader does not contribute to the target directly, but is **entitled to rewards based on the combined performance of the Team Members**, as defined in **[Step 2 - Rewards Information](#step-2---rewards-information)**. See **[Grouping Type](#grouping-type)** for more details.

#### Team Members *(Team only)*

- **Team Members** are employees who **contribute their target achievements** toward the team goal.
- The **combined performance of all team memebers** determines whether the Team Leader qualifies for a reward.
- Rewards are **given only to Team Leader** if the total achievements meet the target set in **[Step 2 - Rewards Information](#step-2---rewards-information)**. See **[Grouping Type](#grouping-type)** for more details.

#### Participant

- **Participant** is the employee responsible for performing the mission.
- They are eligible to receive the reward.

### Features

| Team Target | Individual Target |
|:-----------:|:-----------------:|
| ![Team Target](../../../../../../static/img/integration/vision/mi_creation/participant-team.png) | ![Individual Target](../../../../../../static/img/integration/vision/mi_creation/participant.png) |

| Properties              | Description                                                              |
|:------------------------|:-------------------------------------------------------------------------|
| **Apply Group**         | Allow you to apply group. See more in [**group**](../../../group#apply-group).     |
| **Clear**               | Clears all content on the current page.                                  |
| **Make Quest**          | Converts your mission into a Quest. See more in [**quest**](quest).      |
| **Add Person Icon**     | Add employees as the participant type.                                   |
| **Delete Icon**         | Delete the particular employee.                                          |
| **Back**                | Navigates to the previous page.                                          |
| **Create**              | Creates the mission.                                                     |

### Steps to add Participants

![Steps to add Participants](../../../../../../static/img/integration/vision/mi_creation/participant-steps.png)

1. Press on the **Add Person Icon** in the section for the participant role you want to add.
2. Select participants.
3. Press **Apply** to assign the selected employees to the participant role.
4. Press **Cancel** to discard current changes.

#### Side functions

| Properties              | Description                                                              |
|:------------------------|:-------------------------------------------------------------------------|
| **Search**              | Allows you to search for employees by their names.                       |
| **[Filter](assignment#filter)**   | Allow you to filter and sort the employee list.                |
| **Select All**          | Allow you to select all employees at once.                               |

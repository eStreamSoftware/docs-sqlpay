---
sidebar_position: 2
---

# Create Assignment

Assignment is a qualitative mission (non-countable). E.g. Idea brainstorm, Clothes design.

:::info[Note]

This feature is only available to **manager**.

:::

## Step 1 - Assignment Information

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-1.png)


| Properties               | Description                                                                        | Note     |
|:-------------------------|:-----------------------------------------------------------------------------------|:--------:|
| **Title**                | The title of the mission.                                                          | Required |
| **Description**          | A detailed description of the mission.                                             | Required |
| **[Project/Job/Task](#projectjobtask)** | The category for the mission, indicating whether it relates to a project, job, or specific task. | - |
| **Start Date**           | The date when the mission begins. The start date must be today or a future date.   | Required |
| **End Date**             | The date when the mission ends. The end date must be later than the start date.    | Required |
| **Clear**                | Clears all content on the current page.                                            | -        |
| **Next**                 | Navigates to the next page.                                                        | -        |

### Project/Job/Task

Select a **Project**, **Job**, and **Task** from the dropdown. If you leave any of these fields set to **(None)**, the Manager's Project, Job, and Task will be used in the SQL Payroll.

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-1.3.png)

## Step 2 - Milestone and Rewards

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.png)

| Properties                                          | Description                                                           | Note         |
|:----------------------------------------------------|:----------------------------------------------------------------------|:------------:|
| **[Milestone and Rewards](#milestone-and-rewards)** | Section for entering details about milestones and associated rewards. | At least one |
| **[Consultant Rewards](#consultant-rewards)**| Section for selecting consultants and specifying their respective rewards.| Required     |
| **[Payment By](#payment-by)**                | Section for selecting the payment method and specifying the payout month. | Required     |
| **[Bonus](#bonus)**                          | Section for entering additional bonus rewards.                            | -            |
| **Clear**                                    | Clears all content on the current page.                                   | -            |
| **Back**                                     | Navigates to the previous page.                                           | -            |
| **Next**                                     | Navigates to the next page.                                               | -            |

### Milestone and Rewards

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.1.png)


| Properties          | Description                                                           |
|---------------------|-----------------------------------------------------------------------|
| **Milestone (%)**   | Text field to input the percentage of the milestone (e.g., 20%).      |
| **Description**     | Text field to input the description of the milestone (e.g., the requirements to achieve the particular milestone). |
| **Rewards**         | Text field to enter the rewards available to the achievers of the particular milestone. There are 2 types of rewards: <br/> &nbsp;&nbsp; 1. **Cash (RM):** Commission or allowance provided through the SQL Account on the payout date. <br/> &nbsp;&nbsp; 2. **Coins:** Digital coins that can be used to redeem gifts in SQL Vision via [**Gift**](../../../gift/introduction.md). |
| **Add**             | Adds a new milestone along with its respective rewards.               |
| **Delete**          | Deletes a specific milestone and its associated rewards.              |

### Consultant Rewards

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.2.png)

**Consultants** are employees responsible for providing guidance on a particular mission. They do not complete the mission themselves.

To add a consultant click on ![add person](../../../../../../static/img/integration/vision/mi_creation/a-2.2-add.png) to navigates to the Select Consultant page. The selected consultants will be listed down in the Consultant Rewards section under the associated rewards.

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.2.2.png)

### Payment By

:::info[Note]

The payment method applies only to **Cash**. All coins will be paid immediately upon entitlement.

:::

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.3.png)

There are two types of payment methods:

1. **Payment Terms:**
   - The payout month, which will be X months after the entitled month.
   - E.g., if set to 3 months, the reward will be paid after 3 months from when the employee achieved and became entitled to the reward.

2. **Settlement Month:**
   - The entitled cash will be collected until a specific month for payment, either inclusive or exclusive of that month.
   - **Inclusive Setting:** If inclusive with January and August, all rewards entitled from February to August will be paid in August, while rewards entitled from September to January will be paid in January.
   - **Exclusive Setting:** If exclusive with January and August, all rewards entitled from January to July will be paid in August, and rewards entitled from August to December will be paid in January.

### Bonus

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-2.4.png)

| Properties    | Description                                                                         |
|---------------|-------------------------------------------------------------------------------------|
| **Description** | Text field to input a description of the bonus (e.g., extra points that you hope the employee can achieve, though it is not mandatory). |
| **Rewards**   | Text field to enter the rewards available to the achievers of the particular bonus. |
| **Add**       | Adds a new bonus along with its respective rewards.                                 |
| **Delete**    | Adds a new bonus along with its respective rewards.                                 |


## Step 3 - Add Members

There are 4 combination of members that can be created in Assignment:

1. **Normal member:**  
  An employee who performs the mission without a specific management or advisory role.

2. **Admin:**  
  An employee authorized to manage the task but does not complete the mission themselves. Admin shall not be entitled to any reward.

3. **Consultant:**  
  An employee who provides guidance on the mission without directly managing or completing it (e.g., an advisor).

4. **Consultant and Admin:**  
  An employee who both guides the mission and manages the task but does not complete the mission themselves. This employee will be entitled to consultant's reward.

The *Normal Member* and *Admin* can be created in **[Add Members](#step-3---add-members)** in Step 3, on the other hand the *Consultant* and *Consultant and Admin* combination can be created in **[Consultant Reward](#consultant-rewards)** in Step 2.

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-3.png)

| Properties              | Description                                                              | 
|:------------------------|:-------------------------------------------------------------------------|
| **Search**              | Allows you to search for employees by their names.                       | 
| **[Filter](#filter)**   | Allow you to filter and sort the employee list.                          | 
| **Group**               | Allow you to apply group. See more in [**group**](../../../group#apply-group).     | 
| **Select All**          | Allow you to select all employees at once.                               |
| **Make Quest**          | Converts your mission into a Quest. See more in [**quest**](quest).      |
| **Back**                | Navigates to the previous page.                                          |
| **Create**              | Creates the mission.                                                     |

#### Filter

![assignment](../../../../../../static/img/integration/vision/mi_creation/a-3.2.png)

The employee list can be filtered and sort by:

- Branch
- Department
- HR Group

---
title: Upskill Creation
description: A brief guide on upskill creation
sidebar_position: 1
---

# Upskill Creation
## Creation Steps
### Step 1 - Course Information
![Course Info Diagram](../../../../../static/img/integration/vision/upskillCreation/step1_courseInfo.png)

| <div align="center">Properties</div>          | <div align="center">Description</div>     | Required | <div align="center">Note</div> |
|:----------------------------------------------|:------------------------------------------|:--------:|:----|
| **Title**                                 | The title of the course.                  | ✓        | -   |
| **Description**                           | A detailed description of the course.     | ✗        | -   |
| **Tutor**                                 | The main tutor of the course.             | ✓        | -   |
| **Assistant Tutor**                       | The assistant tutor for the course.       | ✗        | -   |
| **Clear**                                 | Clears all course information on the current page.   | -        |        **Manager:**<br/>Clears all course information.<br/><br/>**Tutor Assistants:**<br/>Clears all excepts tutor and assistants information.|
| **Next**                                  | Navigate to the next page.               | -        | -   |  

<br/>
#### Tutor
- **Tutor** is the employee responsible for giving lessons and providing guidance throughout the learning process in the course. 
- There will be only **one** lead tutor in every course. 

![Add Tutor Diagram](../../../../../static/img/integration/vision/upskillCreation/step1_addTutor.png)
![Add Multiple Tutors Diagram](../../../../../static/img/integration/vision/upskillCreation/step1_addMultipleTutor.png)

<br/>
####  Assistant Tutor
- **Assistant Tutor** plays a role in supporting the lead tutor in completing the course smoothly. 
- There can be **multiple** assistant tutors in every course. 

![Add Assistant Tutors Diagram](../../../../../static/img/integration/vision/upskillCreation/step1_addAssistant.png)












<br/>
### Step 2 - Sessions Information
![Session Info Diagram](../../../../../static/img/integration/vision/upskillCreation/step2_sessionInfo.png)
| <div align="center">Properties</div> | <div align="center">Description</div> | <div align="center">Note</div> |
|:-------------------------------------|:--------------------------------------| :----------------------------- |
| **Date Range**             | Display the start date and end date of the course which is determined by first and last session's date.                                          - |
| **Rewards By Session / Completion**                           | Determine whether the reward is calculated **by session** or **by completion**.<br/><br/> **By Completion**<br/> - Rewards are issued when participants achieve full attendance across all sessions (100% attendance).<br/><br/>**By Session**<br/>- Rewards are issued once participants attend any session. | **On:**<br/>Rewards calculate by session.<br/><br/>**Off:**<br/>Rewards calculate by completion.<br/><br/>To know more about rewards type, [<u>click here</u>](../introduction#rewards-type)|
| **Session (Dropdown)**| The details of each session of the course.                           | - |
| **Add**           | Add more sessions to the course.                                                     | - |
| **Back**                | Navigate back to the previous page.                                                   | - |
| **Next**                 | Navigate to the next page.                                                           | - |

<br/>
#### Session Details
![Session Details Diagram](../../../../../static/img/integration/vision/upskillCreation/step2_sessionInfoDetail.png)
| <div align="center">Properties</div> | <div align="center">Description</div>| <div align="center">Required</div>| <div align="center">Note</div> |
|:--------------------------|:--------------------------------------|:-:|:------------------------------------|
| **Title**           | The title of the session.             | ✓ | - |
| **Description**     | A detailed description of the session.| ✗ | - |
| **Date**            | The date of the session.              | ✓ | - |
| **Start Time**      | The start time of the session.        | ✓ | - |
| **End Time**        | The end time of the session.          | ✓ | Cannot be earlier than start time |
| **Venue**           | The venue of the session.             | ✗ | - |












<br/>
### Step 3 - Rewards Information

![Rewards Info Diagram](../../../../../static/img/integration/vision/upskillCreation/step3_rewardInfo.png)

| <div align="center">Properties</div> | <div align="center">Description</div>     | Required | <div align="center">Note</div> |
|:-------------------------------------|:------------------------------------------|:--------:|:----|
| **Session Rewards**              | **Completion-based course:** There is only **one** completion reward for the entire course.<br/><br/>**Session-based course:** There are **multiple** session rewards. Each session will have their respective session rewards. | ✗        | Default reward is "0".   |
| **Payment by**                   | Type of payment method for this course.<br/>This payment method only applicable for cash only,  coins will be paid immediately upon entitlement.     | ✓        | Same concept as in task creation's payment by, [<u>click here</u>](../../task/manager_view/task_creation/assignment#payment-by)   |
| **Bonus Rewards**                | Extra criterias that employee can achieve to earn more rewards.             | ✗        | Default reward is "0".<br/><br/>If a value is specified in cash or coins, the bonus criteria must be provided.<br/><br/>Same concept as in task creation's bonus, [<u>click here</u>](../../task/manager_view/task_creation/assignment#bonus)   |
| **Clear**                        | Clears all rewards on the current page.   | -        |        **Manager:**<br/>Clears all rewards.<br/><br/>**Tutor Assistants:**<br/>No clear button as they cannot edit rewards.|
| **Back**                         | Navigate to the previous page.           | -        | -   |  
| **Next**                         | Navigate to the next page.               | -        | -   |  

<br/>
#### Session rewards
- **Completion-based course:** There is only **one** completion reward for the entire course.
- **Session-based course:** There are **multiple** session rewards. Each session will have their respective session rewards. 

![Rewards Info Diagram](../../../../../static/img/integration/vision/upskillCreation/step3_sessionReward.png)










<br/>
### Step 4 - Participants Information
![Participant Info Diagram](../../../../../static/img/integration/vision/upskillCreation/step4_ParticipantInfo.png)
| <div align="center">Properties</div> | <div align="center">Description</div> | <div align="center">Note</div> |
|:-----------------------------|:-----------------------------------------------------------------------------------|:---------|
| **Is Public**     | Determine whether this course is public or private. | **On:**<br/>Public course.<br/><br/>**Off:**<br/>Private course.<br/><br/>To know more about public and private course, [<u> click here</u>](../introduction#course-privacy).
| **Filter Icon**        | Filter and sort the employee list.                                             | By branch, department & HR group. |
| **Select All**    | Select all employees as participants.                                                         | Can press again to deselect all employees. |
| **Available Slots**        | The available slots left for this course (Number of selected participants / maximum pax).                                                           |As this is **private** course, so there is **no maximum pax**, hence the maximum pax is "-".|
| **Selected Employees** (With tick)     | All employees in the companies that **participate** in this course.                            |  Click to **remove** employee from course.<br/><br/>Selected participants cannot be removed when the course has started (ongoing). |
| **Unselected Employees** (Without tick)        | All employees in the companies that **does not participate** in this course.                                                                        |Click to **add** employee to course.|
| **Back**          | Navigate back to the previous page.                                                          | - |
| **Save**        | Create or edit the course.                                                                            | - |

<br/>
#### Is Public

**Public course**
- A public course is visible to participants in specific branches, departments, or HR groups as set by the manager.  
- It allows eligible **participants to register** on their own.  

**Private course**
- A private course is not open for general registration. 
- Instead, participants are manually **added by the manager**.  
- Only those who are added to the course can view it in the course tab.  

:::info[Note]
If the is public switch is on, the maximum pax, branch, department and HR group fields are required.
:::

:::tip
If a course is public, the manager can manually add participants who do not belong to the specified branches, departments, or HR groups.
:::

![Public Switch Diagram](../../../../../static/img/integration/vision/upskillCreation/step4_IsPublic.png)














## Edit Course
- The diagram below illustrates the **manager's** and **tutor assistants'** edit permissions based on the different course statuses.
- To know more about course status, [<u>click here</u>](../introduction#course-status).

:::info[Note]
Tutor and assistants cannot edit any rewards-related field.
:::

#### **Manager:**  

![Manager Edit Course Diagram](../../../../../static/img/integration/vision/upskillCreation/editCourse_mgr.png)

#### **Tutor & Assistants:** 

![Tutor Assistant Edit Course Diagram](../../../../../static/img/integration/vision/upskillCreation/editCourse_tutorAsst.png)


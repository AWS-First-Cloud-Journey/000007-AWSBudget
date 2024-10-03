---
title : "Create Usage Budget"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

#### Creating a Usage Budget in AWS

In this section, you will practice creating a Usage Budget.

> **Note:** If you've previously gone through the process of creating a [Cost Budget](../1-cost-budgets), you'll find that the steps for creating a Usage Budget are quite similar. The main distinction is that Cost Budget focuses on **cost**, while Usage Budget focuses on **usage**.

#### Table of Contents
- [Creating a Usage Budget in AWS](#creating-a-usage-budget-in-aws)
      - [Table of Contents](#table-of-contents)
  - [Create usage budget](#create-usage-budget)

#### Create usage budget

1. Log in to the **AWS Management Console** admin page and select the **Billing and Cost Management** service using the search bar.

   ![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

2. On the admin page, click on **Budgets**.

   ![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

3. Choose **Create budget**.

   ![Budget Name & Amount](/images/3/00001.png?featherlight=false&width=90pc)

4. Select the **Budget type**:

   - Choose **Customize**
   - Choose **Usage budget**

   ![Budget Name & Amount](/images/3/0002.png?featherlight=false&width=90pc)

5. Provide a name for your budget.

   ![Budget Name & Amount](/images/3/0003.png?featherlight=false&width=90pc)

6. Select **Use type groups**:

   - Choose **EC2:Running Hours**

   ![Budget Name & Amount](/images/3/0004.png?featherlight=false&width=90pc)

7. Set the budget amount:

   - Select a **Period**
   - Choose a **Budget renewal type**
   - Select a **Budgeting method**
   - Enter the number of hours.

   ![Budget Name & Amount](/images/3/0005.png?featherlight=false&width=90pc)

8. Keep the default settings and click **Next**.

   ![Budget Name & Amount](/images/3/0006.png?featherlight=false&width=90pc)

9. Configure the **Alert**:

   ![Budget Name & Amount](/images/3/0007.png?featherlight=false&width=90pc)

10. Provide complete information for the **Alert**:

    ![Budget Name & Amount](/images/3/0008.png?featherlight=false&width=90pc)

11. Click **Next**.

    ![Budget Name & Amount](/images/3/0009.png?featherlight=false&width=90pc)

12. Click **Create budget**.

    ![Budget Name & Amount](/images/3/00010.png?featherlight=false&width=90pc)

13. Your budget has been successfully created.

    ![Budget Name & Amount](/images/3/00011.png?featherlight=false&width=90pc)

14. Check the **Budget health**:

    ![Budget Name & Amount](/images/3/00012.png?featherlight=false&width=90pc)

15. Review the **Budget history**:

    ![Budget Name & Amount](/images/3/00013.png?featherlight=false&width=90pc)
    ![Budget Name & Amount](/images/3/000131.png?featherlight=false&width=90pc)


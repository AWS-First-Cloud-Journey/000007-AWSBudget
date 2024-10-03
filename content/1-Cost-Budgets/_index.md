---
title : "Create Cost Budget"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

#### Create Cost Budget Tutorial

In this section, you will practice creating a **Cost Budget**.

#### Create Cost Budget

New accounts can only create the *Cost Budget* section; subsequent sections can be skipped.

1. Log in to the **AWS Management Console** admin page and select the **Billing and Cost Management** service in the search bar.

2. In the admin page, select **Budgets**.

3. Select **Create budget**.

   ![Billing Service](/images/2/0001.png?featherlight=false&width=90pc)

4. For **Budget setup**:

   - Select **Customize**
   - **Budget types**: select **Cost budget**
   - Select **Next**

   ![Billing Service](/images/2/0002.png?featherlight=false&width=90pc)

   ![Billing Service](/images/2/00021.png?featherlight=false&width=90pc)

5. In the **Set your budget** interface:

   - For **Budget name**, enter **`Monthly`**

   ![Billing Service](/images/2/0003.png?featherlight=false&width=90pc)

   - **Period**: select the time period for Budget by Day (*Daily*), Month (*Monthly*), Quarter (*Quarterly*), and Year (*Annually*)
   - **Budget effective dates**:
       - Select **Recurring Budget** if you want this Budget to be repeated periodically
       - Select **Expiring Budget** if you only want the Budget to be booked only once.
       - All time zones are **UTC**.
   - Section **Specify your monthly budget**:
       - Choose **Fixed** if you want the budget of each term to be the same
       - Choose **Monthly Budget Planning** if you want the budget of each term to be different
       - **Budgeted amount**: enter the amount corresponding to your budget.
           - **Note**: if you select **Monthly Budget Planning**, you will have to enter a budgeted amount for each term.

   ![Billing Service](/images/2/0004.png?featherlight=false&width=90pc)

6. For **Budget scope**, select **All AWS services**. Then select **Next**

   ![Create Cost Budget](/images/2/0005.png?featherlight=false&width=90pc)

7. For **Configure alerts**, select **Add an alert threshold**. Select **Next**

   ![Create Cost Budget](/images/2/0006.png?featherlight=false&width=90pc)

8. Configure **Alert** and select **Next**

   ![Create Cost Budget](/images/2/0007.png?featherlight=false&width=90pc)

9. Select **Next**

   ![Create Cost Budget](/images/2/0008.png?featherlight=false&width=90pc)

10. Select **Create budget**

    ![Create Cost Budget](/images/2/0009.png?featherlight=false&width=90pc)

11. Create a successful budget.

    ![Create Cost Budget](/images/2/00010.png?featherlight=false&width=90pc)

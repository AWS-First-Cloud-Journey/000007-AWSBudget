---
title : "Create Cost Budget"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2. </b> "
---

#### Overview

In this section, you will learn how to create and configure an AWS Cost Budget to monitor and manage your AWS spending effectively.

{{% notice info %}}
**ℹ️ Information**: Cost Budgets are the most common type of AWS Budget, allowing you to set thresholds for your AWS spending and receive alerts when costs exceed or are forecasted to exceed your defined limits.
{{% /notice %}}

#### Creating a Cost Budget

1. Sign in to the **AWS Management Console** and search for **AWS Billing and Cost Management** in the services search bar.

2. In the navigation pane, select **Budgets**.

3. Click **Create budget**.

   ![AWS Billing Service](/images/2/0001.png?featherlight=false&width=90pc)

4. Configure your **Budget setup**:

   - Select **Customize (advanced)** for more control over your budget settings
   - Under **Budget types**, select **Cost budget**
   - Click **Next**

   ![Budget Setup Options](/images/2/0002.png?featherlight=false&width=90pc)

   ![Cost Budget Selection](/images/2/00021.png?featherlight=false&width=90pc)

5. In the **Set your budget** section:

   - Enter a descriptive **Budget name** (e.g., **`Monthly`**)

   ![Budget Naming](/images/2/0003.png?featherlight=false&width=90pc)

   - For **Period**, select the appropriate time interval:
     - **Daily** for day-to-day monitoring
     - **Monthly** for month-to-month tracking (most common)
     - **Quarterly** for quarterly oversight
     - **Annually** for yearly budget management
   
   - Under **Budget effective dates**:
     - Select **Recurring Budget** if you want this budget to continue indefinitely
     - Select **Expiring Budget** if you need a one-time budget for a specific timeframe
     - Note that all time zones are in **UTC**
   
   - In the **Specify your monthly budget** section:
     - Choose **Fixed** to set the same budget amount for each period
     - Choose **Monthly Budget Planning** to set different amounts for each period
     - Enter your **Budgeted amount** in your preferred currency

   ![Budget Configuration](/images/2/0004.png?featherlight=false&width=90pc)

6. For **Budget scope**, select **All AWS services** to monitor your entire AWS spending, then click **Next**.

   {{% notice tip %}}
   **💡 Pro Tip**: For more granular tracking, you can filter budgets by specific services, linked accounts, tags, or cost categories. This is especially useful for large organizations with multiple projects or departments.
   {{% /notice %}}

   ![Budget Scope Selection](/images/2/0005.png?featherlight=false&width=90pc)

7. In the **Configure alerts** section, click **Add an alert threshold**, then click **Next**.

   ![Adding Alert Threshold](/images/2/0006.png?featherlight=false&width=90pc)

8. Configure your alert settings:
   - Set the threshold percentage (e.g., 80% of actual or forecasted spend)
   - Add email recipients who should receive notifications
   - Optionally, configure an Amazon SNS topic for programmatic notifications
   - Click **Next**

   ![Alert Configuration](/images/2/0007.png?featherlight=false&width=90pc)

9. Review the budget actions settings and click **Next**.

   {{% notice info %}}
   **ℹ️ Information**: Budget actions allow you to configure automated responses when a budget threshold is reached, such as applying an IAM policy or targeting specific EC2 or RDS instances.
   {{% /notice %}}

   ![Budget Actions Review](/images/2/0008.png?featherlight=false&width=90pc)

10. Review your budget configuration and click **Create budget**.

    ![Create Budget Confirmation](/images/2/0009.png?featherlight=false&width=90pc)

11. Verify that your budget has been created successfully.

    ![Budget Creation Success](/images/2/00010.png?featherlight=false&width=90pc)

{{% notice warning %}}
**⚠️ Warning**: AWS Budgets relies on billing data that updates approximately every 8-12 hours. There may be a delay between when costs are incurred and when alerts are triggered. For the most critical workloads, consider setting conservative thresholds to account for this delay.
{{% /notice %}}

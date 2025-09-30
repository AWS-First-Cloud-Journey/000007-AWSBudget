---
title : "Create Usage Budget"
date : 2025-09-30
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

#### Overview

In this section, you will learn how to create and configure an AWS Usage Budget to monitor the consumption of specific AWS services based on usage metrics rather than cost.

ℹ️ **Information**: While Cost Budgets track your AWS spending in monetary terms, Usage Budgets monitor the actual consumption of AWS resources, such as EC2 compute hours, S3 storage, or data transfer volumes.

#### Creating a Usage Budget

1. Sign in to the **AWS Management Console** and search for **AWS Billing and Cost Management** in the services search bar.


![AWS Billing Console](/images/3/abc.png?featherlight=false&width=90pc)


2. In the navigation pane, select **Budgets**.

![Budgets Navigation](/images/3/00001.png?featherlight=false&width=90pc)

3. Click **Create budget**.

![Create Budget Button](/images/3/00001.png?featherlight=false&width=90pc)

4. Configure your **Budget setup**:
   - Select **Customize (advanced)** for more control over your budget settings
   - Under **Budget types**, select **Usage budget**
   - Click **Next**

![Budget Setup Options](/images/3/00002.png?featherlight=false&width=90pc)

5. In the **Details** section, enter a descriptive name for your budget.

![Budget Name Configuration](/images/3/00003.png?featherlight=false&width=90pc)

6. For **Usage type**, select **Use type groups**:
   - Choose **EC2:Running Hours** from the dropdown menu
   
💡 **Pro Tip**: Selecting a specific usage type group allows you to focus on monitoring particular AWS resources that are most important to your workloads.

![Usage Type Selection](/images/3/00004.png?featherlight=false&width=90pc)

7. Configure your **Budget parameters**:
   - Select a **Period** (Monthly, Quarterly, or Annually)
   - Choose a **Budget renewal type** (Recurring or Expiring)
   - Select a **Budgeting method** (Fixed or Planned)
   - Enter your budgeted usage amount in hours

![Budget Parameters Configuration](/images/3/00005.png?featherlight=false&width=90pc)

8. Review the **Budget scope** settings and click **Next**.

![Budget Scope Review](/images/3/00006.png?featherlight=false&width=90pc)

9. In the **Configure alerts** section, click **Add an alert threshold**.

![Add Alert Threshold](/images/3/00007.png?featherlight=false&width=90pc)

10. Configure your alert settings:
    - Set the **Threshold** percentage
    - Choose **Actual** or **Forecasted** for the alert type
    - Add email recipients who should receive the alert notifications
    - Optionally, configure an Amazon SNS topic for additional notification options

⚠️ **Warning**: Usage alerts are based on billing data that updates approximately every 8-12 hours. There may be a delay between when usage occurs and when alerts are triggered.

![Alert Configuration](/images/3/00008.png?featherlight=false&width=90pc)

11. After configuring your alert, click **Next**.

![Next Button](/images/3/00009.png?featherlight=false&width=90pc)

12. Review your budget configuration and click **Create budget** to finalize.

![Create Budget Confirmation](/images/3/000010.png?featherlight=false&width=90pc)

13. You will see a confirmation message that your budget has been successfully created.

![Budget Creation Success](/images/3/000011.png?featherlight=false&width=90pc)

#### Monitoring Your Usage Budget

14. After creation, you can monitor your budget's health in the **Budget details** view:

![Budget Health Monitoring](/images/3/000012.png?featherlight=false&width=90pc)

15. To analyze usage trends over time, navigate to the **Budget history** tab:

![Budget History Tab](/images/3/000013.png?featherlight=false&width=90pc)

![Budget History Details](/images/3/000131.png?featherlight=false&width=90pc)

💡 **Pro Tip**: Regularly review your usage patterns in the Budget history to identify trends and optimize your resource allocation. Consider setting up multiple usage budgets for different services to gain comprehensive visibility into your AWS consumption.

🔒 **Security Note**: Ensure that only authorized personnel have access to budget information, as it can reveal details about your infrastructure scale and resource allocation.

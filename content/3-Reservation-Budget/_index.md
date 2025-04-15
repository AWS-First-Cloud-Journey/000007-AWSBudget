+++
title = "Create RI Budget"
date = 2024
weight = 4
chapter = false
pre = " <b> 4. </b> "
+++

#### Overview

In this section, you will learn how to create and configure an AWS Reservation Budget to monitor the utilization and coverage of your Reserved Instances (RIs).

ℹ️ **Information**: Reserved Instances provide significant discounts (up to 72%) compared to On-Demand pricing when you commit to a one-year or three-year term for specific AWS resources like EC2 instances, RDS databases, or ElastiCache nodes.

⚠️ **Warning**: This lab is for instructional purposes only. You will not actually purchase a Reserved Instance during this lab since it requires an upfront commitment. The steps below demonstrate the budget creation process without requiring any financial commitment.

#### Creating a Reservation Budget

1. Sign in to the **AWS Management Console** and search for **AWS Billing and Cost Management** in the services search bar.

![Billing Service](/images/4/0001.png?featherlight=false&width=90pc)

2. In the navigation pane, select **Budgets**.

![Budgets](/images/4/0001.png?featherlight=false&width=90pc)

3. Click **Create budget**.

![Create Budget](/images/4/00001.png?featherlight=false&width=90pc)

4. Configure your **Budget setup**:
   - Select **Customize (advanced)** for more control over your budget settings
   - Under **Budget types**, select **Reservation budget**
   - Click **Next**

![Budget Setup](/images/4/0002.png?featherlight=false&width=90pc)

5. In the **Details** section, enter a descriptive name for your budget.

![Budget Setup](/images/4/0003.png?featherlight=false&width=90pc)

6. Configure the **Coverage threshold** for your budget:
   - Set the percentage threshold that will trigger an alert when your RI coverage falls below this value
   - RI coverage represents the percentage of eligible instance usage that is covered by Reserved Instances

💡 **Pro Tip**: A higher coverage threshold (e.g., 80%) will alert you earlier when your workloads aren't fully covered by RIs, helping you maximize cost savings by purchasing additional RIs when needed.

![Coverage Threshold](/images/4/0008.png?featherlight=false&width=90pc)

7. Configure your **Alert settings**:
   - Add email recipients who should receive the alert notifications
   - Optionally, configure an Amazon SNS topic for additional notification options

![Alert Settings](/images/4/0006.png?featherlight=false&width=90pc)

8. Review your budget configuration and click **Create budget**.

![Create Budget](/images/4/0007.png?featherlight=false&width=90pc)

9. Verify that your budget has been created successfully.

![Budget Creation](/images/4/0009.png?featherlight=false&width=90pc)

10. Review your budget in the budgets dashboard to monitor RI coverage over time.

![Budget Overview](/images/4/00010.png?featherlight=false&width=90pc)

ℹ️ **Information**: AWS Budgets provides two types of RI budgets: RI utilization budgets (tracking how much of your purchased RIs are being used) and RI coverage budgets (tracking what percentage of your eligible usage is covered by RIs). The example above demonstrates an RI coverage budget.

🔒 **Security Note**: Consider implementing AWS Organizations and consolidated billing to maximize the benefits of Reserved Instances across multiple accounts in your organization.

+++
title = "Create Savings Plans Budget"
date = 2024
weight = 5
chapter = false
pre = " <b> 5. </b> "
+++

#### Overview

In this section, you will learn how to create and configure an AWS Savings Plans Budget to monitor the utilization and coverage of your Savings Plans commitments.

ℹ️ **Information**: Savings Plans provide significant discounts (up to 72%) compared to On-Demand pricing when you commit to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term. AWS offers Compute Savings Plans, EC2 Instance Savings Plans, and SageMaker Savings Plans.

⚠️ **Warning**: This lab is for instructional purposes only. You will not actually purchase a Savings Plan during this lab since it requires a financial commitment. The steps below demonstrate the budget creation process without requiring any financial commitment.

#### Creating a Savings Plans Budget

1. Sign in to the **AWS Management Console** and search for **AWS Billing and Cost Management** in the services search bar.

![Billing Service](/images/5/z0001.png?featherlight=false&width=90pc)

2. In the navigation pane, select **Budgets**.

![Budgets](/images/5/x00001.png?featherlight=false&width=90pc)

3. Click **Create budget**.

![Create Budget](/images/5/x00001.png?featherlight=false&width=90pc)

4. Configure your **Budget setup**:
   - Select **Customize (advanced)** for more control over your budget settings
   - Under **Budget types**, select **Savings Plans budget**
   - Click **Next**

![Billing Service](/images/5/z0002.png?featherlight=false&width=90pc)

![Billing Service](/images/5/z00002.png?featherlight=false&width=90pc)

5. In the **Details** section, enter a descriptive name for your budget.

![Budget Name](/images/5/z0003.png?featherlight=false&width=90pc)

6. Configure the **Coverage threshold** for your budget:
   - Set the percentage threshold that will trigger an alert when your Savings Plans coverage falls below this value
   - Savings Plans coverage represents the percentage of eligible usage that is covered by your Savings Plans commitments

💡 **Pro Tip**: A higher coverage threshold (e.g., 80%) will alert you earlier when your workloads aren't fully covered by Savings Plans, helping you maximize cost savings by purchasing additional commitments when needed.

![Threshold Configuration](/images/5/z0004.png?featherlight=false&width=90pc)

7. Configure your **Alert settings**:
   - Add email recipients who should receive the alert notifications
   - Optionally, configure an Amazon SNS topic for additional notification options

![Alert Configuration](/images/5/z0005.png?featherlight=false&width=90pc)

8. Review your budget configuration and click **Create budget**.

![Create Budget](/images/5/z0006.png?featherlight=false&width=90pc)

9. Verify that your budget has been created successfully.

![Budget Creation Successful](/images/5/z0007.png?featherlight=false&width=90pc)

10. Review your budget in the budgets dashboard to monitor Savings Plans coverage over time.

![Budget Details](/images/5/z0008.png?featherlight=false&width=90pc)

ℹ️ **Information**: AWS Budgets provides two types of Savings Plans budgets: utilization budgets (tracking how much of your purchased Savings Plans are being used) and coverage budgets (tracking what percentage of your eligible usage is covered by Savings Plans). The example above demonstrates a Savings Plans coverage budget.

🔒 **Security Note**: Consider implementing AWS Organizations and consolidated billing to maximize the benefits of Savings Plans across multiple accounts in your organization.

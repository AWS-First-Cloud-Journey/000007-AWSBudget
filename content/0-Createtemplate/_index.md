+++
title = "Create Budget by Template"
date = 2024
weight = 2
chapter = false
pre = " <b> 2. </b> "
+++

#### Overview

In this section, you will learn how to quickly create an AWS Budget using the pre-configured templates provided by AWS. Templates offer a simplified approach to budget creation with recommended settings for common use cases.

#### Creating a Budget Using Templates

1. Access the **AWS Management Console** and navigate to **AWS Billing and Cost Management**:
   - Sign in to the [AWS Console](https://ap-southeast-1.console.aws.amazon.com/console/home?region=ap-southeast-1)
   - Search for and select **Billing and Cost Management** in the services search bar

![AWS Billing Console](/images/1/0001.png?featherlight=false&width=90pc)

2. Navigate to the Budgets section:
   - In the left navigation pane, select **Budgets**
   - Click the **Create a budget** button

![Create Budget](/images/1/0002.png?featherlight=false&width=90pc)

3. Select the template option for budget setup:
   - Choose **Use a template (simplified)**
   - From the available templates, select **Monthly cost budget**

![Budget Template Selection](/images/1/0003.png?featherlight=false&width=90pc)

4. Configure your budget settings:
   - Enter a descriptive name for your budget
   - Set your monthly budget amount
   - Review the email recipients for alerts
   - Click **Create budget** to finalize

![Budget Configuration](/images/1/0004.png?featherlight=false&width=90pc)
![Budget Alert Settings](/images/1/00041.png?featherlight=false&width=90pc)

ℹ️ **Information**: The monthly cost budget template automatically configures alerts at 80% of actual spend and 110% of forecasted spend, helping you stay informed about both current and potential future costs.

5. Verify your budget has been created successfully:
   - You should see a confirmation message
   - Your new budget will appear in the budgets list

![Budget Created Successfully](/images/1/0005.png?featherlight=false&width=90pc)

#### Monitoring Your Budget

6. View your budget history:
   - Select your newly created budget
   - Navigate to the **Budget history** tab to see historical performance

![Budget History Tab](/images/1/00060.png?featherlight=false&width=90pc)

![Budget History Details](/images/1/0006.png?featherlight=false&width=90pc)

7. Review the budget overview:
   - The overview provides a snapshot of your current spending against your budget
   - Visual indicators show your budget status at a glance

![Budget Overview](/images/1/0008.png?featherlight=false&width=90pc)

8. Monitor budget health and alerts:
   - Check the **Budget health** section to see your current status
   - Review any active alerts that have been triggered

![Budget Health](/images/1/0005.png?featherlight=false&width=90pc)

9. Return to the budget history for trend analysis:
   - Historical data helps identify spending patterns over time
   - Use this information to refine future budgets

![Budget History Navigation](/images/1/00060.png?featherlight=false&width=90pc)

![Budget History Trends](/images/1/0006.png?featherlight=false&width=90pc)

10. Understand the template alert configuration:
    - Review the alert thresholds and notification settings
    - Note how the template has configured both actual and forecasted alerts

![Budget Alert Configuration](/images/1/00011.png?featherlight=false&width=90pc)

💡 **Pro Tip**: While templates provide a quick start, consider creating customized budgets for specific projects or departments using tags. This allows for more granular cost tracking and accountability across your organization.

⚠️ **Warning**: Budget alerts are based on billing data that updates approximately every 8-12 hours. There may be a delay between when costs are incurred and when alerts are triggered.

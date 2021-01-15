+++
title = "Create Cost Budget"
date = 2020-04-18T00:38:32+07:00
weight = 1
chapter = false
pre = "<b>1. </b>"
+++

**Contents:**
- [Create your cost budget](#create-your-cost-budget)

#### Create your cost budget

1. Go to the AWS Management Console and open the Billing and Cost Management console at **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)** home page.
2. In the navigation pane, choose **Budgets**.
3. At the top of the page, choose **Create budget**.
4. For **Select budget type**, choose **Cost budget**.
5. Choose **Set your budget**.
6. For **Name**, enter the name of your budget.
7. For **Period**, choose how often you want the budget to reset the actual and forecasted spend. Choose **Monthly** for every month, **Quarterly** for every three months, and **Annually** for every year.
8. For a fixed **Budgeted Amount**, enter the total amount that you want to spend for this budget period.
9. (Optional) For **Budget effective dates**, choose **Recurring Budget** for a budget that resets after the budget period or **Expiring Budget** for a one-time budget that doesn't reset after the budget period.  
    All budget times are in UTC.

![Create Cost Budget](/images/4-budget/CostBudget/Cost-Budget-1.PNG?width=90pc)

10.  (Optional) Under **Budget parameters (optional)**, for **Filtering**, choose one or more of the [available filters](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html). Your choice of budget type determines the set of filters that is displayed on the console.
11.  (Optional) Under Budget parameters (optional), for Advanced options, choose one or more of the following filters. If you are signed in from a member account in an organization instead of from a master account, you might not see all of the advanced options.

![Create Cost Budget](/images/4-budget/CostBudget/Cost-Budget-2.PNG?width=90pc)

12.  Choose **Configure alerts**.
13.  Under **Configure alerts**, for **Alert 1**, choose **Actual** to create a notification for actual spend and **Forecast** to create a notification for your forecasted spend.
14.  For **Alert threshold**, enter the amount that you want to be notified at. This can be either an absolute value or a percentage. For example, for a budget of 200 dollars, if you want to be notified at 160 dollars (80% of your budget), enter 160 for an absolute budget or 80 for a percentage budget.  
15.  For **Email contacts**, enter the email addresses that you want the notifications to be sent to and choose **Add email contact**. Separate multiple email addresses with a comma. A notification can have up to 10 email addresses.  
16.  (Optional) For **SNS topic ARN**, enter the ARN for your Amazon SNS topic and then choose **Verify**. If you want to use an Amazon SNS topic for your notification but don't have one, see [Create a Topic](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html) in the *Amazon Simple Notification Service Developer Guide*.  
17.  Choose **Confirm budget**.

![Configure Alert](/images/4-budget/CostBudget/Cost-Budget-3.PNG?width=90pc)

18. Review your budget settings, and choose **Create**.

![Review](/images/4-budget/CostBudget/Cost-Budget-4.PNG?width=90pc)


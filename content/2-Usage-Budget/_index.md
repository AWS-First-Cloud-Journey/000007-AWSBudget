+++
title = "Create Usage Budget"
date = 2020-04-18T00:38:32+07:00
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

**Contents:**
- [Create your usage budget](#create-your-usage-budget)

#### Create your usage budget

1. Go to the AWS Management Console and open the Billing and Cost Management console at **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)** home page.
2. In the navigation pane, choose **Budgets**.
3. At the top of the page, choose **Create budget**.
4. For **Select budget type**, choose **Usage budget**.
5. Choose **Set up your budget**.
6. For **Name**, enter the name of your budget.
7. For **Period**, choose how often you want the budget to reset the actual and forecasted usage. Choose **Monthly** for every month, **Quarterly** for every three months, or **Annually** for every year.
8. Under **Usage unit(s)**, choose either **Usage Type Group** or **Usage Type**. A usage type group is a collection of usage types that have the same unit of measure, such as resources that measure usage by the hour.
    + For **Usage Type Group**, choose the unit of measurement that you want the budget to use.
    + For **Usage Type**, choose the service that you want to include in the budget and then choose the unit of measurement that you want the budget to use.
9. For a fixed **Budgeted Amount**, enter the total amount of units that you want to use for this budget period. For **Monthly** and **Quarterly** Planning budgets, enter the amount you want to spend for each planned period.
10. (Optional) For **Budget effective dates**, choose **Recurring Budget** for a budget that resets after the budget period or **Expiring Budget** for a one-time budget that doesn't reset after the budget period.   
    All budget times are in UTC.

![Create Usage Budget](/images/4-budget/UsageBudget/usage-budget-1.PNG?width=90pc)
11.  (Optional) Under **Budget parameters (optional)**, for **Filtering**, choose one or more of the [available filters](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html). Your choice of budget type determines the set of filters that is displayed on the console.  

{{% notice note %}}
You must choose **Usage Type**, **Usage Type Group**, or both. You can create a usage budget for only one specific unit of measure at a time such as gigabyte (GB), gigabyte per month (GB-Month), hours (Hrs), or number of requests.
{{% /notice %}}

![Create Usage Budget](/images/4-budget/UsageBudget/usage-budget-2.PNG?width=90pc)

12. Choose **Configure alerts**.
13. Under **Configure alerts**, for **Alert 1**, choose **Actual** to create a notification for actual spend and **Forecast** to create a notification for your forecasted spend.
14. For **Alert threshold**, enter the amount that you want to be notified at. This can be either an absolute value or a percentage. For example, for a budget of 200 dollars, if you want to be notified at 160 dollars (80% of your budget), enter "160" for an absolute budget or "80" for a percentage budget. 
15. (Optional) For **Email contacts**, enter the email addresses that you want the notifications to be sent to and choose **Add email contact**. Separate multiple email addresses with a comma. A notification can have up to 10 email addresses.  
    To receive a notification, you must specify an email address, You can also specify an Amazon SNS topic.
16. (Optional) For **SNS topic ARN**, enter the ARN for your Amazon SNS topic and then choose **Verify**. If you want to use an Amazon SNS topic for your notification but don't have one, see [Create a Topic](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html) in the *Amazon Simple Notification Service Developer Guide*.  
17. Choose **Confirm budget**.

![Configure Alert](/images/4-budget/UsageBudget/usage-budget-3.PNG?width=90pc)

18. Review your budget settings, and choose **Create**.

![Review](/images/4-budget/UsageBudget/usage-budget-4.PNG?width=90pc)


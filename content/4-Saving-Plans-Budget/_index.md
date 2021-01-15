+++
title = "Create Saving Plans Budget"
date = 2020-04-18T00:38:32+07:00
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

**Contents:**
- [Create your saving plans budget](#create-your-saving-plans-budget)

#### Create your saving plans budget

1. Go to the AWS Management Console and open the Billing and Cost Management console at **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)** home page.
2. In the navigation pane, choose **Budgets**.
3. At the top of the page, choose **Create budget**.
4. For **Select budget type**, choose **Savings Plans budget**.
5. Choose **Set up your budget**.
6. For **Name**, enter the name of your budget.
7. For **Period**, choose how often you want the budget to reset the actual and forecasted spend. Choose **Daily** for every day, **Monthly** for every month, **Quarterly** for every three months, or **Annually** for every year.  
   All budget times are in UTC.
8. For **Savings Plans budget type**, choose what you want the budget to track.  
    **Savings Plans Utilization** is how much of your Savings Plans you've used.  
    **Savings Plans Coverage** is how much of your usage a Savings Plan covers.
9.  For **Utilization threshold**, enter the utilization percentage that you want AWS to notify you at. For example, for a utilization budget where you want to stay above 90% Savings Plans utilization, enter 90, and the budget notifies you when your overall Savings Plans utilization goes below 90%.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-1.PNG?width=90pc)

10. (Optional) Under **Budget parameters (optional)**, for **Filtering**, choose one or more of the [available filters](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html). Your choice of budget type determines the set of filters that is displayed on the console.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-2.PNG?width=90pc)

11. Choose **Configure alerts**. You can configure one alert only for a Savings Plans budget.
12. (Optional) For **Email contacts**, enter the email addresses that you want the notifications to be sent to and choose **Add email contact**. Separate multiple email addresses with a comma. A notification can have up to 10 email addresses.  
    To receive a notification, you must specify an email address, You can also specify an Amazon SNS topic.
13. (Optional) For **SNS topic ARN**, enter the ARN for your Amazon SNS topic and then choose **Verify**. If you want to use an Amazon SNS topic for your notification but don't have one, see [Create a Topic](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html) in the *Amazon Simple Notification Service Developer Guide*.  
14. Choose **Confirm budget**.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-3.PNG?width=90pc)

15. Review your budget settings, and choose **Create**.

![Create Reservation Budget](/images/4-budget/SavingPlansBudget/savingplansbudget-4.PNG?width=90pc)

+++
title = "Create Reservation Budget"
date = 2020-04-18T00:38:32+07:00
weight = 3
chapter = false
pre = "<b>3. </b>"
+++

**Contents:**
- [Create Reservation Budget](#create-reservation-budget)

#### Create Reservation Budget

1. Go to the AWS Management Console and open the Billing and Cost Management console at **[Amazon Web Services](https://console.aws.amazon.com/billing/home?#/budgets)** home page.
2. In the navigation pane, choose **Budgets**.
3. At the top of the page, choose **Create budget**.
4. For **Select budget type**, choose **Reservation budget**.
5. Choose **Set your budget**.
6. For **Name**, enter the name of your budget.
7. For **Period**, choose how often you want the budget to reset the actual and forecasted spend. Choose **Daily** for every day, **Monthly** for every month, **Quarterly** for every three months, or **Annually** for every year.  
   All budget times are in UTC.
8. For **Reservation budget type**, choose whether you want the budget to track **RI Utilization** or **RI Coverage**.  
9.  For **Service**, choose the service whose instances you want the budget to track.
10. For **Utilization threshold**, enter the utilization or coverage percentage that you want AWS to notify you at. For example, for a utilization budget where you want to stay above 80% RI utilization, enter 80, and the budget notifies you when you go below 80% utilization. For a coverage budget where you want to make sure that you stay above 80%, enter 80, and the budget notifies you when your instance coverage goes below 80%.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-1.PNG?width=90pc)

11. (Optional) Under **Budget parameters (optional)**, for **Filtering**, choose one or more of the [available filters](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create-filters.html). Your choice of budget type determines the set of filters that is displayed on the console.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-2.PNG?width=90pc)

12. Choose **Configure alert**. You can configure only one alert for a reservation budget.
13. (Optional) Under **Configure alert**, for **Email contacts**, enter the email addresses that you want the notifications to be sent to and then choose **Add email contact**. Separate multiple email addresses with a comma. A notification can have up to 10 email addresses.  
    To receive a notification, you must specify an email address, You can also specify an Amazon SNS topic.
14. (Optional) For **SNS topic ARN**, select **Notify via Amazon Simple Notification Service (SNS) topic** and then choose **Verify**. If you want to use an Amazon SNS topic for your notification but don't have one, see [Create a Topic](https://docs.aws.amazon.com/sns/latest/dg/sns-tutorial-create-topic.html) in the *Amazon Simple Notification Service Developer Guide*.  
15. Choose **Confirm budget**.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-3.PNG?width=90pc)

16. Review your budget settings, and choose **Create**.

![Create Reservation Budget](/images/4-budget/ReservationBudget/reservation-budget-4.PNG?width=90pc)

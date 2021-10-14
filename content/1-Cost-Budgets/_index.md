+++
title = "Creating a Cost Budget"
date = 2020-04-18T00:38:32+07:00
weight = 1
chapter = false
pre = "<b>1. </b>"
+++

In this section, we will practice creating a Cost Budget.

1. Sign in to the AWS Management Console and open the **Billing and Cost Management console** at https://console.aws.amazon.com/billing/ or type in `billing` into the service search-bar and select the first search result.

![Billing Service](/images/4-budget/CostBudget/2.1.1.png?width=90pc)

2. In the navigation pane, choose **Budgets**.

3. At the top of the page, choose **Create budget**.

![Create Service](/images/4-budget/CostBudget/2.1.2.png?width=90pc)

4. For **Choose budget type**, choose **Cost budget**. Then, choose **Next**. 

![Budget Type](/images/4-budget/CostBudget/2.1.3.png?width=90pc)

5. Under **Set budget amount**, for **Period**, choose how often you want the budget to reset the actual and forecasted spend. Select **Daily** for every day, **Monthly** for every month, **Quarterly** for every three months, or **Annually** for every year. 

{{%notice note %}}
With a **Monthly** or **Quarterly** budget period, you can set custom future budgeted amounts using the budget planning feature. 
{{%/notice%}}

6. For **Budget effective date**, choose **Recurring budget** for a budget that resets after the budget period. Or, choose **Expiring budget** for a one-time budget that doesn't reset after the budget period.

7. Choose the start date or period to begin tracking against your budgeted amount. For an **Expiring budget**, choose the end date or period for the budget to end on.

{{%notice tip %}}
All budget times are in the UTC format.
{{%/notice%}}

8. If your budget period is **Daily** or **Annually**: For **Enter your budgeted amount**, enter the total amount that you want to spend each budget period.

    If your budget period is **Monthly**:

    - For **Choose how to budget**, choose **Fixed** to create a budget that monitors the same amount every month. Or, choose **Monthly budget planning** to specify the amount to monitor each month.

    - For a **Fixed** budget, for **Enter your budgeted amount**, enter the total amount that you want to spend every month. For **Monthly budget planning**, enter the amount that you want to spend for each month.

    If your budget period is **Quarterly**:

    - For **Choose how to budget**, choose **Fixed** to create a budget that monitors the same amount every quarter. Or, choose **Quarterly budget planning** to specify the amount to monitor each quarter.

    - For a **Fixed budget**, for **Enter your budgeted amount**, enter the total amount that you want to spend every quarter. For **Quarterly budget planning**, enter the amount that you want to spend for each quarter.


![Budget Amount](/images/4-budget/CostBudget/2.1.4.png?width=90pc)

9. (Optional) **Under Budget scoping - optional**, for **Filters**, choose **Add filter** to apply one or more of the available filters (such as **region** or **tag**.). Your choice of budget type determines the set of filters that's displayed on the console. 

10. Under **Details**, for **Budget name**, enter the name of your budget. Your budget name must be unique within your account. It can contain A-Z, a-z, spaces, and the following characters:

```text
 _.:/=+-%@
```

11. Choose **Next**. 
    
![Budget Scope](/images/4-budget/CostBudget/2.1.5.png?width=90pc)


12. Choose **Add an alert threshold**.

13. Under **Set alert threshold**, for **Threshold**, enter the amount that's needed to be reached for you to be notified. This can be either an absolute value or a percentage. For example, say you have a budget of 200 dollars. To be notiﬁed at 160 dollars (80% of your budget), enter 160 for an absolute budget or 80 for a percentage budget.

    Next to the amount, choose **Absolute value** to be notiﬁed when your costs exceed the threshold amount. Or, choose **% of budgeted amount** to be notiﬁed when your costs exceed the threshold percentage.

    Next to the threshold, choose **Actual** to create an alert for actual spend. Or, choose **Forecasted** to create an alert for forecasted spend.

14. To get an email alert, enter the email addresses that you want the alert to notify under **Notification preferences**. Separate multiple email addresses with commas. A notification can be sent to a maximum of 10 email addresses.

![Configure alert](/images/4-budget/CostBudget/2.1.6.png?width=90pc)

16. For **Attach actions - Optional**, you can configure an action that AWS Budgets performs on your behalf when the alert threshold is exceeded. We'll not add any actions for now.

![Attach actions](/images/4-budget/CostBudget/2.1.7.png?width=90pc)

17. Choose **Next**.

In practice, you must configure at least one of the following parameters for each alert to proceed:
- An email recipient for notifications
- An Amazon SNS topic for notifications
- A budget action

18. Review your budget settings, and then choose **Create budget**.

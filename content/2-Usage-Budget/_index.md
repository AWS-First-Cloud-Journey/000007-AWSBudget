+++
title = "Creating a Usage Budget"
date = 2020-04-18T00:38:32+07:00
weight = 2
chapter = false
pre = "<b>2. </b>"
+++

In this section, we will practice creating a Usage Budget.

{{% notice note%}}
If you've completed [Creating a Cost Budget](../1-cost-budgets), you'll notice that the process of creating a Usage Budget is very similar, with a single difference being Cost Budget works based on **cost**, while Usage Budget works based on **usage**.
{{% /notice%}}

1. Sign in to the AWS Management Console and open the **Billing and Cost Management console** at https://console.aws.amazon.com/billing/ or type in `billing` into the service search-bar and select the first search result.


![Billing Service](/images/4-budget/CostBudget/2.1.1.png?width=90pc)

2. In the navigation pane, choose **Budgets**.

3. At the top of the page, choose **Create budget**.

![Create Service](/images/4-budget/CostBudget/2.1.2.png?width=90pc)
4. For **Choose budget type**, choose **Usage budget**. Then, choose **Next**. 

![Budget Type](/images/4-budget/UsageBudget/2.2.3.png?width=90pc)

5. Under **Choose what you’re budgeting against**, for **Budget against**, choose **Usage type groups** or **Usage types**. A usage type group is a collection of usage types that have the same unit of measure, such as resources that measure usage by the hour.

    - For **Usage type groups**, choose the unit of measurement and the applicable service usage that you want the budget to monitor.

    - For **Usage types**, choose the specific service usage measurements that you want the budget to monitor.

6. Under **Set budget amount**, for **Period**, choose how often you want the budget to reset the actual and forecasted usage. Select **Daily** for every day, **Monthly** for every month, **Quarterly** for every three months, or **Annually** for every year. 

{{%notice note %}}
With a **Monthly** or **Quarterly** budget period, you can set custom future budgeted amounts using the budget planning feature. 
{{%/notice%}}

7. For **Budget effective date**, choose **Recurring budget** for a budget that resets at the end of each budget period. Or, choose **Expiring budget** for a one-time budget that doesn't reset after the given budget period

8. Choose the start date or period to begin tracking against your budgeted amount. For an **Expiring budget**, choose the end date or period for the budget to end on.

{{%notice tip %}}
All budget times are in the UTC format.
{{%/notice%}}

9. If your budget period is **Daily** or **Annually**: For **Enter your budgeted amount**, enter the total amount that you want to use in each budget period.

    If your budget period is **Monthly**:

    - For **Choose how to budget**, choose **Fixed** to create a budget that monitors the same amount every month. Or, choose **Monthly budget planning** to specify the amount to monitor each month.

    - For a **Fixed** budget, for **Enter your budgeted amount**, enter the total amount that you want to use every month. For **Monthly budget planning**, enter the amount that you want to use for each month.

    If your budget period is **Quarterly**:

    - For **Choose how to budget**, choose **Fixed** to create a budget that monitors the same amount every quarter. Or, choose **Quarterly budget planning** to specify the amount to monitor each quarter.

    - For a **Fixed budget**, for **Enter your budgeted amount**, enter the total amount that you want to use every quarter. For **Quarterly budget planning**, enter the amount that you want to use for each quarter.

![Threshold](/images/4-budget/UsageBudget/2.2.4.png?width=90pc)

10. (Optional) **Under Budget scoping - optional**, for **Filters**, choose **Add filter** to apply one or more of the available filters (such as **region** or **tag**.). Your choice of budget type determines the set of filters that's displayed on the console. 

11. Under **Details**, for **Budget name**, enter the name of your budget. Your budget name must be unique within your account. It can contain A-Z, a-z, spaces, and the following characters:

```text
 _.:/=+-%@
```

12. Choose **Next**. 

![Threshold2](/images/4-budget/UsageBudget/2.2.5.png?width=90pc)

13. Choose **Add an alert threshold**.

14. Under **Set alert threshold**, for **Threshold**, enter the amount that's needed to be reached for you to be notified. This can be either an absolute value or a percentage. For example, say you have a budget of 200 hours. To be notiﬁed at 160 hours (80% of your budget), enter 160 for an absolute budget or 80 for a percentage budget.

    Next to the amount, choose **Absolute value** to be notiﬁed when your usage exceed the threshold amount. Or, choose **% of budgeted amount** to be notiﬁed when your usage exceed the threshold percentage.

    Next to the threshold, choose **Actual** to create an alert for actual usage. Or, choose **Forecasted** to create an alert for forecasted usage.

15. To get an email alert, enter the email addresses that you want the alert to notify under **Notification preferences**. Separate multiple email addresses with commas. A notification can be sent to a maximum of 10 email addresses.


![Configure alerts](/images/4-budget/UsageBudget/2.2.6.png?width=90pc)

16. We will be skipping over budget actions for now. Choose **Next**.

In practice, you must configure at least one of the following parameters for each alert to proceed:
- An email recipient for notifications
- An Amazon SNS topic for notifications
- A budget action

17. Review your budget settings, and then choose **Create budget**.
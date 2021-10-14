+++
title = "Creating a Saving Plans Budget"
date = 2020-04-18T00:38:32+07:00
weight = 4
chapter = false
pre = "<b>4. </b>"
+++

{{% notice info%}}
Since you will not use savings plans instance within the scope of lab posts because savings plans instance requires you to purchase savings plans in advance, this lab is only illustrative.
{{% /notice%}}

{{% notice note%}}
If you have read through [Creating a Reservation Budget](../3-reservation-budget), you will notice that the process of creating Savings Plans Budget is very similar, with a single difference that Reservation Budget works in relation to **reserved instances**, while Savings Plans Budget works in relation to **savings plans**.
{{% /notice%}}

1. Sign in to the AWS Management Console and open the **Billing and Cost Management console** at https://console.aws.amazon.com/billing/ or type in `billing` into the service search-bar and select the first search result.

![Billing Service](/images/4-budget/CostBudget/2.1.1.png?width=90pc)

2. In the navigation pane, choose **Budgets**.

3. At the top of the page, choose **Create budget**.

![Create Service](/images/4-budget/CostBudget/2.1.2.png?width=90pc)

4. For **Choose budget type**, choose **Savings Plans budget**. Then, choose **Next**.

![Budget Type](/images/4-budget/SavingPlansBudget/2.4.3.png?width=90pc)

5. Under **Utilization threshold**, for **Period**, choose how often you want the budget to reset the tracked utilization or coverage.

6. For **Monitor my spend against**, choose **Utilization of Savings Plans** to track how much of your Savings Plans you used. Or, choose **Coverage of Savings Plans** to track how much of your instance usage is covered by Savings Plans. 

   For **Utilization threshold**, enter the utilization percentage that you want AWS to notify you at. For example, for a utilization budget where you want to stay above 90% Savings Plans utilization, enter 90. The budget notiﬁes you when your overall Savings Plans utilization is below 90%.

   For **Coverage threshold**, enter the coverage percentage that you want AWS to notify you at. For example, for a coverage budget where you want to stay above 80%, enter 80. The budget notiﬁes you when your overall coverage is below 80%

![Configure Budget](/images/4-budget/SavingPlansBudget/2.4.4.png?width=90pc)

7. Under **Details**, for **Budget name**, enter the name of your budget. Your budget name must be unique within your account. It can contain A-Z, a-z, spaces, and the following characters:

```text
 _.:/=+-%@
```

8. Select **Next** to configure alerts.

![Configure Alerts](/images/4-budget/SavingPlansBudget/2.4.5.png?width=90pc)

9. Review all configurations and select **Create**.
+++
title = "Creating a Reservation Budget"
date = 2020-04-18T00:38:32+07:00
weight = 3
chapter = false
pre = "<b>3. </b>"
+++

{{% notice info%}}
Since we will not be utilising Reserved Instances within our lab due to the usage commitment, this lab is only illustrative.
{{% /notice%}}

1. Sign in to the AWS Management Console and open the **Billing and Cost Management console** at https://console.aws.amazon.com/billing/ or type in `billing` into the service search-bar and select the first search result.

![Billing Service](/images/4-budget/CostBudget/2.1.1.png?width=90pc)

2. In the navigation pane, choose **Budgets**.

3. At the top of the page, choose **Create budget**.

![Create Service](/images/4-budget/CostBudget/2.1.2.png?width=90pc)

4. For **Choose budget type**, choose **Reservation budget**. Then, choose **Next**.

![Budget Type](/images/4-budget/ReservationBudget/2.3.3.png?width=90pc)

5. Under **Utilization threshold**, for **Period**, choose how often you want the budget to reset the tracked utilization or coverage.

6. For **Monitor my spend against**, choose **Utilization of reservations** to track how much of your reservation you used. Or, choose **Coverage of reservations** to track how much of your instance usage is covered by reservations.

{{% notice info%}}
**RI Utilization** = total hours spent using reserve instances / total hours provisioned for reserved instances. RI Utilization helps you measure the effectiveness of using reserve instance. \
**RI Coverage** = total hours spent on reserve instances / total hours spent using the service has the same classification as the reserve instances. RI Coverage helps you decide how much reserve instance to purchase to get the most out of this pricing model.
{{% /notice%}}

{{% notice tip %}}
For example, we commit to use 100 hours but only used up 50 hours.  
**RI Utilization** = 50% (since we only use 50% of committed hours)  
**RI Coverage** = 100% (because the commitment has covered all actual usage)  
In another case, we promise to use 50 hours but actually use up 100 hours.  
**RI Utilization** = 100% (since we have used all committed hours)  
**RI Coverage** = 50% (because we only commit to 50% of the actual usage)  
{{% /notice %}}

7. For **Service**, choose the service that you want the budget to track.

8. For **Utilization threshold**, enter the utilization percentage that you want AWS to notify you at. For example, for a utilization budget where you want to stay above 90% RI utilization, enter 90. The budget notiﬁes you when your overall RI utilization is below 90%.

    For **Coverage threshold**, enter the coverage percentage that you want AWS to notify you at. For example, for a coverage budget where you want to stay above 80%, enter 80. The budget notiﬁes you when your overall coverage is below 80%.

![Configure Budget](/images/4-budget/ReservationBudget/2.3.4.png?width=90pc)

9. Under **Details**, for **Budget name**, enter the name of your budget. Your budget name must be unique within your account. It can contain A-Z, a-z, spaces, and the following characters:

```text
 _.:/=+-%@
```

10. Select **Next** to configure alerts.

![Configure Alerts](/images/4-budget/ReservationBudget/2.3.5.png?width=90pc)

11. Review all configurations and select **Create**.
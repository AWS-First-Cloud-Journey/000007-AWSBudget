---
title : "Create Usage Budget"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

In this section, you will practice creating a Usage Budget.

{{% notice note %}}
If you've gone through [create Cost Budget](../1-cost-budgets), you'll see that the process for creating Usage Budget is very similar, with the only difference being that Cost Budget works on * *cost**, while Usage Budget works on **usage**.

{{% /notice %}}

**Content:**
- [Create usage budget](#create-usage-budget)

#### Create usage budget

1. Log in to the **AWS Management Console** admin page and select the **Billing** service in the search bar.

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

2. In the admin page, select **Budgets**.

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

3. Select **Create budget**.

![Budget Name & Amount](/images/3/0001.png?featherlight=false&width=90pc)

4. Select **Budget type**

- Select **Customize**
- Select **Usage budget**

![Budget Name & Amount](/images/3/0002.png?featherlight=false&width=90pc)

5. Name the budget.

![Budget Name & Amount](/images/3/0003.png?featherlight=false&width=90pc)

6. Select **Use type groups**

- Select **EC2:Running Hours**

![Budget Name & Amount](/images/3/0004.png?featherlight=false&width=90pc)

7. Do **Set budget amount**

- Select **Period**
- Select **Budget renewal type**
- Select **Budgeting method**
- Enter the number of hours.

![Budget Name & Amount](/images/3/0005.png?featherlight=false&width=90pc)

8. Leave the default and select **Next**

![Budget Name & Amount](/images/3/0006.png?featherlight=false&width=90pc)

9. Configure **Alert**

![Budget Name & Amount](/images/3/0007.png?featherlight=false&width=90pc)

10. Complete information **Alert**

![Budget Name & Amount](/images/3/0008.png?featherlight=false&width=90pc)

11. Select **Next**

![Budget Name & Amount](/images/3/0009.png?featherlight=false&width=90pc)

12. Select **Create budget**

![Budget Name & Amount](/images/3/00010.png?featherlight=false&width=90pc)

13. Tao budget success.

![Budget Name & Amount](/images/3/00011.png?featherlight=false&width=90pc)

14. Check **Budget health**

![Budget Name & Amount](/images/3/00012.png?featherlight=false&width=90pc)

15. Review **Budget history**

![Budget Name & Amount](/images/3/00013.png?featherlight=false&width=90pc)
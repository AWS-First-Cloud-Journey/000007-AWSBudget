+++
title = "Clean Up Resources"
date = 2024
weight = 6
chapter = false
pre = " <b> 6. </b> "
+++

#### Overview

In this section, you will learn how to properly clean up AWS Budgets created during this lab to maintain a tidy AWS account and prevent unnecessary notifications.

#### Managing AWS Budgets

AWS Budgets are powerful tools for cost management in cloud environments. After completing this lab, it's important to remove any test budgets you've created to keep your AWS account organized.

{{% notice info %}}
**ℹ️ Information**: AWS Budgets remain active until explicitly deleted, and will continue to send notifications based on your configured thresholds even after you've finished experimenting with them.
{{% /notice %}}

#### Steps to Delete AWS Budgets

1. Sign in to the **AWS Management Console** and search for **AWS Billing and Cost Management** in the services search bar.

2. In the navigation pane, select **Budgets**.

3. From the list of budgets, select the budget you want to remove:
   - Click the checkbox next to the budget name
   - Click the **Delete** button in the upper right corner
   
   ![Deleting a Budget](/images/5/z0009.png?featherlight=false&width=90pc)

4. In the confirmation dialog, review the budget name to ensure you're deleting the correct budget, then click **Confirm** to permanently delete the budget.

   ![Confirming Budget Deletion](/images/5/z00010.png?featherlight=false&width=90pc)

5. Repeat steps 3-4 for each budget you created during this lab.

{{% notice tip %}}
**💡 Pro Tip**: Before deleting production budgets in a real environment, consider exporting budget reports or taking screenshots of historical data if you need to retain this information for reference.
{{% /notice %}}

{{% notice warning %}}
**⚠️ Warning**: Budget deletion is permanent and cannot be undone. Make sure you're deleting the correct budgets, especially in production environments where multiple teams may be relying on budget alerts.
{{% /notice %}}

#### Verification

After deleting all budgets, refresh the Budgets page to confirm that all lab-related budgets have been successfully removed from your account.

{{% notice security %}}
**🔒 Security Note**: Regularly reviewing and cleaning up AWS Budgets is a good security practice, as it ensures that only relevant notifications are being sent to your team and reduces the risk of alert fatigue.
{{% /notice %}}

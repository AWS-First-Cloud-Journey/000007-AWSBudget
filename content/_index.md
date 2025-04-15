+++
title = "Getting Started with AWS Budgets"
date = 2024
weight = 1
chapter = false
+++

# Cost Management with AWS Budgets

#### Overview

In this workshop, you will explore how **AWS Budgets** can help you effectively manage and monitor costs within your AWS account.

#### What is AWS Budgets?

**AWS Budgets** allows you to set custom budgets to track your AWS costs and usage. When your costs or usage exceed (or are forecasted to exceed) your budgeted amount, you receive notifications to help you stay on top of your AWS spending.

ℹ️ **Information**: AWS Budgets provides near real-time visibility into your current and forecasted AWS spend, helping you proactively manage your costs before they occur.

#### Types of AWS Budgets

You can create several types of budgets in AWS:

1. **Cost Budget** - Tracks your AWS spend and alerts you when costs exceed thresholds
2. **Usage Budget** - Monitors usage of specific AWS services (like EC2 hours)
3. **Reservation Budget** - Tracks utilization and coverage of your Reserved Instances
4. **Savings Plans Budget** - Monitors utilization and coverage of your Savings Plans commitments

#### Cost Budget

A **Cost Budget** provides alerts when your current or projected AWS spending exceeds the cost threshold you've set. This is the most common type of budget and helps you maintain financial control over your AWS environment.

#### Usage Budget

A **Usage Budget** sends alerts when the usage of a specific service or group of services exceeds your defined threshold. For example, you can set a budget to monitor EC2 compute hours or data transfer volumes.

#### Reserved Instance (RI) Budget

The **RI Budget** generates alerts based on the utilization or coverage of your Reserved Instances.

ℹ️ **Information**: **Reserved Instances (RIs)** provide significant discounts (up to 72%) compared to On-Demand pricing when you commit to a one-year or three-year term for specific EC2 instance types.

#### Savings Plans Budget

With **Savings Plans Budget**, you receive alerts based on the utilization or coverage of your Savings Plans commitments.

ℹ️ **Information**: **Savings Plans** is a flexible pricing model that offers lower prices compared to On-Demand, in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term. AWS offers Compute Savings Plans, EC2 Instance Savings Plans, and SageMaker Savings Plans.

#### Best Practices for AWS Budgets

##### Access Control

To enable users to create budgets in the AWS Billing and Cost Management console, ensure they have permissions to:

- View billing information
- Create Amazon CloudWatch alarms
- Create Amazon SNS notifications

🔒 **Security Note**: Use IAM roles with least privilege principles when granting access to AWS Budgets. Consider creating dedicated roles for programmatic access to the Budgets API.

##### Budget Actions

AWS Budgets can be configured to take automated actions when a budget threshold is reached. Two AWS managed policies simplify this setup:

1. A policy for users to pass a role to the budgets service
2. A policy for budgets to execute the configured actions

💡 **Pro Tip**: When using budget actions with EC2 instances in Auto Scaling Groups, be aware that the ASG may restart or replace instances that are shut down. Consider adding a second budget action that removes permissions from the Launch Configuration role.

##### Setting Effective Budgets

- Set budgets on a recurring basis to maintain continuous monitoring
- Configure multiple alert thresholds (e.g., 50%, 80%, 90%, 100%)
- Include both actual and forecasted alerts for proactive management
- Consider using advanced options like filtering by tags to track costs by project or department

⚠️ **Warning**: AWS Budgets relies on billing data that updates at least once daily. Budget alerts align with this refresh cadence, so there may be a slight delay between when costs are incurred and when alerts are triggered.

##### Budget Alerts

- Budget alerts can be sent to up to 10 email addresses and one Amazon SNS topic per alert
- Actual alerts trigger once per budget period when reaching the threshold
- Forecast-based alerts may trigger multiple times if forecasted values fluctuate around the threshold
- AWS requires approximately 5 weeks of usage data to generate accurate forecasts

🔒 **Security Note**: Consider enabling multi-factor authentication (MFA) for enhanced account security, especially for accounts with budget management permissions.

#### Workshop Content

1. [Creating a Cost Budget](1-cost-budgets)
2. [Creating a Usage Budget](2-usage-budget)
3. [Creating a Reservation Budget](3-reservation-budget)
4. [Creating a Savings Plans Budget](4-saving-plans-budget)
5. [Resource Cleanup](5-clean-up)

+++
title = "Getting Started with AWS Budgets"
date = 2021
weight = 1
chapter = false
+++

# Cost Management with AWS Budgets

## Overview

In this lab, we will explore how **AWS Budgets** can assist you in cost management within your AWS account.

## AWS Budgets

**AWS Budgets** is a service designed to enable you to establish one-time or recurring budgets. These budgets will send you alerts whenever costs exceed (or are forecasted to exceed) your predetermined budgeted cost or usage amount.

You can create several types of budgets:

- [Cost Budget](#cost-budget).
- [Usage Budget](#usage-budget).
- [Reserved Instance Budget](#reservation-instance-ri-budget).
- [Savings Plans Budget](#savings-plans-budget).

## Cost Budget

A **Cost Budget** provides alerts when the current or projected spending surpasses the cost threshold set within the budget.

## Usage Budget

An **Usage Budget** sends alerts when the current or projected usage of a chosen service or group of services exceeds the usage budget threshold. For instance, you could budget the usage of running hours for EC2 compute services.

## Reserved Instance (RI) Budget

The **RI Budget** generates alerts based on your usage or coverage of committed usage, also known as a *reserved instance*.

> **Note:** A **Reserved Instance (RI)** is a discounted EC2 offering when you commit to a one-year or three-year term.

## Savings Plans Budget

With the **Savings Plans Budget**, you will receive alerts based on usage or coverage of services specified within savings plans.

> **Note:** **Savings Plans** is a pricing model offering reduced prices for EC2, Lambda, and Fargate usage. This is in exchange for committing to a consistent usage amount (measured in $/hour) for a 1 or 3 year term. There are two types of Savings Plans: **Compute Savings Plans** and **EC2 Instance Savings Plans**.

## Best Practices for Controlling Access to AWS Budgets

To enable users to create budgets in the AWS Billing and Cost Management console, ensure they have permission to:

- View your billing information.
- Create Amazon CloudWatch alarms.
- Create Amazon Simple Notification Service (Amazon SNS) notifications.

For more information, see [Allow users to create budgets](link_here).

You can also programmatically create budgets using the Budgets API. When configuring API access, it's recommended to create a unique user role for programmatic requests. This ensures precise access controls between AWS Budgets console and the API. For multiple users with query access to the Budgets API, create a role for each.

## Best Practices for Budget Actions

### Using Managed Policies

Two AWS managed policies simplify budget actions setup: one for users and one for budgets. These policies are related. The first policy allows a user to pass a role to the budgets service, and the second permits budgets to execute the action.

Proper permissions are vital for AWS Budgets to execute your configured actions. Managed policies ensure correct configuration and execution, adding new capabilities automatically.

For policy details, see [Managed policies](link_here).

Learn more about AWS Budgets actions in the [Configuring AWS Budgets actions](link_here) section.

### Using Amazon EC2 Auto Scaling

For budget actions affecting an Amazon EC2 instance in an Auto Scaling Group (ASG), Amazon EC2 Auto Scaling restarts or replaces instances. "Shutdown budget actions is not effective to Amazon EC2/Amazon RDS budget actions" unless combined with a second budget action removing permissions on the Launch Configuration role managing the ASG.

## Best Practices for Setting Budgets

Use AWS Budgets to set custom budgets based on costs, usage, reservation utilization, and coverage. Set budgets on a recurring basis to avoid unexpected alerts.

## Best Practices for Using Advanced Options When Setting Cost Budgets

Cost budgets can be aggregated by unblended costs, amortized costs, or blended costs. Budgets can also include or exclude refunds, credits, upfront reservation fees, recurring reservation charges, non-reservation subscription costs, taxes, and support charges.

## Understanding the AWS Budgets Update Frequency

Budgets rely on AWS billing data, updated at least once daily. Alerts and budget information align with this refresh cadence.

## Best Practices for Setting Budget Alerts

Budget alerts can be sent to up to 10 email addresses and one Amazon SNS topic per alert. Alerts can target actual or forecasted values.

Actual alerts trigger once per budget, per budget period, upon reaching the alert threshold. Forecast-based alerts trigger on a per-budget, per-budget period basis. If forecasted values exceed, dip below, and then exceed the threshold within a budgeted period, multiple alerts can be generated.

AWS requires about 5 weeks of usage data for budget forecasts. Forecast-based alerts need sufficient historical usage information.

A video emphasizes budget alert setup's importance and highlights the use of multi-factor authentication (MFA) for enhanced account security.

## Content

1. [Creating a Cost Budget](1-cost-budgets)
2. [Creating a Usage Budget](2-usage-budget)
3. [Creating an Reservation Budget](3-reservation-budget)
4. [Creating a Savings Plans Budget](4-saving-plans-budget)
5. [Resource Cleanup](5-clean-up)

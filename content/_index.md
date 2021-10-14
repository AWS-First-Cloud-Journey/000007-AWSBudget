+++
title = "Getting Started with AWS Budgets"
date = 2021
weight = 1
chapter = false
+++

# Cost Management with AWS Budgets

#### Overview

In this lab, we'll explore how AWS Budgets can help you manage costs within your AWS account.

#### AWS Budgets
**AWS Budgets** is a service that allows you to set a one-time or recurring budget that alerts you when costs exceed (or are forecasted to exceed) your budgeted cost or usage amount.

You can create the following types of budgets: 
- [Cost Budget](#cost-budget).
- [Usage budget](#usage-budget).
- [Reserved Instance Budget](#reservation-instance-ri-budget).
- [Savings Plans Budget](#savings-plans-budget).

#### Cost Budget
A **Cost Budget** allows you to send alerts when the current or projected spend exceeds the cost threshold in the budget. 

#### Usage Budget
A **Usage Budget** allows you to send alerts when the current or projected usage of a service or group of services you choose exceeds the usage budget threshold.

For example, we may budget the usage of the number of running-hours of EC2 compute-services.

#### Reserved Instance (RI) Budget
**RI Budget** allows you to send alerts based on your usage or coverage of committed usage (*reserve instance*).

{{% notice note%}}
A **Reserved Instance (RI)** is an EC2 offering that provides you with a significant discount on EC2 usage when you commit to a one-year or three-year term.
{{% /notice%}}

#### Savings Plans Budget
**Savings Plans Budget** allows you to send alerts based on the usage or coverage of services specified in the savings plans.

{{% notice note%}}
**Savings Plans** is a flexible pricing model that offers low prices on EC2, Lambda and Fargate usage, in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term. When you sign up for Savings Plans, you will be charged the discounted Savings Plans price for your usage up to your commitment.
\
\
AWS offers two types of Savings Plans:
\
**Compute Savings Plans** provides the most flexibility and help to reduce your costs by up to 66%. These plans automatically apply to EC2 instance usage regardless of instance family, size, Availability Zone, region, Operating System or tenancy, and also apply to AWS Fargate and Lambda usage. For example, with Compute Savings Plans, you can change from `C4` to `M5` instances, shift a workload from EU (Ireland) to EU (London), or move a workload from EC2 to Fargate or Lambda at any time and automatically continue to pay the Savings Plans price.
\
\
**EC2 Instance Savings Plans** provides the lowest prices, offering savings up to 72% in exchange for commitment to usage of individual instance families in a region (e.g. `M5` usage in N. Virginia). This automatically reduces your cost on the selected instance family in that region regardless of Availability Zone, size, Operating System or tenancy. EC2 Instance Savings Plans give you the flexibility to change your usage between instances within a family in that region. For example, you can move from `c5.xlarge` running Windows to `c5.2xlarge` running Linux and automatically benefit from the Savings Plan prices.
\
\
**Savings plans** offer more flexible than Reserved Instances with comparable discounts. You are encouraged to use Savings plans for predictable, sustained workloads on EC2.
{{% /notice%}}

#### Content
1. [Creating a Cost Budget](1-cost-budgets)
2. [Creating a Usage Budget](2-usage-budget)
3. [Creating an Reservation Budget](3-reservation-budget)
4. [Creating a Savings Plans Budget](4-saving-plans-budget)
5. [Resource Cleanup](5-clean-up)
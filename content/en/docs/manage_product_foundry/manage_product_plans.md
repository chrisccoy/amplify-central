---
title: Manage product plans
linkTitle: Manage product plans
weight: 35
---

Monetize the product and define the usage terms by using product plans.

## Objectives

Learn how to create and configure the product plan using the Product Foundry WebUI.

## Concepts

**Plan** - contains the details about how to charge consumers, how often and how much.

**Quotas** - describes the itemized units per resource or group of resources in the product, and how much of those units they are entitled to use over a billing period.

**Units** - defines the billable units. For example: Transactions, Seats, Messages. Used with the quotas to describe the pricing and how many units a consumer is entitled to use.

## Product plan states

| State      | Description                                                                                                                                                                |
|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Draft      | The plan is not listed in the Marketplace. Changes can be made to the plan.                                                                                 |
| Active     | The plan is listed in the Marketplace. Allows new subscriptions.                                                                                            |
| Deprecated | New subscriptions on this plan are not allowed. Consumers with an existing subscription can continue to stay on this plan until their subscription expires. |
| Archived   | After a plan is deprecated with an auto-expiration date, the plan will automatically move to Archived when the last subscription moves to expired.                         |

## Product plan type and consumption cost

There are two types of plans:

* **Free plan** - consumer will not be charged for their API consumption.
* **Paid plan**:
    * **Standard** - consumer will be charged a base price for the consumption of a guaranteed set of quota.
    * **Tier - volume** - consumer will be charged based on the volume corresponding to the tier quota + flat tier fee, if any.
    * **Tier - graduated** - consumer will be charged based on the volume corresponding to each tier quota that includes their consumption + flat tier fee, if any.

Illustrative pricing samples:

* Standard paid plan cost: $0.01 per transaction

* Tier paid plan cost:

| *Limit from* | *Limit to*     | *Unit price* | *Tier Flat fee*   |
|--------------|----------------|--------------|-------------------|
| 1            | 500            | $2           | $0                |
| 501          | 5000           | $1           | $10               |
| 5001         | unlimited      | $0.5         | $20               |

* Associated costs:

| *Plan Type*      | *Consumed transactions* | *Cost*                                                                                                                                                                         |
|------------------|-------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| standard         | 1,975                   | 1,975 * 0.01 = **$ 19.75**                                                                                                                                                     |
| standard         | 10,000                  | 10,000 * 0.01 = **$ 100**                                                                                                                                                      |
|                  |                         |                                                                                                                                                                                |
| tier - volume    | 1,975                   | Second tier applied as matching the number of transactions + flat fee tier 2 -> 1975 \* 1 + 10 = **$ 1,985**                                                                      |
| tier - volume    | 10,000                  | Third tier applied + flat fee tier 3 -> 10,000 \* 0.5 + 20 = **$ 5,020**                                                                                                 |
|                  |                         |                                                                                                                                                                                |
| tier - graduated | 1,975                   | Cost of the first 500 trs + cost of the remaining transactions + flat fee from tier 1 and 2 -> 500 \* 2 + 1,474 \* 1 + 10 = **$ 2,484**                                              |
| tier - graduated | 10,000                  | Cost of the first 500 trs + cost of the next 5000 + cost of the remaining transactions + flat fee from tier 1,2 and 3 -> 500 \* 2 + 4,499 \* 1 + 4,999 \* 0.5 + 10 + 20 = **$ 8,528.5** |

## Create a product plan

When you create a new product, you have the option to configure one **Free** or **paid** product plan. If you skip this step, a default free plan will be auto generated, which you can edit / modify later.

Plans can be created anytime, regardless of the product state (draft / active / deprecated) and the product publication on the Marketplace.

The plan wizard is composed of three pages:

* Page 1: the plan profile - title, description, type (Free / Paid)
* Page 2: [the plan quotas definition](/docs/manage_product_foundry/manage_product_plans#configure-a-quota)
* Page 3: [the approval mode](/docs/manage_product_foundry/manage_product_plans#configure-access)

To configure a product plan from the create product wizard:

1. [Create a new product](/docs/manage_product_foundry/foundry_product_management/#create-a-product). *The Create product wizard is displayed*.
2. Enter the following properties in **Usage plan**:

    * **Plan title** - the display name of the plan that will be listed in the Marketplace to identify the plan.
    * **Logical name** - a logical name to uniquely identity the plan in the system. If no value is entered, one will be auto generated for you.
    * **Description** - describe the product plan in few words so the consumer will know what the offering is.

3. Select either **Free** or **Paid** plan type, and proceed to the **Next** step to configure the plan quota.

To configure a product plan from the product detail:

1. Navigate to the Plans section.
2. Click **+ Add Plan** to open the plan creation wizard.
3. Follow the plan wizard and enter the required information.

### Configure a quota

A quota describes the itemized units per resource or group of resources in a product, and how much of those units they are entitled to use over a period of time.

For paid plan quota, it also describes the base pricing of the plan and the pricing of the quota based on the quota type (Standard / Tier). See [Product plan type and consumption cost](/docs/manage_product_foundry/manage_product_plans/#product-plan-type-and-consumption-cost).

To configure a quota for a free plan, enter values for the following properties:

* **Quota name** - a name for the quota.
* **Quota type** - only **Standard** is available.
* **Unit** - the default is **Transactions**. This non-configurable field defines a quota for Transaction units only.
* **Limit** - a quantity. For example, 1000, 15.
* **Quota type** - select either **Daily**, **Weekly**, **Monthly**, or **Annually**.
* **Limit Type**:  
    * **Strict** - the gateway enforces a hard stop when the quota limit is exceeded.
    * **Loose** - the quota can be exceeded.
* **Assign Resources** - the list of resources the provider will charge for by a measured unit. Only the resources included in the plan can be selected.

{{< alert title="Note" color="primary" >}}When Limit Type is set to Strict, make sure the quota is enforced on the underlying gateway.{{< /alert >}}

To configure a quota for a paid plan, enter values for the following properties:

* **Base price**:
    * **Currency** - the currency that will be used by the billing system (USD - EUR).
    * **Amount** - the price value.
    * **Metering period** - select either **Monthly**, **Daily**, **Weekly**, or **Annually**.
* **Quota type** - select either **Standard** or **Tiered**:
    * Standard - has the same information as the free plan (**Unit**, **Limit**, **Quota type**, **Limit type**).
    * Tiered - for each tier, enter the **lower limit**, the **upper limit**, the **unit price**, and the **Standard** fees. There is no limit in the tier number. Click **+** to add another tier, or **-** to remove a tier definition. The lower limit of the next tier is automatically computed based on the upper limit of previous tier.

Click **+ Add Quota** to create another quota group for a different resource. Once a resources is assigned to a quota group, it is no longer available for another quota group.

When you are finished configuring the quotas, click **Next** to select the approval mode of the plan.

### Configure access

To configure the type of approval when a subscriber submits a request to purchase the plan, choose between:

* **Manual** - a provider will have to manually approve the subscription before the consumer can use it.
* **Automatic** - the subscription is automatically approved and immediately usable.

When you are finished creating the plan, click **Save Draft and Exit** to save the product plan in DRAFT state.

## Edit product plans

1. Navigate to the *Product Foundry* and select a product.
2. Click on the **Plans** tab. All plans configured for this product are displayed.
3. Click on the ellipsis on the plan table and select **Edit Plan**. The plan wizard opens with the plan information. You can modify any value except the plan name.

## View product plans

1. Navigate to the *Product Foundry* and select a product.
2. Click on the **Plans** tab. All plans configured for this product are displayed.
3. Click on the plan title. The configuration of the plan is displayed in the side panel.

## Publish a product plan in the Marketplace

1. Navigate to the *Product Foundry* and select a product.
2. Click on the **Plans** tab. All plans configured for this product are displayed.
3. Click on the plan title. The configuration of the plan is displayed in the side panel.
4. Click **Activate** to publish.

You can also use the ellipsis menu on the plan list and select **Activate**. Only plans in DRAFT state can be activated.

{{< alert title="Note" color="primary" >}}A plan can only be listed in the Marketplace when the product the plan is associated to is ACTIVE and PUBLISHED in the Marketplace.{{< /alert >}}

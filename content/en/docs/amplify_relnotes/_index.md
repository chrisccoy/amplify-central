---
title: Release Notes
linkTitle: Release Notes
no_list: true
weight: 100
date: 2020-10-28
hide_readingtime: true
---

This page displays brief summaries of feature updates and bug fixes for each release of Amplify, including:

* Provider experience: Agents, Service Registry, Asset Catalog, Product Foundry, Business insights
* Consumer experience: Marketplace, Consumer insights

For more details, click on the release note title to go to the corresponding release note.

To view the *Administration Release Notes* [click here](https://docs.axway.com/bundle/platform-management/page/docs/release_notes/index.html).

To view the *Support Policy for Amplify Agents and Amplify Agent SDK* [click here](/docs/amplify_relnotes/agent_agentsdk_support_policy/).

## [Amplify November 18th, 2022](/docs/amplify_relnotes/20221118_amplify/)

Current agent versions are based on Amplify Agents SDK v1.1.41. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.36
* **AWS Gateway using SDK 2.0** - Agent version 1.1.32
* **Azure latest release** - Agent version 1.1.35
* **Istio 1.9.5** - DA=v1.0.3 / TA=v2.0.43
* **Apigee Edge** - Agent version 0.1.3
* **Mulesoft Anypoint platform v3** - Agent version 1.1.10

| Axway Agent SDK |        |
|--------|---------|
| What's new: | Discovery Agent updated for Async API support. |
| Bug fixes: | API Service deletion handling. <br />API Service revision handling. |

| Agents |         |
|--------|---------|
| What's new: | **AWS Gateway** - Agents updated with Axway Agent SDK. <br />**Azure Gateway** - Agents updated with Axway Agent SDK. <br />**Istio Gateway** - Discovery Agent updated with Axway Agent SDK.  <br />**Apigee Edge Gateway** - Agents updated with Axway Agent SDK. |
| Bug fixes: | **Axway API Management Gateway** - Helm chart installation when using an existing service account. |

| Service registry <br />Topology |         |
|------------------|------------------------|
| What's new: | None. |
| Bug fixes: | None. |

| Asset Catalog |         |
|---------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Pay per use plan configured in Catalog Manager. <br />Product visibility for consumer organization user. <br />Support contact alternative method. <br />Support contact set while creating / updating product. |
| Bug fixes: | Country codes list for support contact phone number. |

| Business insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | Vanity URL. <br />Application list page improvement. <br />Call to Action. <br />Access request visibility. |
| Bug fixes: | Consumer user (non-admin) cannot create access request / credentials in the consumer org. <br />Product documents in the Marketplace are not being displayed in proper order. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

## [Amplify November 4th, 2022](/docs/amplify_relnotes/20221104_amplify/)

Current agent versions are based on Amplify Agents SDK v1.1.40. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.34
* **AWS Gateway using SDK 2.0** - Agent version 1.1.31
* **Azure latest release** - Agent version 1.1.34
* **Istio 1.9.5** - DA=v1.0.2 / TA=v2.0.43
* **Apigee Edge** - Agent version 0.1.2
* **Mulesoft Anypoint platform v3** - Agent version 1.1.10

| Axway Agent SDK |        |
|--------|---------|
| What's new: | Discovery Agent supports HTTP Basic Authentication for inbound security of Marketplace products. |
| Bug fixes: | None. |

| Agents |         |
|--------|---------|
| What's new: | **API Management Gateway** - Discovery Agent supports HTTP Basic Authentication for inbound security of Marketplace products. <br />**AWS Gateway** - Updated with the latest Agent SDK. <br />**Azure Gateway** - Updated with the latest Agent SDK. <br />**Istio Gateway** - Usage tracking customization. |
| Bug fixes: | None. |

| Service registry <br />Topology |         |
|------------------|------------------------|
| What's new: | None. |
| Bug fixes: | None. |

| Asset Catalog |         |
|---------------|---------|
| What's new: | An asset can be edited from the Web UI with or without the release of a new asset version. |
| Bug fixes: | None. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Support contacts can be assigned to a product. <br />A product can be edited from the Web UI with or without the release of a new product version. |
| Bug fixes: | Subscription Approver role is not able to see the access requests submitted by a user in a consumer organization. <br />Creating a product/plan and changing the product plan ownership fails. <br />Wrong plan ownership. <br />Quota price validation. |

| Business insights |         |
|-------------------|---------|
| What's new: | Provider engagement report. |
| Bug fixes: | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | Support contact displays on product overview. <br />Product resources page improvement. |
| Bug fixes: | Issue with the “logical name” of the category - Product Foundry. <br />Confusing plan count on product tile. <br />Confusing sign in page. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

## [Amplify October 21st, 2022](/docs/amplify_relnotes/20221021_amplify/)

Current agent versions are based on Amplify Agents SDK v1.1.39. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.33
* **AWS Gateway using SDK 2.0** - Agent version 1.1.30
* **Azure latest release** - Agent version 1.1.33
* **Istio 1.9.5** - Agent version 0.75
* **Apigee Edge** - Agent version 0.1.2
* **Mulesoft Anypoint platform v3** - Agent version 1.1.10

| Axway Agent SDK |        |
|--------|---------|
| What's new: | None. |
| Bug fixes: | Subscription migration. |

| Agents |         |
|--------|---------|
| What's new: | **AWS Gateway** - Quota provisioning feature. <br />**Apigee Gateway** - Configurable IDP settings. |
| Bug fixes: | **Apigee Gateway** - CPU/Memory utilization. |

| Service registry <br />Topology |         |
|------------------|------------------------|
| What's new: | None. |
| Bug fixes: | None. |

| Asset Catalog |         |
|---------------|---------|
| What's new: | Auto release management. |
| Bug fixes: | None. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Auto release management. <br />Export subscriber contact information. <br />Subscription approver role. |
| Bug fixes: | Product ownership not replicated to plan ownership. |

| Business insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | User experience improvements. <br />Consumer Organization management. |
| Bug fixes: | Wrong owner of the subscription. <br />Category names are truncated. <br />Incorrect warning displayed. <br />Error message when subscribing is not clear. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

## [Amplify October 7th, 2022](/docs/amplify_relnotes/20221007_amplify/)

Current agent versions are based on Amplify Agents SDK v1.1.38. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.32
* **AWS Gateway using SDK 2.0** - Agent version 1.1.29
* **Azure latest release** - Agent version 1.1.32
* **Istio 1.9.5** - Agent version 0.75
* **Apigee Edge** - Agent version 0.1.1
* **Mulesoft Anypoint platform v3** - Agent version 1.1.10

| Axway Agent SDK |        |
|--------|---------|
| What's new: | None. |
| Bug fixes: | Credential validation. |

| Agents |         |
|--------|---------|
| What's new: | **Azure Gateway** - Product plan quota provisioning. <br />**Istio Gateway** - Marketplace provisioning, Helm override values. |
| Bug fixes: | **API Management Gateway** - Single entry point URL. |

| Service registry <br />Topology |         |
|------------------|------------------------|
| What's new: | None. |
| Bug fixes: | None. |

| Asset Catalog |         |
|---------------|---------|
| What's new: | Auto-asset release from latest API Service version. |
| Bug fixes: | None. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Filter access requests. <br />Product wizard update to create product category while creating/editing product. <br />Auto-product release from latest Asset version. |
| Bug fixes: | Product plans not inheriting the product ownership. |

| Business insights |         |
|-------------------|---------|
| What's new: | Application usage report. <br />New Application column in Subscription compliance report. |
| Bug fixes: | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | Browse products and product card usability enhancements. |
| Bug fixes: | Product plan display issues. <br />Remaining time to view credential issue. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

## [Amplify September 23rd, 2022](/docs/amplify_relnotes/20220923_amplify/)

Current agent versions are based on Amplify Agents SDK v1.1.37. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.31
* **AWS Gateway using SDK 2.0** - Agent version 1.1.29
* **Azure latest release** - Agent version 1.1.31
* **Istio 1.9.5** - Agent version 2.0.38
* **Apigee Edge** - Agent version 0.1.1
* **Mulesoft Anypoint platform v3** - Agent version 1.1.10

| Agents |         |
|--------|---------|
| What's new: | **All agents** - Consumer credential management. <br />**Apigee Gateway** - Quota provisioning. |
| Bug fixes: | **All agents** - Fix for Analytics support and Marketplace provisioning. <br />**API Management Gateway** - Consumer Insights Application Usage issue, Marketplace product and application deletion issue. |

| Service registry <br />Topology |         |
|------------------|------------------------|
| What's new: | Unified Catalog enabled by entitlements. |
| Bug fixes: | Teams names in the filter are not sorted alphabetically. |

| Asset Catalog |         |
|---------------|---------|
| What's new: | None. |
| Bug fixes: | Teams names in the filter are not sorted alphabetically. <br />Ownership set at the asset version level. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Provider credential management. <br />Subscription approver role. <br />Swap featured categories. |
| Bug fixes: | Teams names in the filter are not sorted alphabetically. |

| Business insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | Consumer credential management. <br />Search feature on the Marketplace Homepage. <br />Subscription enhancements. |
| Bug fixes: | Subscription and applications do not have the same owner. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes: | None. |

## [Amplify September 9th, 2022](/docs/amplify_relnotes/20220909_marketplace/)

Current agent versions are based on Amplify Agents SDK v1.1.33. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.27
* **AWS Gateway using SDK 2.0** - Agent version 1.1.25
* **Azure latest release** - Agent version 1.1.27
* **Istio 1.9.5** - Agent version 2.0.38
* **Apigee Edge** - Agent version 0.0.9
* **Mulesoft Anypoint platform v3** - Agent version 1.1.8

| Agents |         |
|--------|---------|
| What's new: | **Azure** - API discovery. |
| Bug fixes:  | None. |

| Service registry <br />Topology |         |
|--------|---------|
| What's new: | None.  |
| Bug fixes:  | None.  |

| Asset Catalog |         |
|--------|---------|
| What's new: | Asset sharing with read-only access. |
| Bug fixes:  | Team selector does not switch teams. |

| Product Foundry |         |
|--------|---------|
| What's new: | Category management from a dedicated screen. <br />Product sharing with read-only access. |
| Bug fixes:  | Assigning a product to a category changed the product state. <br />Marketplace active subscription list is empty. |

| Business insights |         |
|--------|---------|
| What's new: | View the consuming teams' usage and quota compliance of subscriptions. |
| Bug fixes:  | None. |

| Marketplace |         |
|--------|---------|
| What's new: | View products in a featured category on the home page. <br />Filter the catalog of products by categories. |
| Bug fixes:  | Paid plan base price with large number crashes the backend. |

| Consumer insights |         |
|--------|---------|
| What's new: | None. |
| Bug fixes:  | None. |

## [Amplify August 26, 2022](/docs/amplify_relnotes/20220826_marketplace/)

Current agent versions are based on Amplify Agents SDK v1.1.30. This version is compatible with:

* **Axway API Management 7.6.2 SPx and 7.7 SPx** - Agent version 1.1.26
* **AWS Gateway using SDK 2.0** - Agent version 1.1.24
* **Azure latest release** - Agent version 1.1.26
* **Istio 1.9.5** - Agent version 2.0.38
* **Apigee Edge** - Agent version 0.0.9
* **Mulesoft Anypoint platform v3** - Agent version 1.1.8

| Agents |         |
|--------|---------|
| What's new: | **Azure** - Consumer insights. |
| Bug fixes:  | **All agents** - API Service revision updates. |

| Service registry <br />Topology |         |
|---------------------------------|---------|
| What's new:                     | Team Ownership can be set when creating environments or API Services with the UI. |
| Bug fixes:                      | None.   |

| Asset Catalog |         |
|---------------|---------|
| What's new: | Manual or automatic access request approvals. <br />Share assets with Read-Only permissions. <br />Filter assets by status.|
| Bug fixes:  | Corrupted assets could be added to a product. <br />Wrong product status in Product Foundry. |

| Product Foundry |         |
|-----------------|---------|
| What's new: | Tiered product plans. <br />Product visibility enhancements. <br />Category management. <br />Corrupted products notification. |
| Bug fixes:  | Slow rendering of the Asset Catalog screen. |

| Business insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes:  | None. |

| Marketplace |         |
|-------------|---------|
| What's new: | Marketplace home page. <br />Plan details. |
| Bug fixes:  | None. |

| Consumer insights |         |
|-------------------|---------|
| What's new: | None. |
| Bug fixes:  | None. |

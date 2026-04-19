# Affirm (affirm)
Affirm is a financial technology company that provides buy now, pay later financing for consumers at the point of sale across thousands of online and in-store merchants. Affirm offers a suite of developer APIs and SDKs enabling merchants to embed flexible installment payment options directly into their checkout flows, mobile apps, and marketing experiences.

**URL:** [https://docs.affirm.com](https://docs.affirm.com)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Android, Authorization, Buy Now Pay Later, Capture, Cards, Chargebacks, Checkout, Credit, Disputes, Files, Fintech, Java, Kotlin, Marketing, Merchant, Messaging, Mobile, Objective-C, Payments, Prequalification, Promotions, Refunds, SDK, Swift, Transactions, Uploads, Virtual Card, iOS

## Timestamps

- **Created:** 2026-04-19
- **Modified:** 2026-04-19

## APIs

### Affirm Direct API
The Affirm Direct API is a flexible integration that allows merchants to embed the full Affirm checkout and payment authorization flow directly into their website, giving complete control over the front-end user experience and back-end transaction processing logic. It supports inline checkout via modal or redirect to affirm.com, and handles the full transaction lifecycle including authorization, capture, void, and refund operations.

**Human URL:** [https://docs.affirm.com/payments/docs/direct-api-overview](https://docs.affirm.com/payments/docs/direct-api-overview)

#### Tags:

 - Buy Now Pay Later, Checkout, Fintech, Merchant, Payments

#### Properties

- [Documentation](https://docs.affirm.com/payments/docs/direct-api-overview)
- [OpenAPI](openapi/affirm-direct-api-openapi.yml)

### Affirm Checkout API
The Affirm Checkout API enables merchants to initiate and manage the Affirm buy now pay later checkout flow for customers at the point of purchase. It provides endpoints to create checkout sessions, read and update checkout objects, and store checkout tokens returned after a customer completes the Affirm financing application. The API supports both redirect and direct checkout integration patterns, and includes endpoints for resending checkout links via email or SMS.

**Human URL:** [https://docs.affirm.com/developers/docs/home-introduction](https://docs.affirm.com/developers/docs/home-introduction)

#### Tags:

 - Buy Now Pay Later, Checkout, Fintech, Merchant, Payments

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/home-introduction)
- [OpenAPI](openapi/affirm-checkout-openapi.yml)
- [JSONSchema](json-schema/affirm-checkout-schema.json)

### Affirm Transactions API
The Affirm Transactions API provides server-side endpoints for managing the full lifecycle of Affirm payment transactions after a customer completes checkout. It supports authorization, capture, void, and refund operations, as well as listing and retrieving transaction details and associated settlement events. Merchants use this API to reconcile charges, process partial or full refunds, and track disbursement activity.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Authorization, Capture, Fintech, Payments, Refunds, Transactions

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)
- [OpenAPI](openapi/affirm-transactions-openapi.yml)
- [JSONSchema](json-schema/affirm-transaction-schema.json)

### Affirm Promos API
The Affirm Promos API is a server-side endpoint that enables merchants to render dynamic promotional pricing text and present Affirm-hosted educational modals on their website. It accepts a purchase amount and returns financing terms, "as low as" monthly payment messaging, APR rates, and modal content including headlines, descriptions, and legal disclosures. The API supports multiple installment term options and page-type context (product, cart, homepage) to customize the displayed messaging.

**Human URL:** [https://docs.affirm.com/developers/docs/promos-api-integration-overview](https://docs.affirm.com/developers/docs/promos-api-integration-overview)

#### Tags:

 - Buy Now Pay Later, Marketing, Merchant, Messaging, Promotions

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/promos-api-integration-overview)
- [OpenAPI](openapi/affirm-promos-openapi.yml)

### Affirm Disputes API
The Affirm Disputes API (V3) provides merchants with programmatic access to manage payment disputes initiated by customers. It supports listing and retrieving individual dispute records, submitting evidence to contest a dispute, and closing disputes. The API integrates with the file upload capability so merchants can attach supporting documentation as evidence when responding to disputes.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Chargebacks, Disputes, Fintech, Merchant, Payments

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)
- [OpenAPI](openapi/affirm-disputes-openapi.yml)
- [JSONSchema](json-schema/affirm-dispute-schema.json)

### Affirm Cards API
The Affirm Cards API enables merchants to create and manage virtual card (VCN) transactions for Affirm Lite integrations. It supports creating, reading, finalizing, and canceling virtual cards that can be used anywhere major credit cards are accepted, providing a seamless buy now pay later experience without requiring direct API integration for the merchant's payment processor.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Cards, Fintech, Payments, Virtual Card

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)

### Affirm Files API
The Affirm Files API provides endpoints for uploading supporting documentation that can be attached as evidence when responding to payment disputes. It is used in conjunction with the Disputes API to submit files such as receipts, order confirmations, shipping records, or customer communications.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Disputes, Files, Fintech, Uploads

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)

### Affirm Prequalification API
The Affirm Prequalification API allows merchants to check whether a customer is prequalified for Affirm financing before they reach checkout. This enables merchants to surface Affirm messaging and financing options only to eligible customers, improving conversion rates and customer experience across the shopping journey.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Buy Now Pay Later, Credit, Fintech, Prequalification

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)

### Affirm iOS SDK
The Affirm iOS SDK provides a native library for integrating Affirm buy now pay later checkout into iOS applications. It handles presenting the Affirm checkout flow within a mobile webview and returning the checkout token to the host app upon customer authorization. The SDK supports Swift and Objective-C and includes components for rendering Affirm promotional messaging within native iOS UI.

**Human URL:** [https://docs.affirm.com/developers/docs/ios-sdk-overview](https://docs.affirm.com/developers/docs/ios-sdk-overview)

#### Tags:

 - Buy Now Pay Later, iOS, Mobile, Objective-C, SDK, Swift

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/ios-sdk-overview)
- [SDK](https://github.com/Affirm/affirm-merchant-sdk-ios)

### Affirm Android SDK
The Affirm Android SDK provides a native library for embedding the Affirm buy now pay later checkout experience into Android applications. It manages the checkout webview flow, handles deep link callbacks, and returns a checkout token to the host application upon successful customer authorization. The SDK supports Java and Kotlin and includes components for displaying Affirm promotional messaging within native Android UI.

**Human URL:** [https://docs.affirm.com/developers/docs/android-sdk-overview](https://docs.affirm.com/developers/docs/android-sdk-overview)

#### Tags:

 - Android, Buy Now Pay Later, Java, Kotlin, Mobile, SDK

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/android-sdk-overview)
- [SDK](https://github.com/Affirm/affirm-merchant-sdk-android)

## Common Properties

- [AsyncAPI](asyncapi/affirm-webhooks-asyncapi.yml)
- [JSON-LD](json-ld/affirm-context.jsonld)
- [Portal](https://docs.affirm.com)
- [GettingStarted](https://docs.affirm.com/developers/docs/home-introduction)
- [Authentication](https://docs.affirm.com/developers/docs/authentication)
- [RateLimits](https://docs.affirm.com/developers/docs/rate-limits)
- [SignUp](https://www.affirm.com/business)
- [StatusPage](https://status.affirm.com)
- [GitHubOrganization](https://github.com/Affirm)
- [TermsOfService](https://www.affirm.com/merchant-tos)
- [PrivacyPolicy](https://www.affirm.com/privacy)
- [Support](https://docs.affirm.com/developers/docs/get-support)
- [JSONSchema](json-schema/affirm-checkout-schema.json)
- [JSONSchema](json-schema/affirm-dispute-schema.json)
- [JSONSchema](json-schema/affirm-transaction-schema.json)
- [JSONSchema](json-schema/checkout-address-object-schema.json)
- [JSONSchema](json-schema/checkout-checkout-request-schema.json)
- [JSONSchema](json-schema/checkout-checkout-schema.json)
- [JSONSchema](json-schema/checkout-contact-object-schema.json)
- [JSONSchema](json-schema/checkout-discount-object-schema.json)

## Features

| Name | Description |
|------|-------------|
| Buy Now Pay Later | Enable customers to split purchases into installments with 0% APR options and flexible financing terms at checkout. |
| Adaptive Checkout | Dynamically present the best financing option (Installments, Pay in 4, etc.) to each customer based on eligibility. |
| Virtual Card Network | Issue virtual cards via Affirm Lite so customers can use BNPL anywhere major credit cards are accepted without direct API integration. |
| Split Capture | Capture funds from a single Affirm transaction across multiple shipments or fulfillment events. |
| Promotional Messaging | Display "as low as" monthly payment messaging on product, cart, and homepage views to increase conversion. |
| Prequalification | Check customer eligibility for Affirm financing before checkout to surface relevant offers and improve conversion. |
| Webhook Notifications | Receive real-time event notifications for key transaction lifecycle events including authorization, capture, void, and refund. |
| Dispute Management | Programmatically manage payment disputes by submitting evidence and tracking dispute status via API. |
| Global Integration | Support for merchants in the USA, Canada, and UK with international market configuration. |

## Use Cases

| Name | Description |
|------|-------------|
| E-Commerce Checkout | Embed Affirm BNPL directly in the checkout flow of an online store to offer customers flexible payment options at the point of purchase. |
| Mobile Commerce | Integrate Affirm financing into iOS and Android apps using native mobile SDKs for a seamless in-app BNPL experience. |
| Telesales and Assisted Selling | Send checkout links via SMS or email to allow customers to complete Affirm-financed purchases over the phone or remotely. |
| In-Store Retail | Enable Affirm BNPL in physical retail environments using virtual card or POS integration flows. |
| Transaction Reconciliation | Use the Transactions API to retrieve settlement events and reconcile captured payments against disbursements. |
| Dispute Resolution | Automate dispute response workflows by programmatically fetching dispute records and submitting evidence via the Disputes API. |
| Promotional Marketing | Use the Promos API to display dynamic financing terms on product pages to increase cart size and conversion. |

## Integrations

| Name | Description |
|------|-------------|
| Shopify | Affirm is available as a payment provider plugin for Shopify merchants, enabling BNPL at Shopify-powered checkouts. |
| BigCommerce | Native Affirm integration for BigCommerce stores, providing BNPL checkout without custom API development. |
| WooCommerce | Affirm plugin for WooCommerce-powered WordPress stores enables BNPL payment options. |
| Salesforce Commerce Cloud | Affirm integration for Salesforce Commerce Cloud (SFCC) enterprise e-commerce deployments. |
| Magento | Affirm integration for Magento (Adobe Commerce) merchants to enable BNPL checkout. |
| Stripe | Affirm is available as a payment method through the Stripe payment platform. |
| Braintree | Affirm BNPL is accessible via the Braintree payment gateway for merchants using PayPal infrastructure. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [affirm-checkout-openapi](openapi/affirm-checkout-openapi.yml)
- [affirm-direct-api-openapi](openapi/affirm-direct-api-openapi.yml)
- [affirm-disputes-openapi](openapi/affirm-disputes-openapi.yml)
- [affirm-promos-openapi](openapi/affirm-promos-openapi.yml)
- [affirm-transactions-openapi](openapi/affirm-transactions-openapi.yml)

### AsyncAPI

- [affirm-webhooks-asyncapi](asyncapi/affirm-webhooks-asyncapi.yml)

### JSON Schema

- [affirm-checkout-schema](json-schema/affirm-checkout-schema.json)
- [affirm-dispute-schema](json-schema/affirm-dispute-schema.json)
- [affirm-transaction-schema](json-schema/affirm-transaction-schema.json)
- [checkout-address-object-schema](json-schema/checkout-address-object-schema.json)
- [checkout-checkout-request-schema](json-schema/checkout-checkout-request-schema.json)
- [checkout-checkout-schema](json-schema/checkout-checkout-schema.json)
- [checkout-contact-object-schema](json-schema/checkout-contact-object-schema.json)
- [checkout-discount-object-schema](json-schema/checkout-discount-object-schema.json)
- [checkout-item-object-schema](json-schema/checkout-item-object-schema.json)
- [checkout-merchant-object-schema](json-schema/checkout-merchant-object-schema.json)
- [checkout-name-object-schema](json-schema/checkout-name-object-schema.json)
- [checkout-store-object-schema](json-schema/checkout-store-object-schema.json)
- [direct-api-card-schema](json-schema/direct-api-card-schema.json)
- [direct-api-file-object-schema](json-schema/direct-api-file-object-schema.json)
- [direct-api-transaction-schema](json-schema/direct-api-transaction-schema.json)
- [disputes-dispute-schema](json-schema/disputes-dispute-schema.json)
- [disputes-evidence-item-schema](json-schema/disputes-evidence-item-schema.json)
- [disputes-evidence-request-schema](json-schema/disputes-evidence-request-schema.json)
- [promos-financing-term-schema](json-schema/promos-financing-term-schema.json)
- [promos-offer-content-schema](json-schema/promos-offer-content-schema.json)
- [promos-promo-config-schema](json-schema/promos-promo-config-schema.json)
- [promos-promo-content-schema](json-schema/promos-promo-content-schema.json)
- [promos-promo-response-schema](json-schema/promos-promo-response-schema.json)
- [transactions-settlement-event-schema](json-schema/transactions-settlement-event-schema.json)
- [transactions-settlement-event-summary-schema](json-schema/transactions-settlement-event-summary-schema.json)
- [transactions-transaction-event-schema](json-schema/transactions-transaction-event-schema.json)
- [transactions-transaction-schema](json-schema/transactions-transaction-schema.json)

### JSON Structure

- [affirm-checkout-structure](json-structure/affirm-checkout-structure.json)
- [affirm-dispute-structure](json-structure/affirm-dispute-structure.json)
- [affirm-transaction-structure](json-structure/affirm-transaction-structure.json)
- [checkout-address-object-structure](json-structure/checkout-address-object-structure.json)
- [checkout-checkout-request-structure](json-structure/checkout-checkout-request-structure.json)
- [checkout-checkout-structure](json-structure/checkout-checkout-structure.json)
- [checkout-contact-object-structure](json-structure/checkout-contact-object-structure.json)
- [checkout-discount-object-structure](json-structure/checkout-discount-object-structure.json)
- [checkout-item-object-structure](json-structure/checkout-item-object-structure.json)
- [checkout-merchant-object-structure](json-structure/checkout-merchant-object-structure.json)
- [checkout-name-object-structure](json-structure/checkout-name-object-structure.json)
- [checkout-store-object-structure](json-structure/checkout-store-object-structure.json)
- [direct-api-card-structure](json-structure/direct-api-card-structure.json)
- [direct-api-file-object-structure](json-structure/direct-api-file-object-structure.json)
- [direct-api-transaction-structure](json-structure/direct-api-transaction-structure.json)
- [disputes-dispute-structure](json-structure/disputes-dispute-structure.json)
- [disputes-evidence-item-structure](json-structure/disputes-evidence-item-structure.json)
- [disputes-evidence-request-structure](json-structure/disputes-evidence-request-structure.json)
- [promos-financing-term-structure](json-structure/promos-financing-term-structure.json)
- [promos-offer-content-structure](json-structure/promos-offer-content-structure.json)
- [promos-promo-config-structure](json-structure/promos-promo-config-structure.json)
- [promos-promo-content-structure](json-structure/promos-promo-content-structure.json)
- [promos-promo-response-structure](json-structure/promos-promo-response-structure.json)
- [transactions-settlement-event-structure](json-structure/transactions-settlement-event-structure.json)
- [transactions-settlement-event-summary-structure](json-structure/transactions-settlement-event-summary-structure.json)
- [transactions-transaction-event-structure](json-structure/transactions-transaction-event-structure.json)
- [transactions-transaction-structure](json-structure/transactions-transaction-structure.json)

### JSON-LD

- [affirm-checkout-context](json-ld/affirm-checkout-context.jsonld)
- [affirm-context](json-ld/affirm-context.jsonld)
- [affirm-direct-context](json-ld/affirm-direct-context.jsonld)
- [affirm-disputes-context](json-ld/affirm-disputes-context.jsonld)
- [affirm-promos-context](json-ld/affirm-promos-context.jsonld)
- [affirm-transactions-context](json-ld/affirm-transactions-context.jsonld)

### Examples

- [affirm-checkout-example](examples/affirm-checkout-example.json)
- [affirm-dispute-example](examples/affirm-dispute-example.json)
- [affirm-transaction-example](examples/affirm-transaction-example.json)
- [checkout-address-object-example](examples/checkout-address-object-example.json)
- [checkout-checkout-example](examples/checkout-checkout-example.json)
- [checkout-checkout-request-example](examples/checkout-checkout-request-example.json)
- [checkout-contact-object-example](examples/checkout-contact-object-example.json)
- [checkout-discount-object-example](examples/checkout-discount-object-example.json)
- [checkout-item-object-example](examples/checkout-item-object-example.json)
- [checkout-merchant-object-example](examples/checkout-merchant-object-example.json)
- [checkout-name-object-example](examples/checkout-name-object-example.json)
- [checkout-store-object-example](examples/checkout-store-object-example.json)
- [direct-api-card-example](examples/direct-api-card-example.json)
- [direct-api-file-object-example](examples/direct-api-file-object-example.json)
- [direct-api-transaction-example](examples/direct-api-transaction-example.json)
- [disputes-dispute-example](examples/disputes-dispute-example.json)
- [disputes-evidence-item-example](examples/disputes-evidence-item-example.json)
- [disputes-evidence-request-example](examples/disputes-evidence-request-example.json)
- [promos-financing-term-example](examples/promos-financing-term-example.json)
- [promos-offer-content-example](examples/promos-offer-content-example.json)
- [promos-promo-config-example](examples/promos-promo-config-example.json)
- [promos-promo-content-example](examples/promos-promo-content-example.json)
- [promos-promo-response-example](examples/promos-promo-response-example.json)
- [transactions-settlement-event-example](examples/transactions-settlement-event-example.json)
- [transactions-settlement-event-summary-example](examples/transactions-settlement-event-summary-example.json)
- [transactions-transaction-event-example](examples/transactions-transaction-event-example.json)
- [transactions-transaction-example](examples/transactions-transaction-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [checkout](capabilities/shared/checkout.yaml)
- [disputes](capabilities/shared/disputes.yaml)
- [promos](capabilities/shared/promos.yaml)
- [transactions](capabilities/shared/transactions.yaml)

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Affirm Payment Management](capabilities/payment-management.yaml) | affirm-checkout, affirm-transactions, affirm-disputes, affirm-promos | 11 | Merchant Engineer |

## Vocabulary

- [Affirm Vocabulary](vocabulary/affirm-vocabulary.yaml) — Unified taxonomy mapping resources, actions, workflows, and personas across operational and capability dimensions

## Rules

- [affirm-spectral-rules](rules/affirm-spectral-rules.yml) — 35 rules enforcing Affirm API conventions

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com

# Affirm (affirm)
Affirm is a buy now pay later fintech company that enables consumers to split purchases into installment payments at checkout. Affirm provides a developer platform with APIs and SDKs that allow merchants to integrate Affirm financing directly into their websites and mobile applications, supporting the full payment lifecycle from checkout through settlement, dispute management, and promotional messaging.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/apis.yml)

## Scope
- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Buy Now Pay Later, Payments, Fintech, Checkout, Merchant

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-03-21

## APIs

### Affirm Direct API
The Affirm Direct API is a flexible integration that allows merchants to embed the full Affirm checkout and payment authorization flow directly into their website, giving complete control over the front-end user experience and back-end transaction processing logic. It supports inline checkout via modal or redirect to affirm.com, and handles the full transaction lifecycle including authorization, capture, void, and refund operations. Merchants interact with a sandbox environment at sandbox.affirm.com for development and testing before deploying to the live api.affirm.com endpoint. Authentication is handled via API keys available from the Affirm Merchant Portal.

**Human URL:** [https://docs.affirm.com/payments/docs/direct-api-overview](https://docs.affirm.com/payments/docs/direct-api-overview)

#### Tags:

 - Buy Now Pay Later, Payments, Checkout, Fintech, Merchant

#### Properties

- [Documentation](https://docs.affirm.com/payments/docs/direct-api-overview)
- [OpenAPI](openapi/affirm-direct-api-openapi.yml)

### Affirm Checkout API
The Affirm Checkout API enables merchants to initiate and manage the Affirm buy now pay later checkout flow for customers at the point of purchase. It provides endpoints to create checkout sessions, read and update checkout objects, and store checkout tokens returned after a customer completes the Affirm financing application. The API supports both redirect and direct checkout integration patterns, and includes endpoints for resending checkout links via email or SMS. Once a customer authorizes a loan, the resulting checkout token is exchanged server-side to complete the transaction authorization.

**Human URL:** [https://docs.affirm.com/developers/docs/home-introduction](https://docs.affirm.com/developers/docs/home-introduction)

#### Tags:

 - Checkout, Buy Now Pay Later, Payments, Fintech, Merchant

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/home-introduction)
- [OpenAPI](openapi/affirm-checkout-openapi.yml)
- [JSONSchema](json-schema/affirm-checkout-schema.json)

### Affirm Transactions API
The Affirm Transactions API provides server-side endpoints for managing the full lifecycle of Affirm payment transactions after a customer completes checkout. It supports authorization, capture, void, and refund operations, as well as listing and retrieving transaction details and associated settlement events. Merchants use this API to reconcile charges, process partial or full refunds, and track disbursement activity. The API uses HTTPS with API key authentication and communicates using JSON, with separate sandbox and live base URLs for development and production use.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Transactions, Payments, Authorization, Capture, Refunds, Fintech

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)
- [OpenAPI](openapi/affirm-transactions-openapi.yml)
- [JSONSchema](json-schema/affirm-transaction-schema.json)

### Affirm Promos API
The Affirm Promos API is a server-side endpoint that enables merchants to render dynamic promotional pricing text and present Affirm-hosted educational modals on their website. It accepts a purchase amount and returns financing terms, "as low as" monthly payment messaging, APR rates, and modal content including headlines, descriptions, and legal disclosures. The API supports multiple installment term options and page-type context (product, cart, homepage) to customize the displayed messaging. Merchants authenticate requests using their public API key appended to the base URL path.

**Human URL:** [https://docs.affirm.com/developers/docs/promos-api-integration-overview](https://docs.affirm.com/developers/docs/promos-api-integration-overview)

#### Tags:

 - Promotions, Messaging, Marketing, Buy Now Pay Later, Merchant

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/promos-api-integration-overview)
- [OpenAPI](openapi/affirm-promos-openapi.yml)

### Affirm Disputes API
The Affirm Disputes API (V3) provides merchants with programmatic access to manage payment disputes initiated by customers. It supports listing and retrieving individual dispute records, submitting evidence to contest a dispute, and closing disputes. The API integrates with the file upload capability so merchants can attach supporting documentation as evidence when responding to disputes. This interface allows merchants to handle chargeback workflows programmatically rather than relying solely on the Merchant Portal UI.

**Human URL:** [https://docs.affirm.com/developers/reference/introduction](https://docs.affirm.com/developers/reference/introduction)

#### Tags:

 - Disputes, Chargebacks, Payments, Fintech, Merchant

#### Properties

- [Documentation](https://docs.affirm.com/developers/reference/introduction)
- [OpenAPI](openapi/affirm-disputes-openapi.yml)
- [JSONSchema](json-schema/affirm-dispute-schema.json)

### Affirm iOS SDK
The Affirm iOS SDK provides a native library for integrating Affirm buy now pay later checkout into iOS applications. It handles presenting the Affirm checkout flow within a mobile webview and returning the checkout token to the host app upon customer authorization. The SDK supports Swift and Objective-C and includes components for rendering Affirm promotional messaging within native iOS UI. After the customer completes the Affirm flow, the merchant app passes the checkout token to its server to finalize the transaction via the Affirm server-side API.

**Human URL:** [https://docs.affirm.com/developers/docs/ios-sdk-overview](https://docs.affirm.com/developers/docs/ios-sdk-overview)

#### Tags:

 - iOS, Mobile, SDK, Swift, Objective-C, Buy Now Pay Later

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/ios-sdk-overview)

### Affirm Android SDK
The Affirm Android SDK provides a native library for embedding the Affirm buy now pay later checkout experience into Android applications. It manages the checkout webview flow, handles deep link callbacks, and returns a checkout token to the host application upon successful customer authorization. The SDK supports Java and Kotlin and includes components for displaying Affirm promotional messaging within native Android UI. The checkout token returned by the SDK is passed to the merchant's server to complete the transaction using the Affirm server-side API.

**Human URL:** [https://docs.affirm.com/developers/docs/android-sdk-overview](https://docs.affirm.com/developers/docs/android-sdk-overview)

#### Tags:

 - Android, Mobile, SDK, Java, Kotlin, Buy Now Pay Later

#### Properties

- [Documentation](https://docs.affirm.com/developers/docs/android-sdk-overview)

## Common Properties

- [Portal](https://docs.affirm.com/developers/docs/home-introduction)
- [Documentation](https://docs.affirm.com/developers/docs/home-introduction)
- [Website](https://www.affirm.com/)
- [Login](https://merchant.affirm.com/login)
- [Blog](https://www.affirm.com/blog)
- [PrivacyPolicy](https://www.affirm.com/privacy)
- [TermsOfService](https://www.affirm.com/terms)
- [Support](https://helpcenter.affirm.com/)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com

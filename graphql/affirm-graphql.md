# Affirm GraphQL Schema

This document describes the conceptual GraphQL schema for the Affirm Buy Now Pay Later (BNPL) platform. Affirm's production API is REST-based; this schema models the same domain objects and operations in GraphQL terms for integration planning, tooling, and documentation purposes.

## Overview

Affirm provides merchant-facing APIs for checkout initiation, charge capture, voids, refunds, and transaction/settlement reporting. The schema covers the full lifecycle of a BNPL transaction from cart creation through installment scheduling and settlement.

## Reference

- Developer Docs: https://docs.affirm.com/affirm-developers/reference
- Human URL: https://docs.affirm.com/developers
- Base URL: https://api.affirm.com

## Schema File

See `affirm-schema.graphql` in this directory for the full type definitions.

## Key Types

### Checkout Flow
- `Checkout` / `CheckoutDetails` / `CheckoutStatus` / `CheckoutToken` — initiate and track a consumer checkout session
- `Cart` / `CartDetails` / `CartItem` — line-item representation of the shopping cart
- `Discount` — discount amounts applied to the cart
- `Shipping` / `ShippingDetails` / `Address` — delivery information

### Consumer
- `Consumer` / `ConsumerDetails` / `ConsumerVerification` — the borrower identity and verification state
- `Decision` / `DecisionDetails` / `DecisionReason` — underwriting outcome and reason codes

### Charges & Transactions
- `Charge` / `ChargeDetails` — the core financial instrument created after checkout authorization
- `Capture` / `CaptureDetails` — settlement of a charge against a fulfilled order
- `Void` / `VoidDetails` — cancellation of an authorized charge
- `Refund` / `RefundDetails` — partial or full return of captured funds
- `Transaction` / `TransactionDetails` / `TransactionStatus` / `TransactionType` — unified transaction ledger entry

### Loan & Installments
- `Loan` / `LoanDetails` / `LoanStatus` / `LoanAmount` / `LoanTerm` / `LoanFee` — the consumer loan record
- `Installment` / `InstallmentDetails` / `Schedule` / `PaymentSchedule` — repayment plan breakdown

### Authorization
- `Authorization` / `AuthorizationDetails` — pre-authorization hold on a charge

### Orders
- `Order` / `OrderDetails` / `OrderItem` / `ItemDetails` — merchant order and line-item detail

### Settlement & Reporting
- `Settlement` / `SettlementDetails` — daily/weekly settlement disbursement to the merchant

### Merchant Configuration
- `Merchant` / `MerchantDetails` / `MerchantConfig` — merchant account and configuration settings

### Webhooks & Security
- `Webhook` / `WebhookEvent` — event delivery configuration and payloads
- `APIKey` / `Token` — authentication credentials

## Queries

- `checkout(token: String!)` — retrieve a checkout session by token
- `charge(chargeId: String!)` — retrieve a charge record
- `transaction(transactionId: String!)` — retrieve a transaction
- `loan(loanId: String!)` — retrieve a loan record
- `order(orderId: String!)` — retrieve an order
- `settlement(settlementId: String!)` — retrieve a settlement record
- `merchant(merchantId: String!)` — retrieve merchant details
- `transactions(filter: TransactionFilterInput)` — list transactions with filtering
- `settlements(filter: SettlementFilterInput)` — list settlement records

## Mutations

- `createCheckout(input: CreateCheckoutInput!)` — initiate a new checkout session
- `captureCharge(chargeId: String!, input: CaptureInput!)` — capture an authorized charge
- `voidCharge(chargeId: String!)` — void an authorized charge
- `refundCharge(chargeId: String!, input: RefundInput!)` — refund a captured charge
- `updateOrder(orderId: String!, input: UpdateOrderInput!)` — update order line items
- `createWebhook(input: CreateWebhookInput!)` — register a webhook endpoint
- `deleteWebhook(webhookId: String!)` — remove a webhook endpoint

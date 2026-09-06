
# MerchantReceiptResponse

Receipt response for the merchant audience (dashboard, merchant API keys).  Excludes customer-upload-pipeline fields (uploaded_file_url, file_size, file_type, original_filename, extraction_status/confidence/method/ completed_at, receipt_source, uploaded_by_customer_id), which are always null for merchant-issued receipts and belong to the separate customer-audience response shape instead.

## Properties

Name | Type
------------ | -------------
`id` | string
`publicToken` | string
`barcode` | [Barcode](Barcode.md)
`merchantReceiptId` | string
`merchantName` | string
`merchantLogo` | string
`storeId` | string
`organisationId` | string
`transactionDate` | Date
`orderNumber` | string
`cashier` | string
`items` | [Array&lt;ReceiptItemResponse&gt;](ReceiptItemResponse.md)
`subtotal` | string
`taxAmount` | string
`discountAmount` | string
`tipAmount` | string
`totalAmount` | string
`currency` | string
`paymentInfo` | [Array&lt;PaymentInfoResponse&gt;](PaymentInfoResponse.md)
`qrCodeUrl` | string
`qrToken` | string
`qrExpiresAt` | Date
`receiptUrl` | string
`pdfUrl` | string
`notes` | string
`returnPolicy` | string
`offers` | Array&lt;string&gt;
`offerPolicies` | [Array&lt;OfferPolicyInfo&gt;](OfferPolicyInfo.md)
`feedbackUrl` | string
`loyaltyInfo` | string
`merchantDetails` | [MerchantDetails](MerchantDetails.md)
`adjustments` | [Array&lt;ReceiptAdjustment&gt;](ReceiptAdjustment.md)
`transactionReferences` | [Array&lt;TransactionReference&gt;](TransactionReference.md)
`warranties` | [Array&lt;WarrantyInfo&gt;](WarrantyInfo.md)
`insights` | [ReceiptInsights](ReceiptInsights.md)
`returnInsights` | [ReturnInsights](ReturnInsights.md)
`accessCount` | number
`lastAccessed` | Date
`status` | string
`expiresAt` | Date
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { MerchantReceiptResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "publicToken": null,
  "barcode": null,
  "merchantReceiptId": null,
  "merchantName": null,
  "merchantLogo": null,
  "storeId": null,
  "organisationId": null,
  "transactionDate": null,
  "orderNumber": null,
  "cashier": null,
  "items": null,
  "subtotal": 12.99,
  "taxAmount": 12.99,
  "discountAmount": 12.99,
  "tipAmount": 12.99,
  "totalAmount": 12.99,
  "currency": null,
  "paymentInfo": null,
  "qrCodeUrl": null,
  "qrToken": null,
  "qrExpiresAt": null,
  "receiptUrl": null,
  "pdfUrl": null,
  "notes": null,
  "returnPolicy": null,
  "offers": null,
  "offerPolicies": null,
  "feedbackUrl": null,
  "loyaltyInfo": null,
  "merchantDetails": null,
  "adjustments": null,
  "transactionReferences": null,
  "warranties": null,
  "insights": null,
  "returnInsights": null,
  "accessCount": null,
  "lastAccessed": null,
  "status": null,
  "expiresAt": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies MerchantReceiptResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MerchantReceiptResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



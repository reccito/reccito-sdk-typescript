
# ReceiptCreate

Receipt creation request.

## Properties

Name | Type
------------ | -------------
`merchantReceiptId` | string
`dedupeKey` | string
`barcode` | [Barcode](Barcode.md)
`storeId` | string
`transactionDate` | Date
`orderNumber` | string
`cashier` | string
`items` | [Array&lt;ReceiptItemCreate&gt;](ReceiptItemCreate.md)
`subtotal` | string
`taxAmount` | string
`discountAmount` | string
`tipAmount` | string
`totalAmount` | string
`currency` | string
`paymentInfo` | [Array&lt;PaymentInfoCreate&gt;](PaymentInfoCreate.md)
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
`qrExpiryMinutes` | number

## Example

```typescript
import type { ReceiptCreate } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "merchantReceiptId": null,
  "dedupeKey": null,
  "barcode": null,
  "storeId": null,
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
  "qrExpiryMinutes": null,
} satisfies ReceiptCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



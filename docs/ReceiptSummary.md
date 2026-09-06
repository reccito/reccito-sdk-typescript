
# ReceiptSummary

Slim receipt shape for the paginated merchant list endpoint -- omits qr_code_url, items, payment_info, adjustments, warranties, and insights to keep list responses lightweight. Fetch GET /merchant/receipts/{id} for the full detail (QR code included) when a single receipt is opened.

## Properties

Name | Type
------------ | -------------
`id` | string
`publicToken` | string
`merchantReceiptId` | string
`storeId` | string
`organisationId` | string
`transactionDate` | Date
`totalAmount` | string
`currency` | string
`itemCount` | number
`status` | string
`accessCount` | number
`receiptUrl` | string
`createdAt` | Date

## Example

```typescript
import type { ReceiptSummary } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "publicToken": null,
  "merchantReceiptId": null,
  "storeId": null,
  "organisationId": null,
  "transactionDate": null,
  "totalAmount": 12.99,
  "currency": null,
  "itemCount": null,
  "status": null,
  "accessCount": null,
  "receiptUrl": null,
  "createdAt": null,
} satisfies ReceiptSummary

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptSummary
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



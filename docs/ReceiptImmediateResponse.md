
# ReceiptImmediateResponse

Immediate receipt response for fast QR code generation.

## Properties

Name | Type
------------ | -------------
`id` | string
`publicToken` | string
`barcode` | [Barcode](Barcode.md)
`merchantReceiptId` | string
`storeId` | string
`organisationId` | string
`qrCodeUrl` | string
`qrToken` | string
`qrExpiresAt` | Date
`receiptUrl` | string
`transactionDate` | Date
`totalAmount` | string
`currency` | string
`processingStatus` | string
`createdAt` | Date

## Example

```typescript
import type { ReceiptImmediateResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "publicToken": null,
  "barcode": null,
  "merchantReceiptId": null,
  "storeId": null,
  "organisationId": null,
  "qrCodeUrl": null,
  "qrToken": null,
  "qrExpiresAt": null,
  "receiptUrl": null,
  "transactionDate": null,
  "totalAmount": 12.99,
  "currency": null,
  "processingStatus": null,
  "createdAt": null,
} satisfies ReceiptImmediateResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptImmediateResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# Barcode

Barcode. Used both as the request shape (ReceiptCreate.barcode) and the response shape (see MerchantReceiptResponse/CustomerReceiptDetailResponse/ ReceiptImmediateResponse.barcode). `code` is required: a Barcode object with no code is meaningless.

## Properties

Name | Type
------------ | -------------
`code` | string
`format` | string

## Example

```typescript
import type { Barcode } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "format": null,
} satisfies Barcode

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Barcode
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



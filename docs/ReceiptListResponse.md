
# ReceiptListResponse

Receipt list response with pagination (merchant audience).

## Properties

Name | Type
------------ | -------------
`receipts` | [Array&lt;ReceiptSummary&gt;](ReceiptSummary.md)
`total` | number
`page` | number
`limit` | number
`hasNext` | boolean
`hasPrev` | boolean

## Example

```typescript
import type { ReceiptListResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "receipts": null,
  "total": null,
  "page": null,
  "limit": null,
  "hasNext": null,
  "hasPrev": null,
} satisfies ReceiptListResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptListResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



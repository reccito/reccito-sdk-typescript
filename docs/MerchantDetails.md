
# MerchantDetails

Merchant details parsed from receipt.

## Properties

Name | Type
------------ | -------------
`name` | string
`address` | string
`taxId` | string
`contactPhone` | string
`contactEmail` | string
`website` | string

## Example

```typescript
import type { MerchantDetails } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "address": null,
  "taxId": null,
  "contactPhone": null,
  "contactEmail": null,
  "website": null,
} satisfies MerchantDetails

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MerchantDetails
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



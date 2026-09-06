
# OfferPolicyInfo

Offer metadata with optional validity window.

## Properties

Name | Type
------------ | -------------
`offerText` | string
`offerEndDate` | Date
`terms` | string

## Example

```typescript
import type { OfferPolicyInfo } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "offerText": null,
  "offerEndDate": null,
  "terms": null,
} satisfies OfferPolicyInfo

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as OfferPolicyInfo
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



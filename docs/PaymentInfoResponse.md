
# PaymentInfoResponse

Payment information response.

## Properties

Name | Type
------------ | -------------
`method` | string
`amount` | string
`cardLastFour` | string
`reference` | string

## Example

```typescript
import type { PaymentInfoResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "method": null,
  "amount": 12.99,
  "cardLastFour": null,
  "reference": null,
} satisfies PaymentInfoResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PaymentInfoResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# ReceiptInsights

Actionable insights derived from receipt text.

## Properties

Name | Type
------------ | -------------
`returnWindowDays` | number
`returnDeadline` | Date
`refundEligible` | boolean
`warrantyItems` | [Array&lt;WarrantyInfo&gt;](WarrantyInfo.md)

## Example

```typescript
import type { ReceiptInsights } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "returnWindowDays": null,
  "returnDeadline": null,
  "refundEligible": null,
  "warrantyItems": null,
} satisfies ReceiptInsights

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptInsights
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



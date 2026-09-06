
# ReceiptAdjustment

Price adjustment on line-item or receipt total.

## Properties

Name | Type
------------ | -------------
`scope` | string
`kind` | string
`label` | string
`amount` | string
`itemName` | string

## Example

```typescript
import type { ReceiptAdjustment } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "scope": null,
  "kind": null,
  "label": null,
  "amount": 12.99,
  "itemName": null,
} satisfies ReceiptAdjustment

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptAdjustment
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



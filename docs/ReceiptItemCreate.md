
# ReceiptItemCreate

Receipt line item creation.

## Properties

Name | Type
------------ | -------------
`name` | string
`quantity` | number
`unitPrice` | string
`totalPrice` | string
`description` | string
`sku` | string
`category` | string

## Example

```typescript
import type { ReceiptItemCreate } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "quantity": null,
  "unitPrice": 12.99,
  "totalPrice": 12.99,
  "description": null,
  "sku": null,
  "category": null,
} satisfies ReceiptItemCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReceiptItemCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# TransactionReference

Receipt identifiers like auth code, ARN, invoice id.

## Properties

Name | Type
------------ | -------------
`key` | string
`value` | string

## Example

```typescript
import type { TransactionReference } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "key": null,
  "value": null,
} satisfies TransactionReference

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TransactionReference
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



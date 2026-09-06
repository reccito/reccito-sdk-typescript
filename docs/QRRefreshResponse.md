
# QRRefreshResponse

QR code refresh response.

## Properties

Name | Type
------------ | -------------
`receiptId` | string
`newQrToken` | string
`newQrCodeUrl` | string
`expiresAt` | Date

## Example

```typescript
import type { QRRefreshResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "receiptId": null,
  "newQrToken": null,
  "newQrCodeUrl": null,
  "expiresAt": null,
} satisfies QRRefreshResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as QRRefreshResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



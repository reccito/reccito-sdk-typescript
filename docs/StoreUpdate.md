
# StoreUpdate

Store update request.

## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`state` | string
`postalCode` | string
`country` | string
`latitude` | string
`longitude` | string
`phone` | string
`email` | string
`managerName` | string
`timezone` | string
`defaultQrExpiryMinutes` | number
`logoUrl` | string
`primaryColor` | string
`isActive` | boolean
`openingHours` | { [key: string]: any; }
`customMetadata` | { [key: string]: any; }

## Example

```typescript
import type { StoreUpdate } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "state": null,
  "postalCode": null,
  "country": null,
  "latitude": null,
  "longitude": null,
  "phone": null,
  "email": null,
  "managerName": null,
  "timezone": null,
  "defaultQrExpiryMinutes": null,
  "logoUrl": null,
  "primaryColor": null,
  "isActive": null,
  "openingHours": null,
  "customMetadata": null,
} satisfies StoreUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StoreUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



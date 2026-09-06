
# StoreResponse

Store response.

## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`code` | string
`description` | string
`organisationId` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`state` | string
`postalCode` | string
`country` | string
`fullAddress` | string
`latitude` | string
`longitude` | string
`phone` | string
`email` | string
`managerName` | string
`timezone` | string
`defaultQrExpiryMinutes` | number
`effectiveQrExpiry` | number
`logoUrl` | string
`primaryColor` | string
`effectiveLogoUrl` | string
`effectivePrimaryColor` | string
`isActive` | boolean
`openingHours` | { [key: string]: any; }
`receiptsCreatedCount` | number
`lastReceiptCreated` | Date
`customMetadata` | { [key: string]: any; }
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { StoreResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "code": null,
  "description": null,
  "organisationId": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "state": null,
  "postalCode": null,
  "country": null,
  "fullAddress": null,
  "latitude": null,
  "longitude": null,
  "phone": null,
  "email": null,
  "managerName": null,
  "timezone": null,
  "defaultQrExpiryMinutes": null,
  "effectiveQrExpiry": null,
  "logoUrl": null,
  "primaryColor": null,
  "effectiveLogoUrl": null,
  "effectivePrimaryColor": null,
  "isActive": null,
  "openingHours": null,
  "receiptsCreatedCount": null,
  "lastReceiptCreated": null,
  "customMetadata": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies StoreResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StoreResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# StoreStatsResponse

Store statistics.

## Properties

Name | Type
------------ | -------------
`storeId` | string
`storeName` | string
`receiptsCreatedCount` | number
`receiptsCreatedToday` | number
`receiptsCreatedThisMonth` | number
`qrScansCount` | number
`qrScansToday` | number
`qrScansThisMonth` | number
`totalAmountThisMonth` | string
`averageReceiptAmount` | string
`lastReceiptCreated` | Date
`busiestHour` | string
`busiestDay` | string

## Example

```typescript
import type { StoreStatsResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "storeId": null,
  "storeName": null,
  "receiptsCreatedCount": null,
  "receiptsCreatedToday": null,
  "receiptsCreatedThisMonth": null,
  "qrScansCount": null,
  "qrScansToday": null,
  "qrScansThisMonth": null,
  "totalAmountThisMonth": null,
  "averageReceiptAmount": null,
  "lastReceiptCreated": null,
  "busiestHour": null,
  "busiestDay": null,
} satisfies StoreStatsResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as StoreStatsResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# ReturnInsights

Return-centric actionable insights.

## Properties

Name | Type
------------ | -------------
`returnable` | boolean
`returnWindowDays` | number
`returnDeadline` | Date
`daysLeft` | number
`policySummary` | string

## Example

```typescript
import type { ReturnInsights } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "returnable": null,
  "returnWindowDays": null,
  "returnDeadline": null,
  "daysLeft": null,
  "policySummary": null,
} satisfies ReturnInsights

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReturnInsights
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# ModelApiResponse

Standard API response format.  All API responses should follow this format for consistency. The \'data\' field contains the response payload, while \'error\' is populated when an error occurs. Pagination is included for list endpoints.  Example:     Success response:     {         \"data\": {\"id\": \"123\", \"name\": \"Logo\"},         \"pagination\": {\"page\": 1, \"limit\": 10, \"total\": 100, \"has_next\": true}     }      Error response:     {         \"error\": {             \"code\": \"VALIDATION_ERROR\",             \"message\": \"File size exceeds 5MB limit\",             \"details\": {\"max_size\": \"5242880\"}         }     }

## Properties

Name | Type
------------ | -------------
`data` | { [key: string]: any; }
`error` | [ErrorDetail](ErrorDetail.md)
`pagination` | [PaginationInfo](PaginationInfo.md)

## Example

```typescript
import type { ModelApiResponse } from '@reccito/sdk'

// TODO: Update the object below with actual values
const example = {
  "data": null,
  "error": null,
  "pagination": null,
} satisfies ModelApiResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ModelApiResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



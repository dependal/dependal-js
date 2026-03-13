
# SendEmailResult


## Properties

Name | Type
------------ | -------------
`messageId` | string
`status` | [MessageStatusEnum](MessageStatusEnum.md)

## Example

```typescript
import type { SendEmailResult } from ''

// TODO: Update the object below with actual values
const example = {
  "messageId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "status": null,
} satisfies SendEmailResult

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendEmailResult
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



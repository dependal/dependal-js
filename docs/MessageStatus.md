
# MessageStatus


## Properties

Name | Type
------------ | -------------
`messageId` | string
`status` | [MessageStatusEnum](MessageStatusEnum.md)
`reason` | string
`createdAt` | number
`updatedAt` | number
`to` | string
`from` | string
`subject` | string
`sendingMessageId` | string

## Example

```typescript
import type { MessageStatus } from ''

// TODO: Update the object below with actual values
const example = {
  "messageId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "status": null,
  "reason": null,
  "createdAt": 1773398594,
  "updatedAt": 1773398596,
  "to": developers@dependal.com,
  "from": Dependal <noreply@dependal.com>,
  "subject": Dependal test send,
  "sendingMessageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
} satisfies MessageStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



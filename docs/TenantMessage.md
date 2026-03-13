
# TenantMessage


## Properties

Name | Type
------------ | -------------
`tenantId` | string
`requestId` | string
`status` | [MessageStatusEnum](MessageStatusEnum.md)
`reason` | string
`createdAt` | number
`updatedAt` | number
`lastEventAt` | number
`createdAtIso` | Date
`updatedAtIso` | Date
`lastEventAtIso` | Date
`to` | string
`from` | string
`subject` | string
`sourceIp` | string
`stage` | [StageEnum](StageEnum.md)
`tag` | string
`keyId` | string
`callerType` | [CallerTypeEnum](CallerTypeEnum.md)
`lastSource` | [SourceEnum](SourceEnum.md)
`lastEventType` | [MessageStatusEnum](MessageStatusEnum.md)
`sesMessageId` | string
`idempotencyKey` | string
`metadata` | { [key: string]: any; }
`meta` | [TenantMessageMeta](TenantMessageMeta.md)

## Example

```typescript
import type { TenantMessage } from ''

// TODO: Update the object below with actual values
const example = {
  "tenantId": af57c621-e979-4a8b-8415-7fdb7a07982c,
  "requestId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "status": null,
  "reason": null,
  "createdAt": 1773398594,
  "updatedAt": 1773398596,
  "lastEventAt": 1773398596,
  "createdAtIso": 2026-03-13T10:43:14.338Z,
  "updatedAtIso": 2026-03-13T10:43:16.519Z,
  "lastEventAtIso": 2026-03-13T10:43:16.269Z,
  "to": developers@dependal.com,
  "from": Dependal <noreply@dependal.com>,
  "subject": Dependal test send,
  "sourceIp": 90.201.28.251,
  "stage": null,
  "tag": null,
  "keyId": ak-ez8lrxnZCi,
  "callerType": null,
  "lastSource": null,
  "lastEventType": null,
  "sesMessageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
  "idempotencyKey": 735c4c4f94e1d23e8c9686c5d92e52bcb19f3e91e02ddc42ee4387a6270a1907,
  "metadata": null,
  "meta": null,
} satisfies TenantMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



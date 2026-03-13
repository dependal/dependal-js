
# TenantMessageEvent


## Properties

Name | Type
------------ | -------------
`eventAtIso` | Date
`recipient` | string
`providerMessageId` | string
`messageId` | string
`meta` | [TenantMessageProviderMeta](TenantMessageProviderMeta.md)
`tenantId` | string
`eventAt` | number
`provider` | [ProviderEnum](ProviderEnum.md)
`eventType` | string
`eventGroup` | [EventGroupEnum](EventGroupEnum.md)
`stage` | [StageEnum](StageEnum.md)
`detail` | { [key: string]: any; }
`callerType` | [CallerTypeEnum](CallerTypeEnum.md)
`status` | [MessageStatusEnum](MessageStatusEnum.md)
`source` | [SourceEnum](SourceEnum.md)
`createdAtIso` | Date
`reason` | string
`requestId` | string
`tag` | string

## Example

```typescript
import type { TenantMessageEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "eventAtIso": 2026-03-13T10:43:15.038Z,
  "recipient": developers@dependal.com,
  "providerMessageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
  "messageId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "meta": null,
  "tenantId": af57c621-e979-4a8b-8415-7fdb7a07982c,
  "eventAt": 1773398596,
  "provider": null,
  "eventType": provider.accepted,
  "eventGroup": null,
  "stage": null,
  "detail": {},
  "callerType": null,
  "status": null,
  "source": null,
  "createdAtIso": 2026-03-13T10:43:15.038Z,
  "reason": null,
  "requestId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "tag": null,
} satisfies TenantMessageEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



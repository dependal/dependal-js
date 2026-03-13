
# TenantMessageProviderEvent


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
`eventType` | [MessageStatusEnum](MessageStatusEnum.md)
`eventGroup` | [EventGroupEnum](EventGroupEnum.md)

## Example

```typescript
import type { TenantMessageProviderEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "eventAtIso": 2026-03-13T10:43:16.269Z,
  "recipient": developers@dependal.com,
  "providerMessageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
  "messageId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "meta": null,
  "tenantId": af57c621-e979-4a8b-8415-7fdb7a07982c,
  "eventAt": 1773398596,
  "provider": null,
  "eventType": null,
  "eventGroup": null,
} satisfies TenantMessageProviderEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageProviderEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



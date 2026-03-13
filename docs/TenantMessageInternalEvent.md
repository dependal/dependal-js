
# TenantMessageInternalEvent


## Properties

Name | Type
------------ | -------------
`stage` | [StageEnum](StageEnum.md)
`detail` | { [key: string]: any; }
`tenantId` | string
`callerType` | [CallerTypeEnum](CallerTypeEnum.md)
`status` | [MessageStatusEnum](MessageStatusEnum.md)
`source` | [SourceEnum](SourceEnum.md)
`createdAtIso` | Date
`reason` | string
`requestId` | string
`eventAtIso` | Date
`eventType` | string
`tag` | string
`eventGroup` | [EventGroupEnum](EventGroupEnum.md)

## Example

```typescript
import type { TenantMessageInternalEvent } from ''

// TODO: Update the object below with actual values
const example = {
  "stage": null,
  "detail": {},
  "tenantId": af57c621-e979-4a8b-8415-7fdb7a07982c,
  "callerType": null,
  "status": null,
  "source": null,
  "createdAtIso": 2026-03-13T10:43:15.038Z,
  "reason": null,
  "requestId": 1a011c24-788e-4273-8c81-fd7d767bf0c0,
  "eventAtIso": 2026-03-13T10:43:15.038Z,
  "eventType": provider.accepted,
  "tag": null,
  "eventGroup": null,
} satisfies TenantMessageInternalEvent

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageInternalEvent
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



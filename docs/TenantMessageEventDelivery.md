
# TenantMessageEventDelivery


## Properties

Name | Type
------------ | -------------
`smtpResponse` | string
`processingTimeMillis` | number
`reportingMTA` | string
`remoteMtaIp` | string
`recipients` | Array&lt;string&gt;
`timestamp` | Date

## Example

```typescript
import type { TenantMessageEventDelivery } from ''

// TODO: Update the object below with actual values
const example = {
  "smtpResponse": 250 2.6.0 <010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000@eu-west-2.amazonses.com> ...,
  "processingTimeMillis": 1371,
  "reportingMTA": d218-9.smtp-out.eu-west-2.amazonses.com,
  "remoteMtaIp": 52.101.89.1,
  "recipients": [developers@dependal.com],
  "timestamp": 2026-03-13T10:43:16.269Z,
} satisfies TenantMessageEventDelivery

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageEventDelivery
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



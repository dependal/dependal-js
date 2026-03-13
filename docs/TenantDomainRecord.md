
# TenantDomainRecord


## Properties

Name | Type
------------ | -------------
`type` | [DnsRecordTypeEnum](DnsRecordTypeEnum.md)
`name` | string
`value` | string

## Example

```typescript
import type { TenantDomainRecord } from ''

// TODO: Update the object below with actual values
const example = {
  "type": null,
  "name": cieoxyt4oxhvpr5zmdeqxoxzqgs6umsu._domainkey.yourdomain.com,
  "value": cieoxyt4oxhvpr5zmdeqxoxzqgs6umsu.dkim.amazonses.com,
} satisfies TenantDomainRecord

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantDomainRecord
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# TenantDomainDetail


## Properties

Name | Type
------------ | -------------
`domain` | string
`mailFromDomain` | string
`status` | [DomainStatusEnum](DomainStatusEnum.md)
`ses` | [TenantDomainSesStatus](TenantDomainSesStatus.md)
`records` | [Array&lt;TenantDomainRecord&gt;](TenantDomainRecord.md)

## Example

```typescript
import type { TenantDomainDetail } from ''

// TODO: Update the object below with actual values
const example = {
  "domain": yourdomain.com,
  "mailFromDomain": mail.yourdomain.com,
  "status": null,
  "ses": null,
  "records": null,
} satisfies TenantDomainDetail

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantDomainDetail
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



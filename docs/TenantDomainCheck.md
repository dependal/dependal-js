
# TenantDomainCheck


## Properties

Name | Type
------------ | -------------
`domain` | string
`status` | [DomainStatusEnum](DomainStatusEnum.md)
`ses` | [TenantDomainSesStatus](TenantDomainSesStatus.md)

## Example

```typescript
import type { TenantDomainCheck } from ''

// TODO: Update the object below with actual values
const example = {
  "domain": yourdomain.com,
  "status": null,
  "ses": null,
} satisfies TenantDomainCheck

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantDomainCheck
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



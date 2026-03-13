
# TenantDomainSesStatus


## Properties

Name | Type
------------ | -------------
`verificationStatus` | [SesVerificationStatusEnum](SesVerificationStatusEnum.md)
`dkimStatus` | [SesVerificationStatusEnum](SesVerificationStatusEnum.md)

## Example

```typescript
import type { TenantDomainSesStatus } from ''

// TODO: Update the object below with actual values
const example = {
  "verificationStatus": null,
  "dkimStatus": null,
} satisfies TenantDomainSesStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantDomainSesStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



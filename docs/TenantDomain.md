
# TenantDomain


## Properties

Name | Type
------------ | -------------
`domain` | string
`status` | [DomainStatusEnum](DomainStatusEnum.md)
`createdAt` | number
`verifiedAt` | number
`updatedAt` | Date

## Example

```typescript
import type { TenantDomain } from ''

// TODO: Update the object below with actual values
const example = {
  "domain": example.com,
  "status": null,
  "createdAt": 1773329146,
  "verifiedAt": null,
  "updatedAt": 2026-03-12T15:25:46.312Z,
} satisfies TenantDomain

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantDomain
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



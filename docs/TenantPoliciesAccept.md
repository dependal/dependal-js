
# TenantPoliciesAccept


## Properties

Name | Type
------------ | -------------
`ok` | boolean
`acceptedVersion` | string
`requiredPolicyVersion` | string

## Example

```typescript
import type { TenantPoliciesAccept } from ''

// TODO: Update the object below with actual values
const example = {
  "ok": true,
  "acceptedVersion": 2026-02-22,
  "requiredPolicyVersion": 2026-02-22,
} satisfies TenantPoliciesAccept

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantPoliciesAccept
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



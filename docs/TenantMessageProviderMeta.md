
# TenantMessageProviderMeta


## Properties

Name | Type
------------ | -------------
`mail` | [TenantMessageEventMail](TenantMessageEventMail.md)
`send` | { [key: string]: any; }
`delivery` | [TenantMessageEventDelivery](TenantMessageEventDelivery.md)
`providerEventType` | [ProviderEventTypeEnum](ProviderEventTypeEnum.md)

## Example

```typescript
import type { TenantMessageProviderMeta } from ''

// TODO: Update the object below with actual values
const example = {
  "mail": null,
  "send": null,
  "delivery": null,
  "providerEventType": null,
} satisfies TenantMessageProviderMeta

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageProviderMeta
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)




# TenantMessageEventCommonHeaders


## Properties

Name | Type
------------ | -------------
`messageId` | string
`from` | Array&lt;string&gt;
`to` | Array&lt;string&gt;
`subject` | string

## Example

```typescript
import type { TenantMessageEventCommonHeaders } from ''

// TODO: Update the object below with actual values
const example = {
  "messageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
  "from": [Dependal <noreply@dependal.com>],
  "to": [developers@dependal.com],
  "subject": Dependal test send,
} satisfies TenantMessageEventCommonHeaders

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageEventCommonHeaders
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



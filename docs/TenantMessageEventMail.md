
# TenantMessageEventMail


## Properties

Name | Type
------------ | -------------
`sourceArn` | string
`headers` | [Array&lt;TenantMessageEventHeader&gt;](TenantMessageEventHeader.md)
`sendingAccountId` | string
`destination` | Array&lt;string&gt;
`headersTruncated` | boolean
`messageId` | string
`source` | string
`timestamp` | Date
`commonHeaders` | [TenantMessageEventCommonHeaders](TenantMessageEventCommonHeaders.md)
`tags` | { [key: string]: Array&lt;string&gt;; }

## Example

```typescript
import type { TenantMessageEventMail } from ''

// TODO: Update the object below with actual values
const example = {
  "sourceArn": arn:aws:ses:eu-west-2:154673467564:identity/dependal.com,
  "headers": null,
  "sendingAccountId": 154673467564,
  "destination": [developers@dependal.com],
  "headersTruncated": false,
  "messageId": 010b019ce6cb1552-32720d7c-a2cd-4716-a559-f587669ecacb-000000,
  "source": "Dependal" <noreply@dependal.com>,
  "timestamp": 2026-03-13T10:43:14.898Z,
  "commonHeaders": null,
  "tags": null,
} satisfies TenantMessageEventMail

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TenantMessageEventMail
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



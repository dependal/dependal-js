
# SendEmailRequest


## Properties

Name | Type
------------ | -------------
`from` | string
`to` | string
`subject` | string
`text` | string
`html` | string
`tags` | { [key: string]: string; }

## Example

```typescript
import type { SendEmailRequest } from ''

// TODO: Update the object below with actual values
const example = {
  "from": Dependal <noreply@dependal.com>,
  "to": user@example.com,
  "subject": Welcome to Dependal,
  "text": Thanks for signing up.,
  "html": <p>Thanks for signing up.</p>,
  "tags": null,
} satisfies SendEmailRequest

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as SendEmailRequest
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)



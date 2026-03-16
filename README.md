# Dependal JavaScript SDK

Official JavaScript SDK for the Dependal transactional email API.

Dependal is a reputation-first transactional email platform built for reliable delivery, clear logs, and predictable pricing.

## Installation

```bash
npm install @dependal/sdk
```

## Requirements

- Node.js 18+ recommended
- A Dependal API key

## Quick Start

```javascript
import { Configuration, ApiClient, MessagesApi } from "@dependal/sdk";

const config = new Configuration({
  basePath: "https://api.dependal.com",
  apiKey: "dp_your_api_key_here"
});

const client = new ApiClient(config);
const messages = new MessagesApi(client);

async function main() {
  const response = await messages.sendEmail({
    to: "user@example.com",
    from: "Dependal <noreply@yourdomain.com>",
    subject: "Hello from Dependal",
    html: "<p>Hello 👋</p><p>This is a transactional email sent using Dependal.</p>"
  });

  console.log(response);
}

main().catch(console.error);
```

## Authentication

Dependal uses API key authentication.

Pass your API key when creating the SDK configuration.

```javascript
const config = new Configuration({
  basePath: "https://api.dependal.com",
  apiKey: "dp_your_api_key_here"
});
```

Keep your API key secure and never expose it in client-side code.

## Usage

### Send an email

```javascript
import { Configuration, ApiClient, MessagesApi } from "@dependal/sdk";

const config = new Configuration({
  basePath: "https://api.dependal.com",
  apiKey: "dp_your_api_key_here"
});

const client = new ApiClient(config);
const messages = new MessagesApi(client);

const result = await messages.sendEmail({
  to: "user@example.com",
  from: "Dependal <noreply@yourdomain.com>",
  subject: "Password reset",
  html: "<p>Click the link below to reset your password.</p>"
});

console.log(result);
```

### Send a plain text email

```javascript
const result = await messages.sendEmail({
  to: "user@example.com",
  from: "Dependal <noreply@yourdomain.com>",
  subject: "Plain text example",
  text: "Hello from Dependal"
});
```

### Send to multiple recipients

```javascript
const result = await messages.sendEmail({
  to: [
    "user1@example.com",
    "user2@example.com"
  ],
  from: "Dependal <noreply@yourdomain.com>",
  subject: "Multi-recipient email",
  html: "<p>Hello everyone</p>"
});
```

## Example Response

```json
{
  "messageId": "dep_123456789",
  "status": "queued"
}
```

## Error Handling

Use standard try/catch handling around SDK calls.

```javascript
try {
  const result = await messages.sendEmail({
    to: "user@example.com",
    from: "Dependal <noreply@yourdomain.com>",
    subject: "Test email",
    html: "<p>Hello</p>"
  });

  console.log(result);
} catch (error) {
  console.error("Dependal API error:", error);
}
```

## Base URL

Production API base URL:

```
https://api.dependal.com
```

## Notes

- Dependal is designed for **transactional email**
- You must send from a domain configured in your Dependal account
- API access requires a valid API key
- Sending availability may depend on account status, domain verification, and plan limits

------------------------------------------------------------------------

## Documentation

Full API documentation:

https://dependal.com/docs

------------------------------------------------------------------------

## Support

For support, documentation, or account access, visit the Dependal dashboard or website.

## License

MIT

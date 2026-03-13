# MessagesApi

All URIs are relative to *https://api.dependal.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getMessageStatus**](MessagesApi.md#getmessagestatus) | **GET** /v1/status/{messageId} | Get message delivery status |
| [**getTenantMessage**](MessagesApi.md#gettenantmessage) | **GET** /v1/tenant/messages/{messageId} | Get tenant message |
| [**listTenantMessageEvents**](MessagesApi.md#listtenantmessageevents) | **GET** /v1/tenant/messages/{messageId}/events | List tenant message events |
| [**listTenantMessages**](MessagesApi.md#listtenantmessages) | **GET** /v1/tenant/messages | List tenant messages |
| [**sendEmail**](MessagesApi.md#sendemailoperation) | **POST** /v1/send | Send an email |



## getMessageStatus

> MessageStatusResponse getMessageStatus(messageId)

Get message delivery status

Returns the current delivery status for a message.

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '';
import type { GetMessageStatusRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MessagesApi(config);

  const body = {
    // string
    messageId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetMessageStatusRequest;

  try {
    const data = await api.getMessageStatus(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**MessageStatusResponse**](MessageStatusResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message status |  -  |
| **401** | Missing or invalid credentials |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTenantMessage

> TenantMessageResponse getTenantMessage(messageId)

Get tenant message

Returns a single message record for the authenticated tenant.

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '';
import type { GetTenantMessageRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MessagesApi(config);

  const body = {
    // string | Message request ID
    messageId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetTenantMessageRequest;

  try {
    const data = await api.getTenantMessage(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | `string` | Message request ID | [Defaults to `undefined`] |

### Return type

[**TenantMessageResponse**](TenantMessageResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant message |  -  |
| **401** | Missing or invalid credentials |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTenantMessageEvents

> TenantMessageEventsResponse listTenantMessageEvents(messageId, cursor, limit)

List tenant message events

Returns the event timeline for a single tenant message, including internal processing events and provider delivery events.

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '';
import type { ListTenantMessageEventsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MessagesApi(config);

  const body = {
    // string | Message request ID
    messageId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // string | Opaque pagination cursor returned by a previous response (optional)
    cursor: cursor_example,
    // number | Maximum number of events to return (optional)
    limit: 56,
  } satisfies ListTenantMessageEventsRequest;

  try {
    const data = await api.listTenantMessageEvents(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **messageId** | `string` | Message request ID | [Defaults to `undefined`] |
| **cursor** | `string` | Opaque pagination cursor returned by a previous response | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of events to return | [Optional] [Defaults to `50`] |

### Return type

[**TenantMessageEventsResponse**](TenantMessageEventsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Message events |  -  |
| **401** | Missing or invalid credentials |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTenantMessages

> TenantMessagesResponse listTenantMessages(cursor, limit)

List tenant messages

Returns paginated message logs for the authenticated tenant.

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '';
import type { ListTenantMessagesRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MessagesApi(config);

  const body = {
    // string | Opaque pagination cursor returned by a previous response (optional)
    cursor: cursor_example,
    // number | Maximum number of messages to return (optional)
    limit: 56,
  } satisfies ListTenantMessagesRequest;

  try {
    const data = await api.listTenantMessages(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **cursor** | `string` | Opaque pagination cursor returned by a previous response | [Optional] [Defaults to `undefined`] |
| **limit** | `number` | Maximum number of messages to return | [Optional] [Defaults to `50`] |

### Return type

[**TenantMessagesResponse**](TenantMessagesResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant messages |  -  |
| **401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## sendEmail

> SendEmailResponse sendEmail(sendEmailRequest)

Send an email

Queue a transactional email for delivery.

### Example

```ts
import {
  Configuration,
  MessagesApi,
} from '';
import type { SendEmailOperationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MessagesApi(config);

  const body = {
    // SendEmailRequest
    sendEmailRequest: {"from":"Dependal <noreply@dependal.com>","to":"developers@dependal.com","subject":"Dependal test send","html":"<p>Hello 👋</p><p>This is a transactional test email from Dependal.</p>"},
  } satisfies SendEmailOperationRequest;

  try {
    const data = await api.sendEmail(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **sendEmailRequest** | [SendEmailRequest](SendEmailRequest.md) |  | |

### Return type

[**SendEmailResponse**](SendEmailResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **202** | Accepted for delivery |  -  |
| **400** | Request validation failed |  -  |
| **401** | Missing or invalid credentials |  -  |
| **403** | Sending blocked |  -  |
| **409** | Conflict |  -  |
| **413** | Payload too large |  -  |
| **503** | Service unavailable |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


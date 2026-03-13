# DomainsApi

All URIs are relative to *https://api.dependal.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**checkTenantDomain**](DomainsApi.md#checktenantdomain) | **POST** /v1/tenant/domains/{domain}/check | Check tenant domain verification |
| [**createTenantDomain**](DomainsApi.md#createtenantdomain) | **POST** /v1/tenant/domains | Add tenant domain |
| [**getTenantDomain**](DomainsApi.md#gettenantdomain) | **GET** /v1/tenant/domains/{domain} | Get tenant domain details |
| [**listTenantDomains**](DomainsApi.md#listtenantdomains) | **GET** /v1/tenant/domains | List tenant domains |



## checkTenantDomain

> TenantDomainCheckResponse checkTenantDomain(domain)

Check tenant domain verification

Re-checks the verification status of a tenant domain and returns the latest provider verification state.

### Example

```ts
import {
  Configuration,
  DomainsApi,
} from '';
import type { CheckTenantDomainRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DomainsApi(config);

  const body = {
    // string | Domain name to check
    domain: domain_example,
  } satisfies CheckTenantDomainRequest;

  try {
    const data = await api.checkTenantDomain(body);
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
| **domain** | `string` | Domain name to check | [Defaults to `undefined`] |

### Return type

[**TenantDomainCheckResponse**](TenantDomainCheckResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Domain verification status |  -  |
| **401** | Missing or invalid credentials |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## createTenantDomain

> TenantDomainCreateResponse createTenantDomain(tenantDomainCreateRequest)

Add tenant domain

Registers a domain for the authenticated tenant and begins the verification process.

### Example

```ts
import {
  Configuration,
  DomainsApi,
} from '';
import type { CreateTenantDomainRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DomainsApi(config);

  const body = {
    // TenantDomainCreateRequest
    tenantDomainCreateRequest: {"domain":"yourdomain.com"},
  } satisfies CreateTenantDomainRequest;

  try {
    const data = await api.createTenantDomain(body);
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
| **tenantDomainCreateRequest** | [TenantDomainCreateRequest](TenantDomainCreateRequest.md) |  | |

### Return type

[**TenantDomainCreateResponse**](TenantDomainCreateResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Domain created |  -  |
| **400** | Request validation failed |  -  |
| **401** | Missing or invalid credentials |  -  |
| **409** | Conflict |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTenantDomain

> TenantDomainDetailResponse getTenantDomain(domain)

Get tenant domain details

Returns details for a tenant domain, including SES verification status and required DNS records.

### Example

```ts
import {
  Configuration,
  DomainsApi,
} from '';
import type { GetTenantDomainRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DomainsApi(config);

  const body = {
    // string | Domain name to retrieve
    domain: domain_example,
  } satisfies GetTenantDomainRequest;

  try {
    const data = await api.getTenantDomain(body);
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
| **domain** | `string` | Domain name to retrieve | [Defaults to `undefined`] |

### Return type

[**TenantDomainDetailResponse**](TenantDomainDetailResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant domain details |  -  |
| **401** | Missing or invalid credentials |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTenantDomains

> TenantDomainsResponse listTenantDomains()

List tenant domains

Returns the domains registered for the authenticated tenant.

### Example

```ts
import {
  Configuration,
  DomainsApi,
} from '';
import type { ListTenantDomainsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new DomainsApi(config);

  try {
    const data = await api.listTenantDomains();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**TenantDomainsResponse**](TenantDomainsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Tenant domains |  -  |
| **401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


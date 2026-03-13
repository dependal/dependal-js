# TenantApi

All URIs are relative to *https://api.dependal.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**acceptTenantPolicies**](TenantApi.md#accepttenantpolicies) | **POST** /v1/tenant/policies/accept | Accept tenant policies |



## acceptTenantPolicies

> TenantPoliciesAcceptResponse acceptTenantPolicies()

Accept tenant policies

Records acceptance of the current required policy version for the authenticated tenant.

### Example

```ts
import {
  Configuration,
  TenantApi,
} from '';
import type { AcceptTenantPoliciesRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: ApiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new TenantApi(config);

  try {
    const data = await api.acceptTenantPolicies();
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

[**TenantPoliciesAcceptResponse**](TenantPoliciesAcceptResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Policies accepted successfully |  -  |
| **401** | Missing or invalid credentials |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


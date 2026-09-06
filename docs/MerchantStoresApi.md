# MerchantStoresApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createStore**](MerchantStoresApi.md#createstore) | **POST** /api/v1/merchant/stores | Create Store |
| [**getStore**](MerchantStoresApi.md#getstore) | **GET** /api/v1/merchant/stores/{store_id} | Get Store |
| [**getStoreStats**](MerchantStoresApi.md#getstorestats) | **GET** /api/v1/merchant/stores/{store_id}/stats | Get Store Stats |
| [**listStores**](MerchantStoresApi.md#liststores) | **GET** /api/v1/merchant/stores | List Stores |
| [**updateStore**](MerchantStoresApi.md#updatestore) | **PUT** /api/v1/merchant/stores/{store_id} | Update Store |



## createStore

> StoreResponse createStore(storeCreate)

Create Store

Create a new store for the organisation.  **Authentication:** Required (Organisation bearer token)

### Example

```ts
import {
  Configuration,
  MerchantStoresApi,
} from '@reccito/sdk';
import type { CreateStoreRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantStoresApi(config);

  const body = {
    // StoreCreate
    storeCreate: ...,
  } satisfies CreateStoreRequest;

  try {
    const data = await api.createStore(body);
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
| **storeCreate** | [StoreCreate](StoreCreate.md) |  | |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getStore

> StoreResponse getStore(storeId)

Get Store

Get a specific store by ID.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - &#x60;store_id&#x60;: UUID of the store

### Example

```ts
import {
  Configuration,
  MerchantStoresApi,
} from '@reccito/sdk';
import type { GetStoreRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantStoresApi(config);

  const body = {
    // string
    storeId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetStoreRequest;

  try {
    const data = await api.getStore(body);
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
| **storeId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getStoreStats

> StoreStatsResponse getStoreStats(storeId)

Get Store Stats

Get statistics for a store.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - &#x60;store_id&#x60;: UUID of the store

### Example

```ts
import {
  Configuration,
  MerchantStoresApi,
} from '@reccito/sdk';
import type { GetStoreStatsRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantStoresApi(config);

  const body = {
    // string
    storeId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies GetStoreStatsRequest;

  try {
    const data = await api.getStoreStats(body);
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
| **storeId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**StoreStatsResponse**](StoreStatsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listStores

> StoreListResponse listStores(skip, limit, isActive, q)

List Stores

List all stores for the organisation.  **Authentication:** Required (Organisation bearer token)  **Query Parameters:** - &#x60;skip&#x60;: Number of stores to skip (default: 0) - &#x60;limit&#x60;: Number of stores to return (default: 100, max: 1000) - &#x60;is_active&#x60;: Filter by active status (optional) - &#x60;q&#x60;: Search by store name/code/city/email/phone (optional)

### Example

```ts
import {
  Configuration,
  MerchantStoresApi,
} from '@reccito/sdk';
import type { ListStoresRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantStoresApi(config);

  const body = {
    // number (optional)
    skip: 56,
    // number (optional)
    limit: 56,
    // boolean (optional)
    isActive: true,
    // string (optional)
    q: q_example,
  } satisfies ListStoresRequest;

  try {
    const data = await api.listStores(body);
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
| **skip** | `number` |  | [Optional] [Defaults to `0`] |
| **limit** | `number` |  | [Optional] [Defaults to `100`] |
| **isActive** | `boolean` |  | [Optional] [Defaults to `undefined`] |
| **q** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**StoreListResponse**](StoreListResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateStore

> StoreResponse updateStore(storeId, storeUpdate)

Update Store

Update a store.  **Authentication:** Required (Organisation bearer token)  **Path Parameters:** - &#x60;store_id&#x60;: UUID of the store  **Request Body:** Updated store fields (all optional)

### Example

```ts
import {
  Configuration,
  MerchantStoresApi,
} from '@reccito/sdk';
import type { UpdateStoreRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantStoresApi(config);

  const body = {
    // string
    storeId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // StoreUpdate
    storeUpdate: ...,
  } satisfies UpdateStoreRequest;

  try {
    const data = await api.updateStore(body);
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
| **storeId** | `string` |  | [Defaults to `undefined`] |
| **storeUpdate** | [StoreUpdate](StoreUpdate.md) |  | |

### Return type

[**StoreResponse**](StoreResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


# MerchantReceiptsApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createReceipt**](MerchantReceiptsApi.md#createreceipt) | **POST** /api/v1/merchant/receipts | Create Receipt |
| [**getReceipt**](MerchantReceiptsApi.md#getreceipt) | **GET** /api/v1/merchant/receipts/{receipt_id} | Get Receipt |
| [**listReceipts**](MerchantReceiptsApi.md#listreceipts) | **GET** /api/v1/merchant/receipts | List Receipts |
| [**refreshReceiptQr**](MerchantReceiptsApi.md#refreshreceiptqr) | **PUT** /api/v1/merchant/receipts/{receipt_id}/refresh-qr | Refresh Qr Code |



## createReceipt

> ReceiptImmediateResponse createReceipt(receiptCreate)

Create Receipt

Create a new receipt. Synchronous: the receipt is durably persisted before this returns (see ReceiptService.create_receipt_synchronously). A retry with the same dedupe_key returns the original receipt with 200, not an error (idempotent replay, Stripe-style).

### Example

```ts
import {
  Configuration,
  MerchantReceiptsApi,
} from '@reccito/sdk';
import type { CreateReceiptRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantReceiptsApi(config);

  const body = {
    // ReceiptCreate
    receiptCreate: ...,
  } satisfies CreateReceiptRequest;

  try {
    const data = await api.createReceipt(body);
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
| **receiptCreate** | [ReceiptCreate](ReceiptCreate.md) |  | |

### Return type

[**ReceiptImmediateResponse**](ReceiptImmediateResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Successful Response |  -  |
| **200** | Idempotent replay: a receipt with this organisation + dedupe_key already existed. Returns the original receipt unchanged, not an error. |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getReceipt

> MerchantReceiptResponse getReceipt(receiptId)

Get Receipt

Get receipt by ID.

### Example

```ts
import {
  Configuration,
  MerchantReceiptsApi,
} from '@reccito/sdk';
import type { GetReceiptRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantReceiptsApi(config);

  const body = {
    // string
    receiptId: receiptId_example,
  } satisfies GetReceiptRequest;

  try {
    const data = await api.getReceipt(body);
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
| **receiptId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**MerchantReceiptResponse**](MerchantReceiptResponse.md)

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


## listReceipts

> ReceiptListResponse listReceipts(page, limit, storeId, status, search, sortBy, sortOrder)

List Receipts

List receipts with filters and pagination.

### Example

```ts
import {
  Configuration,
  MerchantReceiptsApi,
} from '@reccito/sdk';
import type { ListReceiptsRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantReceiptsApi(config);

  const body = {
    // number (optional)
    page: 56,
    // number (optional)
    limit: 56,
    // string (optional)
    storeId: storeId_example,
    // string (optional)
    status: status_example,
    // string (optional)
    search: search_example,
    // string (optional)
    sortBy: sortBy_example,
    // string (optional)
    sortOrder: sortOrder_example,
  } satisfies ListReceiptsRequest;

  try {
    const data = await api.listReceipts(body);
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
| **page** | `number` |  | [Optional] [Defaults to `1`] |
| **limit** | `number` |  | [Optional] [Defaults to `50`] |
| **storeId** | `string` |  | [Optional] [Defaults to `undefined`] |
| **status** | `string` |  | [Optional] [Defaults to `undefined`] |
| **search** | `string` |  | [Optional] [Defaults to `undefined`] |
| **sortBy** | `string` |  | [Optional] [Defaults to `&#39;created_at&#39;`] |
| **sortOrder** | `string` |  | [Optional] [Defaults to `&#39;desc&#39;`] |

### Return type

[**ReceiptListResponse**](ReceiptListResponse.md)

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


## refreshReceiptQr

> QRRefreshResponse refreshReceiptQr(receiptId)

Refresh Qr Code

Refresh QR code for a receipt.

### Example

```ts
import {
  Configuration,
  MerchantReceiptsApi,
} from '@reccito/sdk';
import type { RefreshReceiptQrRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantReceiptsApi(config);

  const body = {
    // string
    receiptId: receiptId_example,
  } satisfies RefreshReceiptQrRequest;

  try {
    const data = await api.refreshReceiptQr(body);
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
| **receiptId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**QRRefreshResponse**](QRRefreshResponse.md)

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


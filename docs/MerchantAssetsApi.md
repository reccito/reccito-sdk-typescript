# MerchantAssetsApi

All URIs are relative to *https://api.reccito.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**listOrganisationAssets**](MerchantAssetsApi.md#listorganisationassets) | **GET** /api/v1/merchant/assets/list | List organisation assets |
| [**uploadOrganisationBanner**](MerchantAssetsApi.md#uploadorganisationbanner) | **POST** /api/v1/merchant/assets/upload/banner | Upload organisation banner |
| [**uploadOrganisationLogo**](MerchantAssetsApi.md#uploadorganisationlogo) | **POST** /api/v1/merchant/assets/upload/logo | Upload organisation logo |
| [**uploadStoreLogo**](MerchantAssetsApi.md#uploadstorelogo) | **POST** /api/v1/merchant/assets/upload/store/logo | Upload store logo |



## listOrganisationAssets

> ModelApiResponse listOrganisationAssets(assetType)

List organisation assets

List all branding assets uploaded for the organisation.

### Example

```ts
import {
  Configuration,
  MerchantAssetsApi,
} from '@reccito/sdk';
import type { ListOrganisationAssetsRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantAssetsApi(config);

  const body = {
    // string (optional)
    assetType: assetType_example,
  } satisfies ListOrganisationAssetsRequest;

  try {
    const data = await api.listOrganisationAssets(body);
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
| **assetType** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**ModelApiResponse**](ModelApiResponse.md)

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


## uploadOrganisationBanner

> ModelApiResponse uploadOrganisationBanner(file)

Upload organisation banner

Upload a banner file for the organisation. Supported formats: JPEG, PNG, WebP. Max 5MB.

### Example

```ts
import {
  Configuration,
  MerchantAssetsApi,
} from '@reccito/sdk';
import type { UploadOrganisationBannerRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantAssetsApi(config);

  const body = {
    // Blob | Banner file to upload
    file: BINARY_DATA_HERE,
  } satisfies UploadOrganisationBannerRequest;

  try {
    const data = await api.uploadOrganisationBanner(body);
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
| **file** | `Blob` | Banner file to upload | [Defaults to `undefined`] |

### Return type

[**ModelApiResponse**](ModelApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## uploadOrganisationLogo

> ModelApiResponse uploadOrganisationLogo(file)

Upload organisation logo

Upload a logo file for the organisation. Supported formats: JPEG, PNG, WebP, SVG. Max 5MB.

### Example

```ts
import {
  Configuration,
  MerchantAssetsApi,
} from '@reccito/sdk';
import type { UploadOrganisationLogoRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantAssetsApi(config);

  const body = {
    // Blob | Logo file to upload
    file: BINARY_DATA_HERE,
  } satisfies UploadOrganisationLogoRequest;

  try {
    const data = await api.uploadOrganisationLogo(body);
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
| **file** | `Blob` | Logo file to upload | [Defaults to `undefined`] |

### Return type

[**ModelApiResponse**](ModelApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## uploadStoreLogo

> ModelApiResponse uploadStoreLogo(storeId, file)

Upload store logo

Upload a logo file for a specific store. Supported formats: JPEG, PNG, WebP, SVG. Max 5MB.

### Example

```ts
import {
  Configuration,
  MerchantAssetsApi,
} from '@reccito/sdk';
import type { UploadStoreLogoRequest } from '@reccito/sdk';

async function example() {
  console.log("🚀 Testing @reccito/sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: ApiKeyAuth
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MerchantAssetsApi(config);

  const body = {
    // string
    storeId: storeId_example,
    // Blob | Store logo file to upload
    file: BINARY_DATA_HERE,
  } satisfies UploadStoreLogoRequest;

  try {
    const data = await api.uploadStoreLogo(body);
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
| **file** | `Blob` | Store logo file to upload | [Defaults to `undefined`] |

### Return type

[**ModelApiResponse**](ModelApiResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


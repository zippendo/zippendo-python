# zippendo.BrandsApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**archive_org_brand**](BrandsApi.md#archive_org_brand) | **POST** /orgs/{orgId}/brands/{brandId}/archive | Archive brand
[**check_brand_slug**](BrandsApi.md#check_brand_slug) | **GET** /orgs/{orgId}/brands/check-slug/{slug} | Check brand slug availability
[**create_org_brand**](BrandsApi.md#create_org_brand) | **POST** /orgs/{orgId}/brands | Create brand
[**delete_brand_logo**](BrandsApi.md#delete_brand_logo) | **DELETE** /orgs/{orgId}/brands/{brandId}/logo | Delete brand logo
[**get_brand_logo**](BrandsApi.md#get_brand_logo) | **GET** /orgs/{orgId}/brands/{brandId}/logo | Get brand logo
[**get_org_brand**](BrandsApi.md#get_org_brand) | **GET** /orgs/{orgId}/brands/{brandId} | Get brand
[**list_org_brands**](BrandsApi.md#list_org_brands) | **GET** /orgs/{orgId}/brands | List brands
[**unarchive_org_brand**](BrandsApi.md#unarchive_org_brand) | **POST** /orgs/{orgId}/brands/{brandId}/unarchive | Unarchive brand
[**update_org_brand**](BrandsApi.md#update_org_brand) | **PATCH** /orgs/{orgId}/brands/{brandId} | Update brand
[**upload_brand_logo**](BrandsApi.md#upload_brand_logo) | **POST** /orgs/{orgId}/brands/{brandId}/logo | Upload brand logo


# **archive_org_brand**
> ListOrgBrands200ResponseDataInner archive_org_brand(org_id, brand_id)

Archive brand

Archives a brand: it leaves the brand switcher and default listings, but its orders, shipments and settings are retained and remain visible in the organization-wide view.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID

    try:
        # Archive brand
        api_response = api_instance.archive_org_brand(org_id, brand_id)
        print("The response of BrandsApi->archive_org_brand:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->archive_org_brand: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **check_brand_slug**
> CheckBrandSlug200Response check_brand_slug(org_id, slug)

Check brand slug availability

Reports whether a brand slug is free within this organization. Brand slugs are unique per organization, so the same slug may exist in another organization. Archived brands still hold their slug.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.check_brand_slug200_response import CheckBrandSlug200Response
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    slug = 'acme' # str | Brand slug to check

    try:
        # Check brand slug availability
        api_response = api_instance.check_brand_slug(org_id, slug)
        print("The response of BrandsApi->check_brand_slug:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->check_brand_slug: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **slug** | **str**| Brand slug to check | 

### Return type

[**CheckBrandSlug200Response**](CheckBrandSlug200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_org_brand**
> ListOrgBrands200ResponseDataInner create_org_brand(org_id, create_org_brand_request)

Create brand

Creates a brand (sub-account) in the organization. The slug is derived from the name when omitted. Requires a plan that includes brands.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_org_brand_request import CreateOrgBrandRequest
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    create_org_brand_request = zippendo.CreateOrgBrandRequest() # CreateOrgBrandRequest | 

    try:
        # Create brand
        api_response = api_instance.create_org_brand(org_id, create_org_brand_request)
        print("The response of BrandsApi->create_org_brand:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->create_org_brand: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_org_brand_request** | [**CreateOrgBrandRequest**](CreateOrgBrandRequest.md)|  | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_brand_logo**
> ListOrgBrands200ResponseDataInner delete_brand_logo(org_id, brand_id)

Delete brand logo

Removes a brand's logo. Its documents fall back to the organization's logo. Requires the brands and customBranding entitlements.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID

    try:
        # Delete brand logo
        api_response = api_instance.delete_brand_logo(org_id, brand_id)
        print("The response of BrandsApi->delete_brand_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->delete_brand_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_brand_logo**
> bytes get_brand_logo(org_id, brand_id)

Get brand logo

Streams the brand's logo bytes. This is the URL returned as the brand's `logoUrl`.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID

    try:
        # Get brand logo
        api_response = api_instance.get_brand_logo(org_id, brand_id)
        print("The response of BrandsApi->get_brand_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->get_brand_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 

### Return type

**bytes**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: image/png, image/jpeg, image/webp

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The logo image bytes |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_org_brand**
> ListOrgBrands200ResponseDataInner get_org_brand(org_id, brand_id)

Get brand

Returns a single brand (sub-account) by id.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID

    try:
        # Get brand
        api_response = api_instance.get_org_brand(org_id, brand_id)
        print("The response of BrandsApi->get_org_brand:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->get_org_brand: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_org_brands**
> ListOrgBrands200Response list_org_brands(org_id, include_archived=include_archived)

List brands

Returns the organization's brands (sub-accounts). Archived brands are excluded unless `includeArchived` is set.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response import ListOrgBrands200Response
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    include_archived = 'false' # str | Include archived brands in the response (optional)

    try:
        # List brands
        api_response = api_instance.list_org_brands(org_id, include_archived=include_archived)
        print("The response of BrandsApi->list_org_brands:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->list_org_brands: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **include_archived** | **str**| Include archived brands in the response | [optional] 

### Return type

[**ListOrgBrands200Response**](ListOrgBrands200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **unarchive_org_brand**
> ListOrgBrands200ResponseDataInner unarchive_org_brand(org_id, brand_id)

Unarchive brand

Restores an archived brand so it appears in the brand switcher again.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID

    try:
        # Unarchive brand
        api_response = api_instance.unarchive_org_brand(org_id, brand_id)
        print("The response of BrandsApi->unarchive_org_brand:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->unarchive_org_brand: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_org_brand**
> ListOrgBrands200ResponseDataInner update_org_brand(org_id, brand_id, update_org_brand_request)

Update brand

Updates a brand's name, slug, identity overrides (company name, VAT, customs, address) and document colours. Null clears an override so the organization's value applies again.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.models.update_org_brand_request import UpdateOrgBrandRequest
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID
    update_org_brand_request = zippendo.UpdateOrgBrandRequest() # UpdateOrgBrandRequest | 

    try:
        # Update brand
        api_response = api_instance.update_org_brand(org_id, brand_id, update_org_brand_request)
        print("The response of BrandsApi->update_org_brand:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->update_org_brand: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 
 **update_org_brand_request** | [**UpdateOrgBrandRequest**](UpdateOrgBrandRequest.md)|  | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**401** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |
**409** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_brand_logo**
> ListOrgBrands200ResponseDataInner upload_brand_logo(org_id, brand_id, file)

Upload brand logo

Uploads a brand's logo as multipart/form-data. Accepts PNG, JPG or WEBP up to 5MB and 4096×4096px; the image is re-encoded and stored. Documents for this brand's shipments use it instead of the organization's logo. Requires the brands and customBranding entitlements.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner
from zippendo.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.zippendo.com
# See configuration.py for a list of all supported configuration parameters.
configuration = zippendo.Configuration(
    host = "https://api.zippendo.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearerAuth
configuration = zippendo.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with zippendo.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = zippendo.BrandsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    brand_id = 'brnd_8f3kd92ld0' # str | Brand ID
    file = None # bytes | Image file (PNG, JPG, or WEBP)

    try:
        # Upload brand logo
        api_response = api_instance.upload_brand_logo(org_id, brand_id, file)
        print("The response of BrandsApi->upload_brand_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BrandsApi->upload_brand_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **brand_id** | **str**| Brand ID | 
 **file** | **bytes**| Image file (PNG, JPG, or WEBP) | 

### Return type

[**ListOrgBrands200ResponseDataInner**](ListOrgBrands200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |
**413** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


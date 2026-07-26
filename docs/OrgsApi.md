# zippendo.OrgsApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_org_logo**](OrgsApi.md#delete_org_logo) | **DELETE** /orgs/{orgId}/branding/logo | Delete org logo
[**get_org**](OrgsApi.md#get_org) | **GET** /orgs/{id} | Get org
[**get_org_branding**](OrgsApi.md#get_org_branding) | **GET** /orgs/{orgId}/branding | Get org branding
[**get_org_logo**](OrgsApi.md#get_org_logo) | **GET** /orgs/{orgId}/branding/logo | Download org logo
[**update_org**](OrgsApi.md#update_org) | **PUT** /orgs/{id} | Update org
[**update_org_branding**](OrgsApi.md#update_org_branding) | **PUT** /orgs/{orgId}/branding | Update org branding
[**upload_org_logo**](OrgsApi.md#upload_org_logo) | **POST** /orgs/{orgId}/branding/logo | Upload org logo


# **delete_org_logo**
> GetOrgBranding200Response delete_org_logo(org_id)

Delete org logo

Removes the org logo. Requires the customBranding entitlement.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_org_branding200_response import GetOrgBranding200Response
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
    api_instance = zippendo.OrgsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID

    try:
        # Delete org logo
        api_response = api_instance.delete_org_logo(org_id)
        print("The response of OrgsApi->delete_org_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->delete_org_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_org**
> GetOrg200Response get_org(id)

Get org

Returns a specific organization by ID, including its member count.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_org200_response import GetOrg200Response
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
    api_instance = zippendo.OrgsApi(api_client)
    id = 'clz9x8a7b0001' # str | Resource ID

    try:
        # Get org
        api_response = api_instance.get_org(id)
        print("The response of OrgsApi->get_org:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->get_org: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Resource ID | 

### Return type

[**GetOrg200Response**](GetOrg200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_org_branding**
> GetOrgBranding200Response get_org_branding(org_id)

Get org branding

Returns the org's brand colors and an authenticated URL to download the logo.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_org_branding200_response import GetOrgBranding200Response
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
    api_instance = zippendo.OrgsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID

    try:
        # Get org branding
        api_response = api_instance.get_org_branding(org_id)
        print("The response of OrgsApi->get_org_branding:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->get_org_branding: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_org_logo**
> bytes get_org_logo(org_id)

Download org logo

Returns the org logo image bytes with the stored content type.

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
    api_instance = zippendo.OrgsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID

    try:
        # Download org logo
        api_response = api_instance.get_org_logo(org_id)
        print("The response of OrgsApi->get_org_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->get_org_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 

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
**200** | The org logo image bytes |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_org**
> UpdateOrg200Response update_org(id, update_org_request)

Update org

Updates an existing organization's profile, billing, and customs settings.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.update_org200_response import UpdateOrg200Response
from zippendo.models.update_org_request import UpdateOrgRequest
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
    api_instance = zippendo.OrgsApi(api_client)
    id = 'clz9x8a7b0001' # str | Resource ID
    update_org_request = zippendo.UpdateOrgRequest() # UpdateOrgRequest | 

    try:
        # Update org
        api_response = api_instance.update_org(id, update_org_request)
        print("The response of OrgsApi->update_org:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->update_org: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Resource ID | 
 **update_org_request** | [**UpdateOrgRequest**](UpdateOrgRequest.md)|  | 

### Return type

[**UpdateOrg200Response**](UpdateOrg200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_org_branding**
> GetOrgBranding200Response update_org_branding(org_id, update_org_branding_request)

Update org branding

Sets the org brand colors. Requires the customBranding entitlement.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_org_branding200_response import GetOrgBranding200Response
from zippendo.models.update_org_branding_request import UpdateOrgBrandingRequest
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
    api_instance = zippendo.OrgsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    update_org_branding_request = zippendo.UpdateOrgBrandingRequest() # UpdateOrgBrandingRequest | 

    try:
        # Update org branding
        api_response = api_instance.update_org_branding(org_id, update_org_branding_request)
        print("The response of OrgsApi->update_org_branding:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->update_org_branding: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **update_org_branding_request** | [**UpdateOrgBrandingRequest**](UpdateOrgBrandingRequest.md)|  | 

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_org_logo**
> GetOrgBranding200Response upload_org_logo(org_id, file)

Upload org logo

Uploads the org logo as multipart/form-data. Accepts PNG, JPG, or WEBP up to 5MB and 4096×4096px; the image is re-encoded and stored. Requires the customBranding entitlement.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_org_branding200_response import GetOrgBranding200Response
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
    api_instance = zippendo.OrgsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    file = None # bytes | Image file (PNG, JPG, or WEBP)

    try:
        # Upload org logo
        api_response = api_instance.upload_org_logo(org_id, file)
        print("The response of OrgsApi->upload_org_logo:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrgsApi->upload_org_logo: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **file** | **bytes**| Image file (PNG, JPG, or WEBP) | 

### Return type

[**GetOrgBranding200Response**](GetOrgBranding200Response.md)

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


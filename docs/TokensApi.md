# zippendo.TokensApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_api_token**](TokensApi.md#create_api_token) | **POST** /orgs/{orgId}/api-tokens | Create API keys
[**get_api_token**](TokensApi.md#get_api_token) | **GET** /orgs/{orgId}/api-tokens/{tokenId} | Get API keys
[**list_api_tokens**](TokensApi.md#list_api_tokens) | **GET** /orgs/{orgId}/api-tokens | List API keys
[**revoke_api_token**](TokensApi.md#revoke_api_token) | **DELETE** /orgs/{orgId}/api-tokens/{tokenId} | Revoke API keys
[**update_api_token**](TokensApi.md#update_api_token) | **PATCH** /orgs/{orgId}/api-tokens/{tokenId} | Update API keys
[**verify_api_token**](TokensApi.md#verify_api_token) | **POST** /api-tokens/verify | Verify API keys


# **create_api_token**
> CreateApiToken201Response create_api_token(org_id, create_api_token_request)

Create API keys

Creates a new API token for the specified organization. The full token is only shown once.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_api_token201_response import CreateApiToken201Response
from zippendo.models.create_api_token_request import CreateApiTokenRequest
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
    api_instance = zippendo.TokensApi(api_client)
    org_id = 'org_4d8af01qw2' # str | Organization ID
    create_api_token_request = zippendo.CreateApiTokenRequest() # CreateApiTokenRequest | 

    try:
        # Create API keys
        api_response = api_instance.create_api_token(org_id, create_api_token_request)
        print("The response of TokensApi->create_api_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->create_api_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_api_token_request** | [**CreateApiTokenRequest**](CreateApiTokenRequest.md)|  | 

### Return type

[**CreateApiToken201Response**](CreateApiToken201Response.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_api_token**
> ListApiTokens200ResponseDataInner get_api_token(org_id, token_id)

Get API keys

Returns metadata for a specific API token. The token secret is never returned.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_api_tokens200_response_data_inner import ListApiTokens200ResponseDataInner
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
    api_instance = zippendo.TokensApi(api_client)
    org_id = 'org_4d8af01qw2' # str | Organization ID
    token_id = 'tok_6e2fa83ij9' # str | API Token ID

    try:
        # Get API keys
        api_response = api_instance.get_api_token(org_id, token_id)
        print("The response of TokensApi->get_api_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->get_api_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **token_id** | **str**| API Token ID | 

### Return type

[**ListApiTokens200ResponseDataInner**](ListApiTokens200ResponseDataInner.md)

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

# **list_api_tokens**
> ListApiTokens200Response list_api_tokens(org_id, page=page, limit=limit)

List API keys

Returns a paginated list of API tokens belonging to the specified organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_api_tokens200_response import ListApiTokens200Response
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
    api_instance = zippendo.TokensApi(api_client)
    org_id = 'org_4d8af01qw2' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)

    try:
        # List API keys
        api_response = api_instance.list_api_tokens(org_id, page=page, limit=limit)
        print("The response of TokensApi->list_api_tokens:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->list_api_tokens: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]

### Return type

[**ListApiTokens200Response**](ListApiTokens200Response.md)

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

# **revoke_api_token**
> RevokeApiToken200Response revoke_api_token(org_id, token_id)

Revoke API keys

Revokes and deletes an API token.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.revoke_api_token200_response import RevokeApiToken200Response
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
    api_instance = zippendo.TokensApi(api_client)
    org_id = 'org_4d8af01qw2' # str | Organization ID
    token_id = 'tok_6e2fa83ij9' # str | API Token ID

    try:
        # Revoke API keys
        api_response = api_instance.revoke_api_token(org_id, token_id)
        print("The response of TokensApi->revoke_api_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->revoke_api_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **token_id** | **str**| API Token ID | 

### Return type

[**RevokeApiToken200Response**](RevokeApiToken200Response.md)

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

# **update_api_token**
> ListApiTokens200ResponseDataInner update_api_token(org_id, token_id, update_api_token_request)

Update API keys

Updates the name of an API token.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_api_tokens200_response_data_inner import ListApiTokens200ResponseDataInner
from zippendo.models.update_api_token_request import UpdateApiTokenRequest
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
    api_instance = zippendo.TokensApi(api_client)
    org_id = 'org_4d8af01qw2' # str | Organization ID
    token_id = 'tok_6e2fa83ij9' # str | API Token ID
    update_api_token_request = zippendo.UpdateApiTokenRequest() # UpdateApiTokenRequest | 

    try:
        # Update API keys
        api_response = api_instance.update_api_token(org_id, token_id, update_api_token_request)
        print("The response of TokensApi->update_api_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->update_api_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **token_id** | **str**| API Token ID | 
 **update_api_token_request** | [**UpdateApiTokenRequest**](UpdateApiTokenRequest.md)|  | 

### Return type

[**ListApiTokens200ResponseDataInner**](ListApiTokens200ResponseDataInner.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verify_api_token**
> VerifyApiToken200Response verify_api_token(verify_api_token_request)

Verify API keys

Verifies whether an API token is valid and returns its metadata.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.verify_api_token200_response import VerifyApiToken200Response
from zippendo.models.verify_api_token_request import VerifyApiTokenRequest
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
    api_instance = zippendo.TokensApi(api_client)
    verify_api_token_request = zippendo.VerifyApiTokenRequest() # VerifyApiTokenRequest | 

    try:
        # Verify API keys
        api_response = api_instance.verify_api_token(verify_api_token_request)
        print("The response of TokensApi->verify_api_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TokensApi->verify_api_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verify_api_token_request** | [**VerifyApiTokenRequest**](VerifyApiTokenRequest.md)|  | 

### Return type

[**VerifyApiToken200Response**](VerifyApiToken200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


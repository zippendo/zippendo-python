# zippendo.AddressesApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_address**](AddressesApi.md#create_address) | **POST** /orgs/{orgId}/addresses | Create address
[**delete_address**](AddressesApi.md#delete_address) | **DELETE** /orgs/{orgId}/addresses/{addressId} | Delete address
[**get_address**](AddressesApi.md#get_address) | **GET** /orgs/{orgId}/addresses/{addressId} | Get address
[**list_addresses**](AddressesApi.md#list_addresses) | **GET** /orgs/{orgId}/addresses | List addresses
[**update_address**](AddressesApi.md#update_address) | **PUT** /orgs/{orgId}/addresses/{addressId} | Update address


# **create_address**
> ListAddresses200ResponseDataInner create_address(org_id, create_address_request)

Create address

Creates a new sender, pickup or return address for the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_address_request import CreateAddressRequest
from zippendo.models.list_addresses200_response_data_inner import ListAddresses200ResponseDataInner
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
    api_instance = zippendo.AddressesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    create_address_request = zippendo.CreateAddressRequest() # CreateAddressRequest | 

    try:
        # Create address
        api_response = api_instance.create_address(org_id, create_address_request)
        print("The response of AddressesApi->create_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->create_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_address_request** | [**CreateAddressRequest**](CreateAddressRequest.md)|  | 

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Default Response |  -  |
**400** | Default Response |  -  |
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_address**
> str delete_address(org_id, address_id)

Delete address

Deletes an address belonging to the organization.

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
    api_instance = zippendo.AddressesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    address_id = 'addr_01HZX9K2QF' # str | Address ID

    try:
        # Delete address
        api_response = api_instance.delete_address(org_id, address_id)
        print("The response of AddressesApi->delete_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->delete_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **address_id** | **str**| Address ID | 

### Return type

**str**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_address**
> ListAddresses200ResponseDataInner get_address(org_id, address_id)

Get address

Returns a single address belonging to the organization, identified by its ID.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_addresses200_response_data_inner import ListAddresses200ResponseDataInner
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
    api_instance = zippendo.AddressesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    address_id = 'addr_01HZX9K2QF' # str | Address ID

    try:
        # Get address
        api_response = api_instance.get_address(org_id, address_id)
        print("The response of AddressesApi->get_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->get_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **address_id** | **str**| Address ID | 

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_addresses**
> ListAddresses200Response list_addresses(org_id, page=page, limit=limit, type=type)

List addresses

Returns a paginated list of addresses for the organization, optionally filtered by type.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_addresses200_response import ListAddresses200Response
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
    api_instance = zippendo.AddressesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)
    type = 'sender' # str | Filter by address type (sender, pickup, return) (optional)

    try:
        # List addresses
        api_response = api_instance.list_addresses(org_id, page=page, limit=limit, type=type)
        print("The response of AddressesApi->list_addresses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->list_addresses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]
 **type** | **str**| Filter by address type (sender, pickup, return) | [optional] 

### Return type

[**ListAddresses200Response**](ListAddresses200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_address**
> ListAddresses200ResponseDataInner update_address(org_id, address_id, update_address_request)

Update address

Updates an existing address belonging to the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_addresses200_response_data_inner import ListAddresses200ResponseDataInner
from zippendo.models.update_address_request import UpdateAddressRequest
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
    api_instance = zippendo.AddressesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    address_id = 'addr_01HZX9K2QF' # str | Address ID
    update_address_request = zippendo.UpdateAddressRequest() # UpdateAddressRequest | 

    try:
        # Update address
        api_response = api_instance.update_address(org_id, address_id, update_address_request)
        print("The response of AddressesApi->update_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AddressesApi->update_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **address_id** | **str**| Address ID | 
 **update_address_request** | [**UpdateAddressRequest**](UpdateAddressRequest.md)|  | 

### Return type

[**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md)

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


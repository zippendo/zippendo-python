# zippendo.CarriersApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**connect_carrier**](CarriersApi.md#connect_carrier) | **POST** /orgs/{orgId}/carriers | Connect carrier
[**disconnect_carrier**](CarriersApi.md#disconnect_carrier) | **DELETE** /orgs/{orgId}/carriers/{carrierId} | Disconnect carrier
[**get_carrier**](CarriersApi.md#get_carrier) | **GET** /orgs/{orgId}/carriers/{carrierId} | Get carrier
[**list_carrier_product_service_points**](CarriersApi.md#list_carrier_product_service_points) | **POST** /orgs/{orgId}/carriers/{carrierId}/products/{productId}/service-points | List product service points
[**list_carrier_products**](CarriersApi.md#list_carrier_products) | **GET** /orgs/{orgId}/carriers/{carrierId}/products | List carrier products
[**list_carriers**](CarriersApi.md#list_carriers) | **GET** /orgs/{orgId}/carriers | List carriers
[**update_carrier**](CarriersApi.md#update_carrier) | **PUT** /orgs/{orgId}/carriers/{carrierId} | Update carrier


# **connect_carrier**
> ListCarriers200ResponseDataInner connect_carrier(org_id, connect_carrier_request)

Connect carrier

Connects a new carrier to the organization with its configuration.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.connect_carrier_request import ConnectCarrierRequest
from zippendo.models.list_carriers200_response_data_inner import ListCarriers200ResponseDataInner
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    connect_carrier_request = zippendo.ConnectCarrierRequest() # ConnectCarrierRequest | 

    try:
        # Connect carrier
        api_response = api_instance.connect_carrier(org_id, connect_carrier_request)
        print("The response of CarriersApi->connect_carrier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->connect_carrier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **connect_carrier_request** | [**ConnectCarrierRequest**](ConnectCarrierRequest.md)|  | 

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

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
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **disconnect_carrier**
> str disconnect_carrier(org_id, carrier_id)

Disconnect carrier

Disconnects a carrier from the organization.

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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    carrier_id = 'carr_01HZX9K2QF' # str | Carrier ID

    try:
        # Disconnect carrier
        api_response = api_instance.disconnect_carrier(org_id, carrier_id)
        print("The response of CarriersApi->disconnect_carrier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->disconnect_carrier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **carrier_id** | **str**| Carrier ID | 

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

# **get_carrier**
> ListCarriers200ResponseDataInner get_carrier(org_id, carrier_id)

Get carrier

Returns a single connected carrier.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_carriers200_response_data_inner import ListCarriers200ResponseDataInner
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    carrier_id = 'carr_01HZX9K2QF' # str | Carrier ID

    try:
        # Get carrier
        api_response = api_instance.get_carrier(org_id, carrier_id)
        print("The response of CarriersApi->get_carrier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->get_carrier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **carrier_id** | **str**| Carrier ID | 

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

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

# **list_carrier_product_service_points**
> List[ListCarrierProductServicePoints200ResponseInner] list_carrier_product_service_points(org_id, carrier_id, product_id, list_carrier_product_service_points_request)

List product service points

Returns pickup service points near a location for a specific carrier product.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_carrier_product_service_points200_response_inner import ListCarrierProductServicePoints200ResponseInner
from zippendo.models.list_carrier_product_service_points_request import ListCarrierProductServicePointsRequest
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    carrier_id = 'carr_01HZX9K2QF' # str | Carrier ID
    product_id = 'PNL13' # str | Carrier product ID
    list_carrier_product_service_points_request = zippendo.ListCarrierProductServicePointsRequest() # ListCarrierProductServicePointsRequest | 

    try:
        # List product service points
        api_response = api_instance.list_carrier_product_service_points(org_id, carrier_id, product_id, list_carrier_product_service_points_request)
        print("The response of CarriersApi->list_carrier_product_service_points:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->list_carrier_product_service_points: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **carrier_id** | **str**| Carrier ID | 
 **product_id** | **str**| Carrier product ID | 
 **list_carrier_product_service_points_request** | [**ListCarrierProductServicePointsRequest**](ListCarrierProductServicePointsRequest.md)|  | 

### Return type

[**List[ListCarrierProductServicePoints200ResponseInner]**](ListCarrierProductServicePoints200ResponseInner.md)

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

# **list_carrier_products**
> List[ListCarrierProducts200ResponseInner] list_carrier_products(org_id, carrier_id)

List carrier products

Returns the shipping products available for a connected carrier.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_carrier_products200_response_inner import ListCarrierProducts200ResponseInner
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    carrier_id = 'carr_01HZX9K2QF' # str | Carrier ID

    try:
        # List carrier products
        api_response = api_instance.list_carrier_products(org_id, carrier_id)
        print("The response of CarriersApi->list_carrier_products:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->list_carrier_products: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **carrier_id** | **str**| Carrier ID | 

### Return type

[**List[ListCarrierProducts200ResponseInner]**](ListCarrierProducts200ResponseInner.md)

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

# **list_carriers**
> ListCarriers200Response list_carriers(org_id, page=page, limit=limit, brand_id=brand_id, brand_scope=brand_scope)

List carriers

Returns a paginated list of carriers connected to the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_carriers200_response import ListCarriers200Response
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)
    brand_id = 'brnd_8f3kd92ld0' # str | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)
    brand_scope = 'own' # str | How the brand context narrows this list: \"own\" returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \"shared\" returns only unassigned organization-wide rows, \"both\" (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \"shared\" returns no rows, since those records are never visible organization-wide from within a brand context. (optional)

    try:
        # List carriers
        api_response = api_instance.list_carriers(org_id, page=page, limit=limit, brand_id=brand_id, brand_scope=brand_scope)
        print("The response of CarriersApi->list_carriers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->list_carriers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]
 **brand_id** | **str**| Filter by brand. Pass a brand ID, or \&quot;none\&quot; for records not assigned to any brand. | [optional] 
 **brand_scope** | **str**| How the brand context narrows this list: \&quot;own\&quot; returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \&quot;shared\&quot; returns only unassigned organization-wide rows, \&quot;both\&quot; (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \&quot;shared\&quot; returns no rows, since those records are never visible organization-wide from within a brand context. | [optional] 

### Return type

[**ListCarriers200Response**](ListCarriers200Response.md)

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

# **update_carrier**
> ListCarriers200ResponseDataInner update_carrier(org_id, carrier_id, update_carrier_request)

Update carrier

Updates a connected carrier's configuration or name.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_carriers200_response_data_inner import ListCarriers200ResponseDataInner
from zippendo.models.update_carrier_request import UpdateCarrierRequest
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
    api_instance = zippendo.CarriersApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    carrier_id = 'carr_01HZX9K2QF' # str | Carrier ID
    update_carrier_request = zippendo.UpdateCarrierRequest() # UpdateCarrierRequest | 

    try:
        # Update carrier
        api_response = api_instance.update_carrier(org_id, carrier_id, update_carrier_request)
        print("The response of CarriersApi->update_carrier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarriersApi->update_carrier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **carrier_id** | **str**| Carrier ID | 
 **update_carrier_request** | [**UpdateCarrierRequest**](UpdateCarrierRequest.md)|  | 

### Return type

[**ListCarriers200ResponseDataInner**](ListCarriers200ResponseDataInner.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |
**400** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


# zippendo.ShipmentsApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**batch_send_shipments**](ShipmentsApi.md#batch_send_shipments) | **POST** /orgs/{orgId}/shipments/batch-send | Batch send shipments
[**batch_split_shipment**](ShipmentsApi.md#batch_split_shipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/batch-split-shipment | Batch split shipment
[**create_return_shipment**](ShipmentsApi.md#create_return_shipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/create-return | Create return shipment
[**create_shipment**](ShipmentsApi.md#create_shipment) | **POST** /orgs/{orgId}/shipments | Create shipment
[**delete_shipment**](ShipmentsApi.md#delete_shipment) | **DELETE** /orgs/{orgId}/shipments/{shipmentId} | Delete shipment
[**get_shipment**](ShipmentsApi.md#get_shipment) | **GET** /orgs/{orgId}/shipments/{shipmentId} | Get shipment
[**get_shipment_document_content**](ShipmentsApi.md#get_shipment_document_content) | **GET** /orgs/{orgId}/shipments/{shipmentId}/documents/{documentId}/content | Download shipment document
[**list_shipments**](ShipmentsApi.md#list_shipments) | **GET** /orgs/{orgId}/shipments | List shipments
[**send_shipment**](ShipmentsApi.md#send_shipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/send | Send shipment
[**split_shipment**](ShipmentsApi.md#split_shipment) | **POST** /orgs/{orgId}/shipments/{shipmentId}/split-shipment | Split shipment
[**split_shipment_parcel**](ShipmentsApi.md#split_shipment_parcel) | **POST** /orgs/{orgId}/shipments/{shipmentId}/split-parcel | Split parcels
[**track_shipment**](ShipmentsApi.md#track_shipment) | **GET** /orgs/{orgId}/shipments/{shipmentId}/tracking | Get shipment tracking
[**update_shipment**](ShipmentsApi.md#update_shipment) | **PATCH** /orgs/{orgId}/shipments/{shipmentId} | Update shipment


# **batch_send_shipments**
> BatchSendShipments200Response batch_send_shipments(org_id, batch_send_shipments_request)

Batch send shipments

Book multiple pending/error shipments with their carriers in one request. Each shipment is processed independently and reported in `results`; a failure on one shipment never aborts the others. Use it to send every shipment on an order at once.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.batch_send_shipments200_response import BatchSendShipments200Response
from zippendo.models.batch_send_shipments_request import BatchSendShipmentsRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    batch_send_shipments_request = zippendo.BatchSendShipmentsRequest() # BatchSendShipmentsRequest | 

    try:
        # Batch send shipments
        api_response = api_instance.batch_send_shipments(org_id, batch_send_shipments_request)
        print("The response of ShipmentsApi->batch_send_shipments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->batch_send_shipments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **batch_send_shipments_request** | [**BatchSendShipmentsRequest**](BatchSendShipmentsRequest.md)|  | 

### Return type

[**BatchSendShipments200Response**](BatchSendShipments200Response.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **batch_split_shipment**
> BatchSplitShipment201Response batch_split_shipment(org_id, shipment_id, batch_split_shipment_request)

Batch split shipment

Split a parcel into multiple new shipments with per-line quantities in a single atomic operation. Only draft or pending shipments can be split.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.batch_split_shipment201_response import BatchSplitShipment201Response
from zippendo.models.batch_split_shipment_request import BatchSplitShipmentRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.
    batch_split_shipment_request = zippendo.BatchSplitShipmentRequest() # BatchSplitShipmentRequest | 

    try:
        # Batch split shipment
        api_response = api_instance.batch_split_shipment(org_id, shipment_id, batch_split_shipment_request)
        print("The response of ShipmentsApi->batch_split_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->batch_split_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 
 **batch_split_shipment_request** | [**BatchSplitShipmentRequest**](BatchSplitShipmentRequest.md)|  | 

### Return type

[**BatchSplitShipment201Response**](BatchSplitShipment201Response.md)

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

# **create_return_shipment**
> CreateShipment201Response create_return_shipment(org_id, shipment_id)

Create return shipment

Create and auto-send a return shipment from a dispatched outbound shipment with swapped sender/receiver. Requires a configured return shipping rule.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipment201_response import CreateShipment201Response
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.

    try:
        # Create return shipment
        api_response = api_instance.create_return_shipment(org_id, shipment_id)
        print("The response of ShipmentsApi->create_return_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->create_return_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

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
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_shipment**
> CreateShipment201Response create_shipment(org_id, create_shipment_request)

Create shipment

Create a new shipment for an organization. When orderId is provided, parties and parcels are derived from the order.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipment201_response import CreateShipment201Response
from zippendo.models.create_shipment_request import CreateShipmentRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    create_shipment_request = zippendo.CreateShipmentRequest() # CreateShipmentRequest | 

    try:
        # Create shipment
        api_response = api_instance.create_shipment(org_id, create_shipment_request)
        print("The response of ShipmentsApi->create_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->create_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_shipment_request** | [**CreateShipmentRequest**](CreateShipmentRequest.md)|  | 

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

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

# **delete_shipment**
> RevokeApiToken200Response delete_shipment(org_id, shipment_id)

Delete shipment

Delete a shipment. Only shipments in pending status can be deleted.

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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.

    try:
        # Delete shipment
        api_response = api_instance.delete_shipment(org_id, shipment_id)
        print("The response of ShipmentsApi->delete_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->delete_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 

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
**400** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_shipment**
> CreateShipment201Response get_shipment(org_id, shipment_id)

Get shipment

Retrieve a single shipment by its ID, including parcels, parties, documents and activity.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipment201_response import CreateShipment201Response
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.

    try:
        # Get shipment
        api_response = api_instance.get_shipment(org_id, shipment_id)
        print("The response of ShipmentsApi->get_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->get_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

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

# **get_shipment_document_content**
> get_shipment_document_content(org_id, shipment_id, document_id, disposition=disposition, filename=filename)

Download shipment document

Streams a shipment document or label file from storage.

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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.
    document_id = 'doc_8f3a2b1c' # str | Document identifier.
    disposition = 'inline' # str | Render the document inline (default) or force a download. (optional) (default to 'inline')
    filename = 'label' # str | Suggested filename (without extension) for attachment downloads. (optional)

    try:
        # Download shipment document
        api_instance.get_shipment_document_content(org_id, shipment_id, document_id, disposition=disposition, filename=filename)
    except Exception as e:
        print("Exception when calling ShipmentsApi->get_shipment_document_content: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 
 **document_id** | **str**| Document identifier. | 
 **disposition** | **str**| Render the document inline (default) or force a download. | [optional] [default to &#39;inline&#39;]
 **filename** | **str**| Suggested filename (without extension) for attachment downloads. | [optional] 

### Return type

void (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_shipments**
> ListShipments200Response list_shipments(org_id, page=page, limit=limit, brand_id=brand_id)

List shipments

List all shipments for an organization, paginated and ordered by newest first.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_shipments200_response import ListShipments200Response
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)
    brand_id = 'brnd_8f3kd92ld0' # str | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)

    try:
        # List shipments
        api_response = api_instance.list_shipments(org_id, page=page, limit=limit, brand_id=brand_id)
        print("The response of ShipmentsApi->list_shipments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->list_shipments: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]
 **brand_id** | **str**| Filter by brand. Pass a brand ID, or \&quot;none\&quot; for records not assigned to any brand. | [optional] 

### Return type

[**ListShipments200Response**](ListShipments200Response.md)

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
**403** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_shipment**
> CreateShipment201Response send_shipment(org_id, shipment_id)

Send shipment

Book a pending or error shipment with the carrier, generating labels and tracking. Returns 422 with carrier errors if booking fails.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipment201_response import CreateShipment201Response
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.

    try:
        # Send shipment
        api_response = api_instance.send_shipment(org_id, shipment_id)
        print("The response of ShipmentsApi->send_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->send_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

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
**403** | Default Response |  -  |
**404** | Default Response |  -  |
**422** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **split_shipment**
> SplitShipment201Response split_shipment(org_id, shipment_id, split_shipment_request)

Split shipment

Move order lines from a parcel into a new shipment. Only draft or pending shipments can be split.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.split_shipment201_response import SplitShipment201Response
from zippendo.models.split_shipment_request import SplitShipmentRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.
    split_shipment_request = zippendo.SplitShipmentRequest() # SplitShipmentRequest | 

    try:
        # Split shipment
        api_response = api_instance.split_shipment(org_id, shipment_id, split_shipment_request)
        print("The response of ShipmentsApi->split_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->split_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 
 **split_shipment_request** | [**SplitShipmentRequest**](SplitShipmentRequest.md)|  | 

### Return type

[**SplitShipment201Response**](SplitShipment201Response.md)

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

# **split_shipment_parcel**
> SplitShipmentParcel200Response split_shipment_parcel(org_id, shipment_id, split_shipment_parcel_request)

Split parcels

Redistribute order lines across parcels within a shipment, moving lines between parcels and creating new ones. Only draft, pending or error shipments can be modified.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.split_shipment_parcel200_response import SplitShipmentParcel200Response
from zippendo.models.split_shipment_parcel_request import SplitShipmentParcelRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.
    split_shipment_parcel_request = zippendo.SplitShipmentParcelRequest() # SplitShipmentParcelRequest | 

    try:
        # Split parcels
        api_response = api_instance.split_shipment_parcel(org_id, shipment_id, split_shipment_parcel_request)
        print("The response of ShipmentsApi->split_shipment_parcel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->split_shipment_parcel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 
 **split_shipment_parcel_request** | [**SplitShipmentParcelRequest**](SplitShipmentParcelRequest.md)|  | 

### Return type

[**SplitShipmentParcel200Response**](SplitShipmentParcel200Response.md)

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

# **track_shipment**
> TrackShipment200Response track_shipment(org_id, shipment_id)

Get shipment tracking

Retrieve the tracking timeline for a shipment, including current status and all carrier events.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.track_shipment200_response import TrackShipment200Response
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.

    try:
        # Get shipment tracking
        api_response = api_instance.track_shipment(org_id, shipment_id)
        print("The response of ShipmentsApi->track_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->track_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 

### Return type

[**TrackShipment200Response**](TrackShipment200Response.md)

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

# **update_shipment**
> CreateShipment201Response update_shipment(org_id, shipment_id, update_shipment_request)

Update shipment

Update an existing shipment. Only draft, pending or error shipments can be updated; an applied shipping rule overrides carrier settings and sender party.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipment201_response import CreateShipment201Response
from zippendo.models.update_shipment_request import UpdateShipmentRequest
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
    api_instance = zippendo.ShipmentsApi(api_client)
    org_id = 'org_1a2b3c4d' # str | Organization identifier.
    shipment_id = 'shp_4d9e7a2f' # str | Shipment identifier.
    update_shipment_request = zippendo.UpdateShipmentRequest() # UpdateShipmentRequest | 

    try:
        # Update shipment
        api_response = api_instance.update_shipment(org_id, shipment_id, update_shipment_request)
        print("The response of ShipmentsApi->update_shipment:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ShipmentsApi->update_shipment: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization identifier. | 
 **shipment_id** | **str**| Shipment identifier. | 
 **update_shipment_request** | [**UpdateShipmentRequest**](UpdateShipmentRequest.md)|  | 

### Return type

[**CreateShipment201Response**](CreateShipment201Response.md)

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


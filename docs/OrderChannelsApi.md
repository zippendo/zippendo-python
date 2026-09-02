# zippendo.OrderChannelsApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_order_channel**](OrderChannelsApi.md#create_order_channel) | **POST** /orgs/{orgId}/order-channels | Create order channel
[**create_order_channel_webhook_secret**](OrderChannelsApi.md#create_order_channel_webhook_secret) | **POST** /orgs/{orgId}/order-channels/{channelId}/webhook-secret | Create or rotate webhook signing secret
[**delete_order_channel**](OrderChannelsApi.md#delete_order_channel) | **DELETE** /orgs/{orgId}/order-channels/{channelId} | Delete order channel
[**get_order_channel**](OrderChannelsApi.md#get_order_channel) | **GET** /orgs/{orgId}/order-channels/{channelId} | Get order channel
[**get_order_channel_webhook_status**](OrderChannelsApi.md#get_order_channel_webhook_status) | **GET** /orgs/{orgId}/order-channels/{channelId}/webhooks | Get channel webhook status
[**list_order_channels**](OrderChannelsApi.md#list_order_channels) | **GET** /orgs/{orgId}/order-channels | List order channels
[**revoke_order_channel_webhook_secret**](OrderChannelsApi.md#revoke_order_channel_webhook_secret) | **DELETE** /orgs/{orgId}/order-channels/{channelId}/webhook-secret | Revoke webhook signing secret
[**update_order_channel**](OrderChannelsApi.md#update_order_channel) | **PATCH** /orgs/{orgId}/order-channels/{channelId} | Update order channel


# **create_order_channel**
> ListOrderChannels200ResponseDataInner create_order_channel(org_id, create_order_channel_request)

Create order channel

Creates a new order channel for an organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_order_channel_request import CreateOrderChannelRequest
from zippendo.models.list_order_channels200_response_data_inner import ListOrderChannels200ResponseDataInner
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    create_order_channel_request = zippendo.CreateOrderChannelRequest() # CreateOrderChannelRequest | 

    try:
        # Create order channel
        api_response = api_instance.create_order_channel(org_id, create_order_channel_request)
        print("The response of OrderChannelsApi->create_order_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->create_order_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_order_channel_request** | [**CreateOrderChannelRequest**](CreateOrderChannelRequest.md)|  | 

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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

# **create_order_channel_webhook_secret**
> CreateOrderChannelWebhookSecret201Response create_order_channel_webhook_secret(org_id, channel_id)

Create or rotate webhook signing secret

Generates (or rotates) the custom channel's webhook signing secret used to authenticate order pushes to the ingest URL. The secret is returned only once. Rotating invalidates the previous secret immediately.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_order_channel_webhook_secret201_response import CreateOrderChannelWebhookSecret201Response
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.

    try:
        # Create or rotate webhook signing secret
        api_response = api_instance.create_order_channel_webhook_secret(org_id, channel_id)
        print("The response of OrderChannelsApi->create_order_channel_webhook_secret:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->create_order_channel_webhook_secret: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 

### Return type

[**CreateOrderChannelWebhookSecret201Response**](CreateOrderChannelWebhookSecret201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Default Response |  -  |
**400** | Default Response |  -  |
**403** | Default Response |  -  |
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_order_channel**
> RevokeApiToken200Response delete_order_channel(org_id, channel_id)

Delete order channel

Deletes an order channel and cascades deletion of its orders.

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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.

    try:
        # Delete order channel
        api_response = api_instance.delete_order_channel(org_id, channel_id)
        print("The response of OrderChannelsApi->delete_order_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->delete_order_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 

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

# **get_order_channel**
> ListOrderChannels200ResponseDataInner get_order_channel(org_id, channel_id)

Get order channel

Returns a single order channel by ID, including its linked shipping rules.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_order_channels200_response_data_inner import ListOrderChannels200ResponseDataInner
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.

    try:
        # Get order channel
        api_response = api_instance.get_order_channel(org_id, channel_id)
        print("The response of OrderChannelsApi->get_order_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->get_order_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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

# **get_order_channel_webhook_status**
> GetOrderChannelWebhookStatus200Response get_order_channel_webhook_status(org_id, channel_id)

Get channel webhook status

Returns whether webhooks are enabled and lists the webhooks registered with the platform.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_order_channel_webhook_status200_response import GetOrderChannelWebhookStatus200Response
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.

    try:
        # Get channel webhook status
        api_response = api_instance.get_order_channel_webhook_status(org_id, channel_id)
        print("The response of OrderChannelsApi->get_order_channel_webhook_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->get_order_channel_webhook_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 

### Return type

[**GetOrderChannelWebhookStatus200Response**](GetOrderChannelWebhookStatus200Response.md)

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

# **list_order_channels**
> ListOrderChannels200Response list_order_channels(org_id, page=page, limit=limit, brand_id=brand_id, brand_scope=brand_scope, type=type, enabled=enabled, search=search)

List order channels

Returns a paginated list of order channels for an organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_order_channels200_response import ListOrderChannels200Response
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)
    brand_id = 'brnd_8f3kd92ld0' # str | Filter by brand. Pass a brand ID, or \"none\" for records not assigned to any brand. (optional)
    brand_scope = 'own' # str | How the brand context narrows this list: \"own\" returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \"shared\" returns only unassigned organization-wide rows, \"both\" (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \"shared\" returns no rows, since those records are never visible organization-wide from within a brand context. (optional)
    type = 'shopify' # str | Filter by channel type. (optional)
    enabled = 'true' # str | Filter by enabled state. (optional)
    search = 'Anna\'s Shopify Store' # str | Search by channel name. (optional)

    try:
        # List order channels
        api_response = api_instance.list_order_channels(org_id, page=page, limit=limit, brand_id=brand_id, brand_scope=brand_scope, type=type, enabled=enabled, search=search)
        print("The response of OrderChannelsApi->list_order_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->list_order_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]
 **brand_id** | **str**| Filter by brand. Pass a brand ID, or \&quot;none\&quot; for records not assigned to any brand. | [optional] 
 **brand_scope** | **str**| How the brand context narrows this list: \&quot;own\&quot; returns only rows assigned to the current brand (requires a brand session, a brand-bound token, or the X-Zippendo-Brand header), \&quot;shared\&quot; returns only unassigned organization-wide rows, \&quot;both\&quot; (default) returns both. The X-Zippendo-Brand-Scope header supplies a default when the parameter is omitted. For strictly brand-owned records (orders, shipments), a brand-scoped request combined with \&quot;shared\&quot; returns no rows, since those records are never visible organization-wide from within a brand context. | [optional] 
 **type** | **str**| Filter by channel type. | [optional] 
 **enabled** | **str**| Filter by enabled state. | [optional] 
 **search** | **str**| Search by channel name. | [optional] 

### Return type

[**ListOrderChannels200Response**](ListOrderChannels200Response.md)

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

# **revoke_order_channel_webhook_secret**
> RevokeOrderChannelWebhookSecret200Response revoke_order_channel_webhook_secret(org_id, channel_id)

Revoke webhook signing secret

Revokes the custom channel's webhook signing secret. All subsequent pushes to the ingest URL are rejected until a new secret is generated.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.revoke_order_channel_webhook_secret200_response import RevokeOrderChannelWebhookSecret200Response
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.

    try:
        # Revoke webhook signing secret
        api_response = api_instance.revoke_order_channel_webhook_secret(org_id, channel_id)
        print("The response of OrderChannelsApi->revoke_order_channel_webhook_secret:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->revoke_order_channel_webhook_secret: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 

### Return type

[**RevokeOrderChannelWebhookSecret200Response**](RevokeOrderChannelWebhookSecret200Response.md)

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

# **update_order_channel**
> ListOrderChannels200ResponseDataInner update_order_channel(org_id, channel_id, update_order_channel_request)

Update order channel

Updates an order channel and its linked shipping rules.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_order_channels200_response_data_inner import ListOrderChannels200ResponseDataInner
from zippendo.models.update_order_channel_request import UpdateOrderChannelRequest
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
    api_instance = zippendo.OrderChannelsApi(api_client)
    org_id = 'clz9k2f0a0000abcd0000zzzz' # str | Organization ID.
    channel_id = 'clz9k2f0a0001abcd1234efgh' # str | Order channel ID.
    update_order_channel_request = zippendo.UpdateOrderChannelRequest() # UpdateOrderChannelRequest | 

    try:
        # Update order channel
        api_response = api_instance.update_order_channel(org_id, channel_id, update_order_channel_request)
        print("The response of OrderChannelsApi->update_order_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrderChannelsApi->update_order_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID. | 
 **channel_id** | **str**| Order channel ID. | 
 **update_order_channel_request** | [**UpdateOrderChannelRequest**](UpdateOrderChannelRequest.md)|  | 

### Return type

[**ListOrderChannels200ResponseDataInner**](ListOrderChannels200ResponseDataInner.md)

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


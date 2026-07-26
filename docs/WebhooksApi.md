# zippendo.WebhooksApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_org_webhook**](WebhooksApi.md#create_org_webhook) | **POST** /orgs/{orgId}/webhooks | Create webhook
[**delete_org_webhook**](WebhooksApi.md#delete_org_webhook) | **DELETE** /orgs/{orgId}/webhooks/{webhookId} | Delete webhook
[**get_org_webhook**](WebhooksApi.md#get_org_webhook) | **GET** /orgs/{orgId}/webhooks/{webhookId} | Get webhook
[**list_org_webhook_deliveries**](WebhooksApi.md#list_org_webhook_deliveries) | **GET** /orgs/{orgId}/webhooks/{webhookId}/deliveries | List webhook deliveries
[**list_org_webhooks**](WebhooksApi.md#list_org_webhooks) | **GET** /orgs/{orgId}/webhooks | List webhooks
[**test_org_webhook**](WebhooksApi.md#test_org_webhook) | **POST** /orgs/{orgId}/webhooks/{webhookId}/test | Test webhook
[**update_org_webhook**](WebhooksApi.md#update_org_webhook) | **PATCH** /orgs/{orgId}/webhooks/{webhookId} | Update webhook


# **create_org_webhook**
> CreateOrgWebhook201Response create_org_webhook(org_id, create_org_webhook_request)

Create webhook

Create a new webhook endpoint for an organization that receives event notifications.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_org_webhook201_response import CreateOrgWebhook201Response
from zippendo.models.create_org_webhook_request import CreateOrgWebhookRequest
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    create_org_webhook_request = zippendo.CreateOrgWebhookRequest() # CreateOrgWebhookRequest | 

    try:
        # Create webhook
        api_response = api_instance.create_org_webhook(org_id, create_org_webhook_request)
        print("The response of WebhooksApi->create_org_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->create_org_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_org_webhook_request** | [**CreateOrgWebhookRequest**](CreateOrgWebhookRequest.md)|  | 

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

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

# **delete_org_webhook**
> DeleteOrgWebhook200Response delete_org_webhook(org_id, webhook_id)

Delete webhook

Permanently delete a webhook and all its delivery logs.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.delete_org_webhook200_response import DeleteOrgWebhook200Response
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_clx1a2b3c4' # str | Organization ID
    webhook_id = 'wh_clx1a2b3c4' # str | Webhook ID

    try:
        # Delete webhook
        api_response = api_instance.delete_org_webhook(org_id, webhook_id)
        print("The response of WebhooksApi->delete_org_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->delete_org_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **webhook_id** | **str**| Webhook ID | 

### Return type

[**DeleteOrgWebhook200Response**](DeleteOrgWebhook200Response.md)

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

# **get_org_webhook**
> CreateOrgWebhook201Response get_org_webhook(org_id, webhook_id)

Get webhook

Get a specific webhook including its signing secret.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_org_webhook201_response import CreateOrgWebhook201Response
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_clx1a2b3c4' # str | Organization ID
    webhook_id = 'wh_clx1a2b3c4' # str | Webhook ID

    try:
        # Get webhook
        api_response = api_instance.get_org_webhook(org_id, webhook_id)
        print("The response of WebhooksApi->get_org_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->get_org_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **webhook_id** | **str**| Webhook ID | 

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

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

# **list_org_webhook_deliveries**
> ListOrgWebhookDeliveries200Response list_org_webhook_deliveries(org_id, webhook_id, page=page, limit=limit)

List webhook deliveries

List the delivery history for a specific webhook.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_webhook_deliveries200_response import ListOrgWebhookDeliveries200Response
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_clx1a2b3c4' # str | Organization ID
    webhook_id = 'wh_clx1a2b3c4' # str | Webhook ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)

    try:
        # List webhook deliveries
        api_response = api_instance.list_org_webhook_deliveries(org_id, webhook_id, page=page, limit=limit)
        print("The response of WebhooksApi->list_org_webhook_deliveries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->list_org_webhook_deliveries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **webhook_id** | **str**| Webhook ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]

### Return type

[**ListOrgWebhookDeliveries200Response**](ListOrgWebhookDeliveries200Response.md)

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

# **list_org_webhooks**
> ListOrgWebhooks200Response list_org_webhooks(org_id, page=page, limit=limit)

List webhooks

List all webhooks belonging to an organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_org_webhooks200_response import ListOrgWebhooks200Response
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)

    try:
        # List webhooks
        api_response = api_instance.list_org_webhooks(org_id, page=page, limit=limit)
        print("The response of WebhooksApi->list_org_webhooks:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->list_org_webhooks: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]

### Return type

[**ListOrgWebhooks200Response**](ListOrgWebhooks200Response.md)

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

# **test_org_webhook**
> TestOrgWebhook200Response test_org_webhook(org_id, webhook_id)

Test webhook

Send a test ping event to the webhook endpoint to verify connectivity.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.test_org_webhook200_response import TestOrgWebhook200Response
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_clx1a2b3c4' # str | Organization ID
    webhook_id = 'wh_clx1a2b3c4' # str | Webhook ID

    try:
        # Test webhook
        api_response = api_instance.test_org_webhook(org_id, webhook_id)
        print("The response of WebhooksApi->test_org_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->test_org_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **webhook_id** | **str**| Webhook ID | 

### Return type

[**TestOrgWebhook200Response**](TestOrgWebhook200Response.md)

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

# **update_org_webhook**
> CreateOrgWebhook201Response update_org_webhook(org_id, webhook_id, update_org_webhook_request)

Update webhook

Update the configuration of an existing webhook.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_org_webhook201_response import CreateOrgWebhook201Response
from zippendo.models.update_org_webhook_request import UpdateOrgWebhookRequest
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
    api_instance = zippendo.WebhooksApi(api_client)
    org_id = 'org_clx1a2b3c4' # str | Organization ID
    webhook_id = 'wh_clx1a2b3c4' # str | Webhook ID
    update_org_webhook_request = zippendo.UpdateOrgWebhookRequest() # UpdateOrgWebhookRequest | 

    try:
        # Update webhook
        api_response = api_instance.update_org_webhook(org_id, webhook_id, update_org_webhook_request)
        print("The response of WebhooksApi->update_org_webhook:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->update_org_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **webhook_id** | **str**| Webhook ID | 
 **update_org_webhook_request** | [**UpdateOrgWebhookRequest**](UpdateOrgWebhookRequest.md)|  | 

### Return type

[**CreateOrgWebhook201Response**](CreateOrgWebhook201Response.md)

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


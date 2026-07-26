# zippendo.CarrierCatalogApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_available_carriers**](CarrierCatalogApi.md#list_available_carriers) | **GET** /orgs/{orgId}/available-carriers | List available carriers


# **list_available_carriers**
> List[ListAvailableCarriers200ResponseInner] list_available_carriers(org_id)

List available carriers

Returns the carriers available to connect, as supported by the carrier server.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_available_carriers200_response_inner import ListAvailableCarriers200ResponseInner
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
    api_instance = zippendo.CarrierCatalogApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID

    try:
        # List available carriers
        api_response = api_instance.list_available_carriers(org_id)
        print("The response of CarrierCatalogApi->list_available_carriers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarrierCatalogApi->list_available_carriers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 

### Return type

[**List[ListAvailableCarriers200ResponseInner]**](ListAvailableCarriers200ResponseInner.md)

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
**500** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


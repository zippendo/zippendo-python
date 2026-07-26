# zippendo.BillingApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_billing_usage**](BillingApi.md#get_billing_usage) | **GET** /orgs/{orgId}/billing/usage | Get usage


# **get_billing_usage**
> GetBillingUsage200Response get_billing_usage(org_id)

Get usage

Get detailed usage statistics for the current billing period.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.get_billing_usage200_response import GetBillingUsage200Response
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
    api_instance = zippendo.BillingApi(api_client)
    org_id = 'org_8f3kd92ld0' # str | Organization ID

    try:
        # Get usage
        api_response = api_instance.get_billing_usage(org_id)
        print("The response of BillingApi->get_billing_usage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_billing_usage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 

### Return type

[**GetBillingUsage200Response**](GetBillingUsage200Response.md)

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


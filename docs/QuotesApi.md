# zippendo.QuotesApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_quote**](QuotesApi.md#create_shipping_quote) | **POST** /orgs/{orgId}/shipping-quote | Calculate shipping rates


# **create_shipping_quote**
> CreateShippingQuote200Response create_shipping_quote(org_id, create_shipping_quote_request)

Calculate shipping rates

Calculates shipping rates from configured shipping rules based on cart items and destination.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipping_quote200_response import CreateShippingQuote200Response
from zippendo.models.create_shipping_quote_request import CreateShippingQuoteRequest
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
    api_instance = zippendo.QuotesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    create_shipping_quote_request = zippendo.CreateShippingQuoteRequest() # CreateShippingQuoteRequest | 

    try:
        # Calculate shipping rates
        api_response = api_instance.create_shipping_quote(org_id, create_shipping_quote_request)
        print("The response of QuotesApi->create_shipping_quote:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->create_shipping_quote: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_shipping_quote_request** | [**CreateShippingQuoteRequest**](CreateShippingQuoteRequest.md)|  | 

### Return type

[**CreateShippingQuote200Response**](CreateShippingQuote200Response.md)

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
**404** | Default Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


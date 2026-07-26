# zippendo.RulesApi

All URIs are relative to *https://api.zippendo.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_shipping_rule**](RulesApi.md#create_shipping_rule) | **POST** /orgs/{orgId}/shipping-rules | Create shipping rule
[**delete_shipping_rule**](RulesApi.md#delete_shipping_rule) | **DELETE** /orgs/{orgId}/shipping-rules/{ruleId} | Delete shipping rule
[**get_shipping_rule**](RulesApi.md#get_shipping_rule) | **GET** /orgs/{orgId}/shipping-rules/{ruleId} | Get shipping rule
[**list_shipping_rules**](RulesApi.md#list_shipping_rules) | **GET** /orgs/{orgId}/shipping-rules | List shipping rules
[**update_shipping_rule**](RulesApi.md#update_shipping_rule) | **PATCH** /orgs/{orgId}/shipping-rules/{ruleId} | Update shipping rule


# **create_shipping_rule**
> CreateShippingRule201Response create_shipping_rule(org_id, create_shipping_rule_request)

Create shipping rule

Creates a new shipping rule with conditions and carrier product for the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipping_rule201_response import CreateShippingRule201Response
from zippendo.models.create_shipping_rule_request import CreateShippingRuleRequest
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
    api_instance = zippendo.RulesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    create_shipping_rule_request = zippendo.CreateShippingRuleRequest() # CreateShippingRuleRequest | 

    try:
        # Create shipping rule
        api_response = api_instance.create_shipping_rule(org_id, create_shipping_rule_request)
        print("The response of RulesApi->create_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RulesApi->create_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **create_shipping_rule_request** | [**CreateShippingRuleRequest**](CreateShippingRuleRequest.md)|  | 

### Return type

[**CreateShippingRule201Response**](CreateShippingRule201Response.md)

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

# **delete_shipping_rule**
> DeleteShippingRule200Response delete_shipping_rule(org_id, rule_id)

Delete shipping rule

Deletes a shipping rule belonging to the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.delete_shipping_rule200_response import DeleteShippingRule200Response
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
    api_instance = zippendo.RulesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    rule_id = 'rule_01HZX9K2QF' # str | Shipping Rule ID

    try:
        # Delete shipping rule
        api_response = api_instance.delete_shipping_rule(org_id, rule_id)
        print("The response of RulesApi->delete_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RulesApi->delete_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **rule_id** | **str**| Shipping Rule ID | 

### Return type

[**DeleteShippingRule200Response**](DeleteShippingRule200Response.md)

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

# **get_shipping_rule**
> ListShippingRules200ResponseDataInner get_shipping_rule(org_id, rule_id)

Get shipping rule

Returns a single shipping rule with its carrier, address and printer relations.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_shipping_rules200_response_data_inner import ListShippingRules200ResponseDataInner
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
    api_instance = zippendo.RulesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    rule_id = 'rule_01HZX9K2QF' # str | Shipping Rule ID

    try:
        # Get shipping rule
        api_response = api_instance.get_shipping_rule(org_id, rule_id)
        print("The response of RulesApi->get_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RulesApi->get_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **rule_id** | **str**| Shipping Rule ID | 

### Return type

[**ListShippingRules200ResponseDataInner**](ListShippingRules200ResponseDataInner.md)

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

# **list_shipping_rules**
> ListShippingRules200Response list_shipping_rules(org_id, page=page, limit=limit)

List shipping rules

Returns a paginated list of shipping rules for the organization with their relations.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.list_shipping_rules200_response import ListShippingRules200Response
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
    api_instance = zippendo.RulesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    page = 1 # int | Page number (1-based) (optional) (default to 1)
    limit = 20 # int | Items per page (max 100) (optional) (default to 20)

    try:
        # List shipping rules
        api_response = api_instance.list_shipping_rules(org_id, page=page, limit=limit)
        print("The response of RulesApi->list_shipping_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RulesApi->list_shipping_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **page** | **int**| Page number (1-based) | [optional] [default to 1]
 **limit** | **int**| Items per page (max 100) | [optional] [default to 20]

### Return type

[**ListShippingRules200Response**](ListShippingRules200Response.md)

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

# **update_shipping_rule**
> CreateShippingRule201Response update_shipping_rule(org_id, rule_id, update_shipping_rule_request)

Update shipping rule

Updates an existing shipping rule for the organization.

### Example

* Bearer (JWT) Authentication (bearerAuth):

```python
import zippendo
from zippendo.models.create_shipping_rule201_response import CreateShippingRule201Response
from zippendo.models.update_shipping_rule_request import UpdateShippingRuleRequest
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
    api_instance = zippendo.RulesApi(api_client)
    org_id = 'org_01HZX9K2QF' # str | Organization ID
    rule_id = 'rule_01HZX9K2QF' # str | Shipping Rule ID
    update_shipping_rule_request = zippendo.UpdateShippingRuleRequest() # UpdateShippingRuleRequest | 

    try:
        # Update shipping rule
        api_response = api_instance.update_shipping_rule(org_id, rule_id, update_shipping_rule_request)
        print("The response of RulesApi->update_shipping_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RulesApi->update_shipping_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**| Organization ID | 
 **rule_id** | **str**| Shipping Rule ID | 
 **update_shipping_rule_request** | [**UpdateShippingRuleRequest**](UpdateShippingRuleRequest.md)|  | 

### Return type

[**CreateShippingRule201Response**](CreateShippingRule201Response.md)

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


# CreateShippingQuote404Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** | Error type | 
**message** | **str** | Human-readable error message | 

## Example

```python
from zippendo.models.create_shipping_quote404_response import CreateShippingQuote404Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuote404Response from a JSON string
create_shipping_quote404_response_instance = CreateShippingQuote404Response.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuote404Response.to_json())

# convert the object into a dict
create_shipping_quote404_response_dict = create_shipping_quote404_response_instance.to_dict()
# create an instance of CreateShippingQuote404Response from a dict
create_shipping_quote404_response_from_dict = CreateShippingQuote404Response.from_dict(create_shipping_quote404_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



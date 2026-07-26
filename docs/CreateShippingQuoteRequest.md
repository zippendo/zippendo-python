# CreateShippingQuoteRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**destination** | [**CreateShippingQuoteRequestDestination**](CreateShippingQuoteRequestDestination.md) |  | 
**items** | [**List[CreateShippingQuoteRequestItemsInner]**](CreateShippingQuoteRequestItemsInner.md) | Cart items | 
**currency** | **str** | ISO 4217 currency code | 
**total_price_cents** | **float** | Total price in cents after discounts (optional, enables total-based conditions) | [optional] 

## Example

```python
from zippendo.models.create_shipping_quote_request import CreateShippingQuoteRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuoteRequest from a JSON string
create_shipping_quote_request_instance = CreateShippingQuoteRequest.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuoteRequest.to_json())

# convert the object into a dict
create_shipping_quote_request_dict = create_shipping_quote_request_instance.to_dict()
# create an instance of CreateShippingQuoteRequest from a dict
create_shipping_quote_request_from_dict = CreateShippingQuoteRequest.from_dict(create_shipping_quote_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



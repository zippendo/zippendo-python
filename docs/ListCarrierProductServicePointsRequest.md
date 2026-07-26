# ListCarrierProductServicePointsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address1** | **str** | Street address line 1 | 
**address2** | **str** | Street address line 2 | [optional] 
**postal_code** | **str** | Postal code | 
**state** | **str** | State or region | [optional] 
**city** | **str** | City name | 
**country_code** | **str** | ISO 3166-1 alpha-2 country code | 

## Example

```python
from zippendo.models.list_carrier_product_service_points_request import ListCarrierProductServicePointsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProductServicePointsRequest from a JSON string
list_carrier_product_service_points_request_instance = ListCarrierProductServicePointsRequest.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProductServicePointsRequest.to_json())

# convert the object into a dict
list_carrier_product_service_points_request_dict = list_carrier_product_service_points_request_instance.to_dict()
# create an instance of ListCarrierProductServicePointsRequest from a dict
list_carrier_product_service_points_request_from_dict = ListCarrierProductServicePointsRequest.from_dict(list_carrier_product_service_points_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



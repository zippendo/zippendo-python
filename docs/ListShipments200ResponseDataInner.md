# ListShipments200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipment identifier. | 
**reference** | **str** | Customer-facing shipment reference. | 
**type** | **str** | Direction of the shipment relative to the organization. | 
**carrier_settings** | [**ListShipments200ResponseDataInnerCarrierSettings**](ListShipments200ResponseDataInnerCarrierSettings.md) |  | 
**status** | **str** | Lifecycle status of the shipment. | 
**brand_id** | **str** | Brand this record belongs to, or null when it is organization-wide | 
**address** | [**ListShipments200ResponseDataInnerAddress**](ListShipments200ResponseDataInnerAddress.md) |  | [optional] 
**created_at** | **str** | Timestamp when the shipment was created. | 
**updated_at** | **str** | Timestamp when the shipment was last updated. | 

## Example

```python
from zippendo.models.list_shipments200_response_data_inner import ListShipments200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListShipments200ResponseDataInner from a JSON string
list_shipments200_response_data_inner_instance = ListShipments200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListShipments200ResponseDataInner.to_json())

# convert the object into a dict
list_shipments200_response_data_inner_dict = list_shipments200_response_data_inner_instance.to_dict()
# create an instance of ListShipments200ResponseDataInner from a dict
list_shipments200_response_data_inner_from_dict = ListShipments200ResponseDataInner.from_dict(list_shipments200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



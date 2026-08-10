# SplitShipmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parcel_id** | **str** | Parcel whose order lines are split into a new shipment. | 
**order_line_ids** | **List[str]** | Order line IDs to move. If omitted, all order lines in the parcel are moved. | [optional] 
**carrier_id** | **str** | Carrier for the new shipment. Copied from the original if omitted. | [optional] 
**product_id** | **str** | Carrier product for the new shipment. Copied from the original if omitted. | [optional] 
**services** | **List[str]** | Service codes for the new shipment. Copied from the original if omitted. | [optional] 
**additional_parameters** | [**Dict[str, CreateShippingRuleRequestAdditionalParametersValue]**](CreateShippingRuleRequestAdditionalParametersValue.md) | Carrier-specific parameters for the new shipment. Copied from the original if omitted. | [optional] 
**reference** | **str** | Reference for the new shipment. Defaults to the original reference with a suffix. | [optional] 

## Example

```python
from zippendo.models.split_shipment_request import SplitShipmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SplitShipmentRequest from a JSON string
split_shipment_request_instance = SplitShipmentRequest.from_json(json)
# print the JSON string representation of the object
print(SplitShipmentRequest.to_json())

# convert the object into a dict
split_shipment_request_dict = split_shipment_request_instance.to_dict()
# create an instance of SplitShipmentRequest from a dict
split_shipment_request_from_dict = SplitShipmentRequest.from_dict(split_shipment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



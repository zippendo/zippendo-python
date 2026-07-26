# SplitShipment201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**original_shipment** | [**CreateShipment201Response**](CreateShipment201Response.md) |  | 
**new_shipment** | [**CreateShipment201Response**](CreateShipment201Response.md) |  | 

## Example

```python
from zippendo.models.split_shipment201_response import SplitShipment201Response

# TODO update the JSON string below
json = "{}"
# create an instance of SplitShipment201Response from a JSON string
split_shipment201_response_instance = SplitShipment201Response.from_json(json)
# print the JSON string representation of the object
print(SplitShipment201Response.to_json())

# convert the object into a dict
split_shipment201_response_dict = split_shipment201_response_instance.to_dict()
# create an instance of SplitShipment201Response from a dict
split_shipment201_response_from_dict = SplitShipment201Response.from_dict(split_shipment201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



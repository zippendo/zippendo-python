# BatchSplitShipment201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**original_shipment** | [**CreateShipment201Response**](CreateShipment201Response.md) |  | 
**new_shipments** | [**List[CreateShipment201Response]**](CreateShipment201Response.md) | Newly created shipments resulting from the split. | 

## Example

```python
from zippendo.models.batch_split_shipment201_response import BatchSplitShipment201Response

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSplitShipment201Response from a JSON string
batch_split_shipment201_response_instance = BatchSplitShipment201Response.from_json(json)
# print the JSON string representation of the object
print(BatchSplitShipment201Response.to_json())

# convert the object into a dict
batch_split_shipment201_response_dict = batch_split_shipment201_response_instance.to_dict()
# create an instance of BatchSplitShipment201Response from a dict
batch_split_shipment201_response_from_dict = BatchSplitShipment201Response.from_dict(batch_split_shipment201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



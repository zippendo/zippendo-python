# ListShipments200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ListShipments200ResponseDataInner]**](ListShipments200ResponseDataInner.md) | Page of results | 
**total** | **float** | Total matching items across all pages | 
**page** | **float** | Current page number (1-based) | 
**limit** | **float** | Items per page | 
**total_pages** | **float** | Total number of pages | 

## Example

```python
from zippendo.models.list_shipments200_response import ListShipments200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListShipments200Response from a JSON string
list_shipments200_response_instance = ListShipments200Response.from_json(json)
# print the JSON string representation of the object
print(ListShipments200Response.to_json())

# convert the object into a dict
list_shipments200_response_dict = list_shipments200_response_instance.to_dict()
# create an instance of ListShipments200Response from a dict
list_shipments200_response_from_dict = ListShipments200Response.from_dict(list_shipments200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



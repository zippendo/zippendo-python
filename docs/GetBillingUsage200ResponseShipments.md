# GetBillingUsage200ResponseShipments


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**used** | **float** | Shipments created this period | 
**included** | **float** | Shipments included in the plan | 
**overage** | **float** | Shipments above the included allowance | 
**overage_charges** | **float** | Overage charges so far, in øre | 

## Example

```python
from zippendo.models.get_billing_usage200_response_shipments import GetBillingUsage200ResponseShipments

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseShipments from a JSON string
get_billing_usage200_response_shipments_instance = GetBillingUsage200ResponseShipments.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseShipments.to_json())

# convert the object into a dict
get_billing_usage200_response_shipments_dict = get_billing_usage200_response_shipments_instance.to_dict()
# create an instance of GetBillingUsage200ResponseShipments from a dict
get_billing_usage200_response_shipments_from_dict = GetBillingUsage200ResponseShipments.from_dict(get_billing_usage200_response_shipments_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



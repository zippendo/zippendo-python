# GetOrder200ResponseShippingRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipping rule identifier. | 
**name** | **str** | Display name of the shipping rule. | 
**carrier_id** | **str** | Carrier applied by the rule. | 
**product_id** | **str** | Carrier product applied by the rule. | 
**services** | **List[str]** | Additional service codes applied by the rule. | 
**address_id** | **str** | Sender address applied by the rule. | 
**return_shipping_rule_id** | **str** | ID of the linked return shipping rule. | [optional] 
**auto_create_return_shipment** | **bool** | Whether a return shipment is created automatically. | [optional] 
**auto_print_labels** | **bool** | Whether labels are printed automatically on send. | [optional] 
**auto_print_documents** | **bool** | Whether documents are printed automatically on send. | [optional] 
**label_printer_id** | **str** | Printer used for labels. | [optional] 
**document_printer_id** | **str** | Printer used for documents. | [optional] 

## Example

```python
from zippendo.models.get_order200_response_shipping_rule import GetOrder200ResponseShippingRule

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200ResponseShippingRule from a JSON string
get_order200_response_shipping_rule_instance = GetOrder200ResponseShippingRule.from_json(json)
# print the JSON string representation of the object
print(GetOrder200ResponseShippingRule.to_json())

# convert the object into a dict
get_order200_response_shipping_rule_dict = get_order200_response_shipping_rule_instance.to_dict()
# create an instance of GetOrder200ResponseShippingRule from a dict
get_order200_response_shipping_rule_from_dict = GetOrder200ResponseShippingRule.from_dict(get_order200_response_shipping_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



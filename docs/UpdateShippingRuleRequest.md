# UpdateShippingRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Shipping rule name | [optional] 
**description** | **str** | Optional description | [optional] 
**direction** | **str** | Whether this rule is for outbound or inbound (return) shipments | [optional] [default to 'outbound']
**carrier_id** | **str** | Carrier ID | [optional] 
**product_id** | **str** | Product ID from carrier | [optional] 
**services** | **List[str]** | List of selected services | [optional] 
**additional_parameters** | [**Dict[str, CreateShippingRuleRequestAdditionalParametersValue]**](CreateShippingRuleRequestAdditionalParametersValue.md) | Carrier-specific extra parameters, keyed by the carrier parameter &#x60;key&#x60; from the product&#39;s &#x60;additionalParameters[].key&#x60;. Omit to leave the rule&#39;s parameters unchanged. | [optional] 
**address_id** | **str** | Sender address ID | [optional] 
**receiving_countries** | **List[str]** | List of supported country codes | [optional] 
**email_notification** | **bool** | Send email notification to recipient | [optional] [default to False]
**phone_notification** | **bool** | Send SMS notification to recipient | [optional] [default to False]
**min_weight** | **float** | Minimum required weight in kg | [optional] 
**max_weight** | **float** | Maximum allowed weight in kg | [optional] 
**min_order_value** | **float** | Minimum required order value in currency units | [optional] 
**max_order_value** | **float** | Maximum allowed order value in currency units | [optional] 
**conditions** | [**List[CreateShippingRuleRequestConditionsInner]**](CreateShippingRuleRequestConditionsInner.md) | Rule conditions (weight/price/quantity) | [optional] 
**generate_proforma_invoice** | **bool** | Generate proforma invoice for shipments | [optional] [default to False]
**generate_commercial_invoice** | **bool** | Generate commercial invoice for international shipments | [optional] [default to False]
**generate_packing_list** | **bool** | Generate packing slip with package and item details | [optional] [default to False]
**auto_print_labels** | **bool** | Automatically print labels when shipment is sent | [optional] [default to False]
**auto_print_documents** | **bool** | Automatically print documents when shipment is sent | [optional] [default to False]
**label_printer_id** | **str** | ID of the label printer | [optional] 
**document_printer_id** | **str** | ID of the document printer | [optional] 
**return_shipping_rule_id** | **str** | ID of the return shipping rule | [optional] 
**auto_create_return_shipment** | **bool** | Automatically create and send a return shipment on dispatch | [optional] [default to False]

## Example

```python
from zippendo.models.update_shipping_rule_request import UpdateShippingRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateShippingRuleRequest from a JSON string
update_shipping_rule_request_instance = UpdateShippingRuleRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateShippingRuleRequest.to_json())

# convert the object into a dict
update_shipping_rule_request_dict = update_shipping_rule_request_instance.to_dict()
# create an instance of UpdateShippingRuleRequest from a dict
update_shipping_rule_request_from_dict = UpdateShippingRuleRequest.from_dict(update_shipping_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



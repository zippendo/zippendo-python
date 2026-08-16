# ListShippingRules200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipping rule identifier | 
**name** | **str** | Shipping rule name | 
**description** | **str** | Optional description | 
**direction** | **str** | Whether this rule is for outbound or inbound (return) shipments | [default to 'outbound']
**carrier_id** | **str** | Carrier ID | 
**product_id** | **str** | Product ID from carrier | 
**services** | **List[str]** | List of selected services | 
**additional_parameters** | [**Dict[str, ListShippingRules200ResponseDataInnerAdditionalParametersValue]**](ListShippingRules200ResponseDataInnerAdditionalParametersValue.md) | Carrier-specific extra parameters, keyed by the carrier parameter &#x60;key&#x60; from the product&#39;s &#x60;additionalParameters[].key&#x60;. | 
**address_id** | **str** | Sender address ID | 
**receiving_countries** | **List[str]** | List of supported country codes | 
**email_notification** | **bool** | Send email notification to recipient | [default to False]
**phone_notification** | **bool** | Send SMS notification to recipient | [default to False]
**min_weight** | **float** | Minimum required weight in kg. Orders below this are excluded from the rule. | 
**max_weight** | **float** | Maximum allowed weight in kg. Orders exceeding this are excluded from the rule. | 
**min_order_value** | **float** | Minimum required order value in currency units. Orders below this are excluded from the rule. | 
**max_order_value** | **float** | Maximum allowed order value in currency units. Orders exceeding this are excluded from the rule. | 
**conditions** | [**List[ListShippingRules200ResponseDataInnerConditionsInner]**](ListShippingRules200ResponseDataInnerConditionsInner.md) | Rule conditions (weight/price/quantity) | 
**generate_proforma_invoice** | **bool** | Generate proforma invoice for shipments | [default to False]
**generate_commercial_invoice** | **bool** | Generate commercial invoice for international shipments | [default to False]
**generate_packing_list** | **bool** | Generate packing slip with package and item details | [default to False]
**auto_print_labels** | **bool** | Automatically print labels when shipment is sent | [default to False]
**auto_print_documents** | **bool** | Automatically print documents when shipment is sent | [default to False]
**label_printer_id** | **str** | ID of the label printer | 
**document_printer_id** | **str** | ID of the document printer | 
**return_shipping_rule_id** | **str** | ID of the return shipping rule | 
**auto_create_return_shipment** | **bool** | Automatically create and send a return shipment on dispatch | [default to False]
**org_id** | **str** | Owning organization ID | 
**brand_id** | **str** | Brand this record belongs to, or null when it is organization-wide | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 
**carrier** | [**ListShippingRules200ResponseDataInnerCarrier**](ListShippingRules200ResponseDataInnerCarrier.md) |  | 
**address** | [**ListAddresses200ResponseDataInner**](ListAddresses200ResponseDataInner.md) |  | 
**label_printer** | [**ListShippingRules200ResponseDataInnerLabelPrinter**](ListShippingRules200ResponseDataInnerLabelPrinter.md) |  | [optional] 
**document_printer** | [**ListShippingRules200ResponseDataInnerLabelPrinter**](ListShippingRules200ResponseDataInnerLabelPrinter.md) |  | [optional] 
**return_shipping_rule** | [**ListShippingRules200ResponseDataInnerReturnShippingRule**](ListShippingRules200ResponseDataInnerReturnShippingRule.md) |  | [optional] 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner import ListShippingRules200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInner from a JSON string
list_shipping_rules200_response_data_inner_instance = ListShippingRules200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInner.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_dict = list_shipping_rules200_response_data_inner_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInner from a dict
list_shipping_rules200_response_data_inner_from_dict = ListShippingRules200ResponseDataInner.from_dict(list_shipping_rules200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



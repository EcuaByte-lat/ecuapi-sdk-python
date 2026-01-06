# Invoice


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**organization_id** | **str** |  | 
**status** | **str** |  | 
**type** | **str** |  | 
**subtotal** | **float** |  | 
**tax_amount** | **float** |  | 
**total_amount** | **float** |  | 
**access_key** | **str** |  | 
**recipient_name** | **str** |  | 
**recipient_id** | **str** |  | 
**recipient_phone** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from ecuapi.models.invoice import Invoice

# TODO update the JSON string below
json = "{}"
# create an instance of Invoice from a JSON string
invoice_instance = Invoice.from_json(json)
# print the JSON string representation of the object
print(Invoice.to_json())

# convert the object into a dict
invoice_dict = invoice_instance.to_dict()
# create an instance of Invoice from a dict
invoice_from_dict = Invoice.from_dict(invoice_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



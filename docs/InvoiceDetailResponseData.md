# InvoiceDetailResponseData


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
**items** | **List[object]** |  | 

## Example

```python
from ecuapi.models.invoice_detail_response_data import InvoiceDetailResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceDetailResponseData from a JSON string
invoice_detail_response_data_instance = InvoiceDetailResponseData.from_json(json)
# print the JSON string representation of the object
print(InvoiceDetailResponseData.to_json())

# convert the object into a dict
invoice_detail_response_data_dict = invoice_detail_response_data_instance.to_dict()
# create an instance of InvoiceDetailResponseData from a dict
invoice_detail_response_data_from_dict = InvoiceDetailResponseData.from_dict(invoice_detail_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



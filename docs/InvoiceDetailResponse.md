# InvoiceDetailResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**InvoiceDetailResponseData**](InvoiceDetailResponseData.md) |  | 
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from ecuapi.models.invoice_detail_response import InvoiceDetailResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceDetailResponse from a JSON string
invoice_detail_response_instance = InvoiceDetailResponse.from_json(json)
# print the JSON string representation of the object
print(InvoiceDetailResponse.to_json())

# convert the object into a dict
invoice_detail_response_dict = invoice_detail_response_instance.to_dict()
# create an instance of InvoiceDetailResponse from a dict
invoice_detail_response_from_dict = InvoiceDetailResponse.from_dict(invoice_detail_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



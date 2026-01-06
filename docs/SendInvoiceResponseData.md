# SendInvoiceResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**access_key** | **str** |  | 
**status** | **str** |  | 
**sri_response** | **object** |  | [optional] 

## Example

```python
from ecuapi.models.send_invoice_response_data import SendInvoiceResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of SendInvoiceResponseData from a JSON string
send_invoice_response_data_instance = SendInvoiceResponseData.from_json(json)
# print the JSON string representation of the object
print(SendInvoiceResponseData.to_json())

# convert the object into a dict
send_invoice_response_data_dict = send_invoice_response_data_instance.to_dict()
# create an instance of SendInvoiceResponseData from a dict
send_invoice_response_data_from_dict = SendInvoiceResponseData.from_dict(send_invoice_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



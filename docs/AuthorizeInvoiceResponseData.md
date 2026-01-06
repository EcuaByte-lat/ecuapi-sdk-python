# AuthorizeInvoiceResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**status** | **str** |  | 
**sri_response** | **object** |  | [optional] 

## Example

```python
from ecuapi.models.authorize_invoice_response_data import AuthorizeInvoiceResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of AuthorizeInvoiceResponseData from a JSON string
authorize_invoice_response_data_instance = AuthorizeInvoiceResponseData.from_json(json)
# print the JSON string representation of the object
print(AuthorizeInvoiceResponseData.to_json())

# convert the object into a dict
authorize_invoice_response_data_dict = authorize_invoice_response_data_instance.to_dict()
# create an instance of AuthorizeInvoiceResponseData from a dict
authorize_invoice_response_data_from_dict = AuthorizeInvoiceResponseData.from_dict(authorize_invoice_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



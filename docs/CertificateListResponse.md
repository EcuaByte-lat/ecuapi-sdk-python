# CertificateListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Certificate]**](Certificate.md) |  | 
**meta** | [**CertificateUploadResponseMeta**](CertificateUploadResponseMeta.md) |  | 

## Example

```python
from ecuapi.models.certificate_list_response import CertificateListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateListResponse from a JSON string
certificate_list_response_instance = CertificateListResponse.from_json(json)
# print the JSON string representation of the object
print(CertificateListResponse.to_json())

# convert the object into a dict
certificate_list_response_dict = certificate_list_response_instance.to_dict()
# create an instance of CertificateListResponse from a dict
certificate_list_response_from_dict = CertificateListResponse.from_dict(certificate_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



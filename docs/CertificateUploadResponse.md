# CertificateUploadResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CertificateUploadResponseData**](CertificateUploadResponseData.md) |  | 
**meta** | [**CertificateUploadResponseMeta**](CertificateUploadResponseMeta.md) |  | 

## Example

```python
from ecuapi.models.certificate_upload_response import CertificateUploadResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateUploadResponse from a JSON string
certificate_upload_response_instance = CertificateUploadResponse.from_json(json)
# print the JSON string representation of the object
print(CertificateUploadResponse.to_json())

# convert the object into a dict
certificate_upload_response_dict = certificate_upload_response_instance.to_dict()
# create an instance of CertificateUploadResponse from a dict
certificate_upload_response_from_dict = CertificateUploadResponse.from_dict(certificate_upload_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



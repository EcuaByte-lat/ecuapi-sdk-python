# CertificateUploadResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**expires_at** | **str** |  | 
**subject** | **str** |  | 

## Example

```python
from ecuapi.models.certificate_upload_response_data import CertificateUploadResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateUploadResponseData from a JSON string
certificate_upload_response_data_instance = CertificateUploadResponseData.from_json(json)
# print the JSON string representation of the object
print(CertificateUploadResponseData.to_json())

# convert the object into a dict
certificate_upload_response_data_dict = certificate_upload_response_data_instance.to_dict()
# create an instance of CertificateUploadResponseData from a dict
certificate_upload_response_data_from_dict = CertificateUploadResponseData.from_dict(certificate_upload_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



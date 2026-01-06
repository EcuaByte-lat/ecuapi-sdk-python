# HealthResponseChecks


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**api** | **str** |  | 
**database** | **str** |  | 
**storage** | **str** |  | 

## Example

```python
from ecuapi.models.health_response_checks import HealthResponseChecks

# TODO update the JSON string below
json = "{}"
# create an instance of HealthResponseChecks from a JSON string
health_response_checks_instance = HealthResponseChecks.from_json(json)
# print the JSON string representation of the object
print(HealthResponseChecks.to_json())

# convert the object into a dict
health_response_checks_dict = health_response_checks_instance.to_dict()
# create an instance of HealthResponseChecks from a dict
health_response_checks_from_dict = HealthResponseChecks.from_dict(health_response_checks_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



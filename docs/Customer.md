# Customer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | RUC, Cédula, or Passport | 
**id_type** | **str** |  | 
**name** | **str** |  | 
**email** | **str** |  | [optional] 
**address** | **str** |  | [optional] 
**phone** | **str** |  | [optional] 

## Example

```python
from ecuapi.models.customer import Customer

# TODO update the JSON string below
json = "{}"
# create an instance of Customer from a JSON string
customer_instance = Customer.from_json(json)
# print the JSON string representation of the object
print(Customer.to_json())

# convert the object into a dict
customer_dict = customer_instance.to_dict()
# create an instance of Customer from a dict
customer_from_dict = Customer.from_dict(customer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



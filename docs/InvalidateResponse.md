# InvalidateResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | Success message | 

## Example

```python
from blackman_client.models.invalidate_response import InvalidateResponse

# TODO update the JSON string below
json = "{}"
# create an instance of InvalidateResponse from a JSON string
invalidate_response_instance = InvalidateResponse.from_json(json)
# print the JSON string representation of the object
print(InvalidateResponse.to_json())

# convert the object into a dict
invalidate_response_dict = invalidate_response_instance.to_dict()
# create an instance of InvalidateResponse from a dict
invalidate_response_from_dict = InvalidateResponse.from_dict(invalidate_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



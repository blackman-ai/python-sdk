# CompletionOptions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**max_tokens** | **int** |  | [optional] 
**stop** | **List[str]** |  | [optional] 
**stream** | **bool** |  | [optional] 
**temperature** | **float** |  | [optional] 
**top_p** | **float** |  | [optional] 

## Example

```python
from blackman_client.models.completion_options import CompletionOptions

# TODO update the JSON string below
json = "{}"
# create an instance of CompletionOptions from a JSON string
completion_options_instance = CompletionOptions.from_json(json)
# print the JSON string representation of the object
print(CompletionOptions.to_json())

# convert the object into a dict
completion_options_dict = completion_options_instance.to_dict()
# create an instance of CompletionOptions from a dict
completion_options_from_dict = CompletionOptions.from_dict(completion_options_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



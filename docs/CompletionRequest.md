# CompletionRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**max_tokens** | **int** |  | [optional] 
**stop** | **List[str]** |  | [optional] 
**stream** | **bool** |  | [optional] 
**temperature** | **float** |  | [optional] 
**top_p** | **float** |  | [optional] 
**messages** | [**List[Message]**](Message.md) |  | 
**metadata** | **object** | Optional metadata for tracking, analytics, and conditional processing. Can include session IDs, user context, feature flags, or any custom data. This metadata is logged with the request and can be used for filtering/analysis. | [optional] 
**model** | **str** |  | 
**provider** | [**Provider**](Provider.md) |  | 

## Example

```python
from blackman_client.models.completion_request import CompletionRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CompletionRequest from a JSON string
completion_request_instance = CompletionRequest.from_json(json)
# print the JSON string representation of the object
print(CompletionRequest.to_json())

# convert the object into a dict
completion_request_dict = completion_request_instance.to_dict()
# create an instance of CompletionRequest from a dict
completion_request_from_dict = CompletionRequest.from_dict(completion_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# SubmitFeedbackResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**message** | **str** |  | 

## Example

```python
from blackman_client.models.submit_feedback_response import SubmitFeedbackResponse

# TODO update the JSON string below
json = "{}"
# create an instance of SubmitFeedbackResponse from a JSON string
submit_feedback_response_instance = SubmitFeedbackResponse.from_json(json)
# print the JSON string representation of the object
print(SubmitFeedbackResponse.to_json())

# convert the object into a dict
submit_feedback_response_dict = submit_feedback_response_instance.to_dict()
# create an instance of SubmitFeedbackResponse from a dict
submit_feedback_response_from_dict = SubmitFeedbackResponse.from_dict(submit_feedback_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



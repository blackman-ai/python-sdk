# ImageUrl


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**detail** | **str** | Optional detail level: \&quot;auto\&quot;, \&quot;low\&quot;, or \&quot;high\&quot; | [optional] 
**url** | **str** |  | 

## Example

```python
from blackman_client.models.image_url import ImageUrl

# TODO update the JSON string below
json = "{}"
# create an instance of ImageUrl from a JSON string
image_url_instance = ImageUrl.from_json(json)
# print the JSON string representation of the object
print(ImageUrl.to_json())

# convert the object into a dict
image_url_dict = image_url_instance.to_dict()
# create an instance of ImageUrl from a dict
image_url_from_dict = ImageUrl.from_dict(image_url_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



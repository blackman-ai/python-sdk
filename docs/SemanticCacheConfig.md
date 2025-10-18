# SemanticCacheConfig


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Whether semantic caching is enabled | 
**similarity_threshold** | **float** | Similarity threshold for cache hits (0.0-1.0) | 
**ttl_seconds** | **int** | Time-to-live for cache entries in seconds | 

## Example

```python
from blackman_client.models.semantic_cache_config import SemanticCacheConfig

# TODO update the JSON string below
json = "{}"
# create an instance of SemanticCacheConfig from a JSON string
semantic_cache_config_instance = SemanticCacheConfig.from_json(json)
# print the JSON string representation of the object
print(SemanticCacheConfig.to_json())

# convert the object into a dict
semantic_cache_config_dict = semantic_cache_config_instance.to_dict()
# create an instance of SemanticCacheConfig from a dict
semantic_cache_config_from_dict = SemanticCacheConfig.from_dict(semantic_cache_config_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



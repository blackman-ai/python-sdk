# SemanticCacheStats


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**avg_similarity_score** | **float** | Average similarity score for cache hits | 
**cost_saved** | **float** | Total cost saved from cache hits | 
**hit_rate** | **float** | Cache hit rate as a percentage | 
**tokens_saved** | **int** | Total tokens saved from cache hits | 
**total_hits** | **int** | Total number of cache hits | 
**total_misses** | **int** | Total number of cache misses | 

## Example

```python
from blackman_client.models.semantic_cache_stats import SemanticCacheStats

# TODO update the JSON string below
json = "{}"
# create an instance of SemanticCacheStats from a JSON string
semantic_cache_stats_instance = SemanticCacheStats.from_json(json)
# print the JSON string representation of the object
print(SemanticCacheStats.to_json())

# convert the object into a dict
semantic_cache_stats_dict = semantic_cache_stats_instance.to_dict()
# create an instance of SemanticCacheStats from a dict
semantic_cache_stats_from_dict = SemanticCacheStats.from_dict(semantic_cache_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



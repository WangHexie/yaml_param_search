# yaml_param_search
***********************************
Yield all permutations of nested dictionary.    
Check out the template.

## install
```
pip install yaml-param-search
```
## usage
```python
from yaml_param_search import Config


config = Config("template", "search.yaml")
for i in config.yield_param():
    config.write_logs(i)
```

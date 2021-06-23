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
### output
```
{'param_name': 'option 1', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 1'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 1', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 1', 'value2 of option 1'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 1', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 2'}}
|||
{'param_name': 'option 2', 'param_name2': ['value1 of option 2', 'value2 of option 2'], 'param_name3': {'param_name3_1': 'option 2', 'param_name3_2': 'option 2'}}
|||
```
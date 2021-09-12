builtin modules

### builtin modules

e.g let say you want to stop your program execution for a few seconds, you may wanna for a sleep function. Where can you find it?

It doesn't exist on dir(__builtin_functions__)

We can look for that in other builtin modules, here is how

```python
import sys # system
sys.builtin_module_names # this will all builtin modules and inside that you need to find functions using dir(module_name)

# sleep method exists in time modules

import time
dir(time) # you will sleep function
help(time.sleep)
```
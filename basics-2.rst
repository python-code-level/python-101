# more python notes

code creation and modules

- code decomposition, code can be decomposed into smaller component parts to keep them easier to maintain,  
- modules is one option to deal with the need for code decomposition
- many modules are pre-supplied as part of the python standard library
- the way a module is imported changes the way functions can be used
- imports obs must occur before the first use of a moduel function
- namespace = where anmes are uniqe, have meaning and do not conflict with one another
- inside a namespace, all names are unique,
- elements enter the namespace when they are qualified (not just when they are imported)
- import math
- math.pi
- math.sin
- this makes it very clear where the entities come from, and also means it is possible to have multiple pi or sin in a code, they only enter namespace when qualified by their source module
- it is also possible to do a selective import, so only use certain entities from a module, but can cause problems with name conflicts. any new definitions with same names will override previously imported entity
- from math import pi, sin
- from math import *
- the above generic way of importing all entities in a module has several drawbacks. mainly it can be unclear what exactly has been imported, and this can cause problems or conflict with functions in the main codebase
- a further option allows whole module to be imported with an alias, can help make it clear of a source module if conflicts or similar to existing modules, or can shorten the fully qualified names
- import numpy as np
- import pandas as pd
- a further option allows selected entities to be imported froma module and also aliased at the same time, 
- from numpy import leastcost as myleastcost, time as thistime  etc
- once using aliases the original names become unavailable
- 
- 
- 








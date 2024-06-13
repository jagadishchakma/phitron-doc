

--- start-multi-column: ID_gpbi
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>
---
### Simple Import Export
- not necessary export
```python
# module1.py
language = "Python"

# module2.py
import module2
print(module2.language)

```

---
### Renamming Module
- "as" use for renaming
```python
# module1.py
language = "Python"

# module2.py
import module2 as mymodule
print(mymodule.language)
```

---
### Import From Another Folder
```python
import package.module.module1 as module1
from package.module.module1 import customFunction
```

---
### ==Not Have==
```python











```
--- column-break ---

# <p align="center">JavaScript</p>

---
### Simple Import Export
- must be add type="module" in package.json file
- or file extension rename "mjs"

```javascript
//module1.js
export let language = "JavaScript";

//module2.js
import {language} from './module1.js';
console.log(language);
```

---
### Renaming Module
- "as" use for renamming
```javascript
//module1.js
export let language = "JavaScript";

//module2.js
import {language as lang} from './module1.js';
console.log(lang);
```

---
### Import From Another Folder
```javascript
import {language} from "./package/module/module1.js"

```

---
### Default Export Import
```javascript
//module1.js
export let language = "JavaScript";
function myfunc(){
	console.log("Defualt Export Import");
}
export default myfunc;

//module2.js
import anyname, {language as lang} from './module1.js';
anyname();
console.log(lang);
```


--- end-multi-column


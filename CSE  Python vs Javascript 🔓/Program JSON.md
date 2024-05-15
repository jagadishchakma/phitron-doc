

--- start-multi-column: ID_d8jr
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>

---
### JSON Loads
```python

import json
person = '''{
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":28
}''';

data = json.loads(person)
```

---
### JSON Convert
```python
import json
person = {
		  "fname": "Jagaidish",
		  "lname": "Chakma",
		  "age": 28
}
jsn = json.dumps(person)
```
--- column-break ---

# <p align="center">JavaScript</p>

---
### JSON Loads
```javascript
let person = '
	{
	"fname":"Jagadish",
	"lname":"Chakma",
	"age":28
	}
'
data = JSON.parse(person)

```

---
### JSON Convert
```javascript
let person = {
	fname: "Jagadish",
	lname: "Chakma",
	age: 28
}
let jsn = JSON.stringify(person)

```
--- end-multi-column





--- start-multi-column: ID_wguo
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python Dictionary</p>

---
### ==dictionary== is object this have own properties and methods.
---
### Declare
```python
person = {
	"fname":"Jagadish",
	"lname":"Chakma",
	"age": 29,
	"city":"Rangamati"
	"Village":"Bodhipur"
}
```

---
### Constructor
```python
person = dict(name="jon", age=28, city="rangamati", village="bodhipur")







```
---
### Access  Item
```python
person["city"]


```

---
### Get Length
```python
len(person)
```

---
### Get Keys
```python
person.keys()
```

---
### Get Values
```python
person.values()
```

---
### Check If Key Exists
```python
if("city" in person):
	print("Yes have")
	
```

---
### Change Values
```python
person["age"] = 30 
```

---
### Adding Items
```python
person["study"] = "BBA"
```

---
### Remove Items
```python
person.pop("city")
person.popitem()
del person["city"]

```

---
### Looping 
```python
for item in person: #using in 
	print(person[item])


for key in person.keys(): #using keys(()
	print(person[key])


for value in person.values(): #using values()
	print(value)


for key,value in person.items(): #using items()
	print(key, value)

```

---
### Copy Dictionary
```python
newPerson = person.copy()

newPerson = dict(person)
```

---
### Nested Dictionary
```python
person= {
	"fname": "Jagadish",
	"lname": "Chakma",
	"more": {
		"fullName": "Jagadish Chakma"
	}
}
```

--- column-break ---

# <p align="center">JavaScript Object</p>

---
### ==object== is object this have own properties and methods.
---
### Declare
```javascript
let person = {
	fname: "Jagadish",
	lname: "Chakma",
	age: 29,
	city: "Rangamati",
	village: "Bodhipur"
}
```

---
### Constructor
```javascript
function Person(name, age, city, village){
	this.name = name;
	this.age = age;
	this.city = city;
	this.village = village;
}

let person = new Person("Jagadish Chakma", 28, "rangamati", "bodhipur")
```

---
### Access  Items
```javascript
person["city"]

person.city
```

---
### Get Length
```javascript
Object.keys(person).length
```

---
### Get Keys
```javascript
Object.keys(person)
```

---
### Get Values
```javascript
Object.values(person)
```

---
### Check If Key Exists
```javascript
if("city" in person){
	console.log("Yes Have")
}
```

---
### Change Values
```javascript
person["age"] = 29
```

---
### Adding Items
```javascript
person["study"] = "BBA"
```

---
### Remove Items
```javascript
delete person.city



```

---
### Looping
```javascript
for(let item in person){ //using in
	console.log(person[item])
}

for(let key of Object.keys(person)){ //using keys()
	console.log(person[key])
}

for(let value of Object.vlaues(person)){ //using values()
	console.log(value)
}

for(let [key, value] of Object.entries(person)){ //using entries()
	consloe.log(key, value);
}
```

---
### Copy Object
```javascript
let newPerson = Object.assign({},person);

let newPerson = {...person}
```

---
### Nested Object
```javascript
let person = {
	fname: "Jagadish",
	lname: "Chakma",
	more: {
		fullName: "Jagadish Chakma"
	}
}
```


--- end-multi-column



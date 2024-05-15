- JSON is a syntax fo storing and exchanging data.
- JSON is text, written with JavaScript Object Notation.
- # JSON in Python
- Python has a built-in package called ==json==, which can be used to work with JSON data.
```python
import json
```
- # Parse JSON -  Convert from JSON to Python
```python
import json
person = """
{
"fname":"Jagadsih"
"lname":"Chakma"
"age": 27
"city": "Rangamati"
}
"""
data = json.loads(person)
print(data)
```
- # Convert from Python to JSON
```python
import json
person = {
"fname":"Jagadsih"
"lname":"Chakma"
"age": 27
"city": "Rangamati"
}
parse = json.dumps(person)
print(parse)
```

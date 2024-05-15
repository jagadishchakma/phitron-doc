

--- start-multi-column: ID_t0r5
```column-settings
Number of Columns: 2
Largest Column: standard
```

# <p align="center">Python</p>

---
### Now Date
```python
import datetime

nowdate = datetime.datetime.now()
print(nowdate)
```

---
### Weekday
```python
weekday = nowdate.strftime("%a")
weekday = nowdate.strftime("%A")
weekday = nowdate.strftime("%w")
```

---
### Date
```python
date = nowdate.strftime("%d")
```

---
### Month
```python
month = nowdate.strftime("%b")
month = nowdate.strftime("%B")
month = nowdate.strftime("%m")
```

---
### Year
```python
year = nowdate.strftime("%y")
year = nowdate.strftime("%Y")
```

---
# Hours
```python
hours = nowdate.strftime("%H")
hours = nowdate.strftime("%I")
```

---
### Minutes
```python
minutes = nowdate.strftime("%M")
```

---
### Seconds
```python
seconds = nowdate.strftime("%S")
```

---
### Am/PM
```python
ampm = nowdate.strftime("%p")
```
--- column-break ---

# <p align="center">JavaScript</p>

---
### Now Date
```javascript


nowdate = new Date();
console.log(nowdate);
```

---
### Weekday
```javascript
weekday = nowdate.getDay();


```

---
### Date
```javascript
date = nowdate.getDate()
```

---
### Month
```javascript
month = nowdate.getMonth()


```

---
### Year
```javascript
year = nowdate.getFullYear()

```

---
### Hours
```javascript
hours = nowdate.getHours();

```

---
### Minutes
```javascript
minutes = nowdate.getMinutes()
```

---
### Seconds
```javascript
seconds = nowdate.getSeconds();
```

---
### ==Not Have==
```javascript


```
--- end-multi-column


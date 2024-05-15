- # Import
- Full package import
```python
import authentication
print(authentication.name)
```
- Specific function import
```python
from authentication import user
print(user.name)
```
- Rename
```python
import authentication as auth
from authentication import user as customer
```
- # Export
- Don't necessary export. Behind the scene python all package are export.

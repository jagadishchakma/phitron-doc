## Export
- named export
	- export a = 23;
	- export b = 34;
- defualt export
	- export default b;
## Import
- named import
	- import {a,b} from "__path";
- all import
	- import \* as name from "__path";
- defult import
	- import name, {a} from "__path";
## Key-Points
- Every single file can do only one defult exports
- Must be add a line in package.json file {"type":"module"}
# Key Points
- ## Garbage Collection:
	- JavaScript automatically collects unused data.
	- free and memory with the help of an algorithm called ==Mark-and-sweep==.
	- The garbage collector goes to the roots, marking(remembering) them on its way.
	- It then moves on the references and marks them as well.
	- The cycle continues until the garbage collector visits all the roots and references.
	- The garbage collector ==moves all the objects, except the marked ones==.
	- 
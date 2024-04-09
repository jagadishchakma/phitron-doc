# Introductions
- CSS allows animation in an HTML elements without using JavaScript of Flash.

# What are CSS Animations?
- An animation lets an element gradually change from one style to another.
- You can change as many CSS properties you want, as many times as you want.
- To use CSS animation, you must first specify some keyframes for the animation.
- Keyframes hold what styles the element will have at certain times.

# The @keyframes Rule
- When you specify CSS Styles inside the ==@keyframes== rule, the animation will gradually change from the current style to the new style at certain times.
- To get an animation to work, you must bind the animation to an element.
- 
# Properties
- ==@keyframes==
- ==animation-name==
- ==animation-duration==
- ==animation-delay==
- ==animation-iteration-count==
- ==animation-direction==
- ==animation-timing-function==
- ==animation-fill-mode==
- ==animation==

==Without @keyframes proerperty all properties declare in .hover element==

# ==@keyframes==
In animation code will be declare into the ==@keyframes== :
```css
@keyframes animation-name{
	from{}
	to{}
}
```
```css
@keyframes animation-name{
	0%{}
	25%{}
	50%{}
	75%{}
	100%{}
}
```


# ==animation-name==
Name of the animation element name:
```css
.div:hover{
	animation-name: example
}
```

# ==animation-duration==
Duration of the animation occuring:
```css
.div:hover{
	animation-duration: 4s(default value is 0s)
}
```

# ==animation-delay==
The ==animation-delay== property specifies a delay for the ==start== of an animation.
```css
.div:hover{
	animation-delay: 2s;
}
```

# ==animation-iteration-count==
The ==animation-iteration-count== properties specifies the number of times 
an animation should run:
```css
.div:hover{
	animation-iteration-count: 5, infinity
}
```
# ==animation-direction==
The ==animation-direction== property specifies whether an animation should be palyed forwards, backwards  or in alternate cycles.
```css
.div:hover{
	animation-direction: normal, reverse, alternate, alternate-reverse;
}
```
# ==animation-timing-function==
The ==animation-timing-function== property specifies the speed curve of the animation.
```css
.div:hover{
	animation-timing-function: ease, linear, ease-in, ease-out, ease-                                in-out;
}
```
# ==animation-fill-mode==
The ==animation-fill-mode== property specifies a style for the target element when the animation is not playing (before it starts, after it ends, or both)
```css
.div:hover{
	animation-fill-mode: none, forwards, backwards, both;
}
```

# ==animation== Shorthand
```css
.div:hover{
	animation: example 5s linear 2s infinity alternative;
}
```

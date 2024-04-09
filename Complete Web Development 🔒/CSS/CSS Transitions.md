# Introductions
CSS transitions allow you to change property vlaues smoothly, over a given duration.
==Always use transition proerty after event occuring==.
# Transitions Properties
- ==transition==
- ==transition-delay==
- ==transition-duration==
- ==transition-property==
- ==transition-timing-function==

# How  To Use CSS Transitions?
To create a transition effect, you must specify two things.
- The CSS property you want to add an effect to.
- The duration of the effect.
- ==**Note:** If the duration part is not specified, the transition will have no effect, because the default value is 0.

# ==transition== property
*property_name duration*,......,....,
```css
div:hover{
	width: 300px;
	height: 400px;
	transition: width 1s, hieght 3s;
}
```
# ==transition-delay== property
The ==transition-delay== property working on after how much time transitions will be start.
```css
div:hover{
	width: 400px;
	height: 400px;
	transition-delay: 4s;
	transition: width 1s, height 2s;
}
```
# ==transition-timing-function== property
The ==transition-timing-function== property specifies the speed curve of the transition effect.
- ==ease== = slow-fast-slow(defult)
- ==linear== = same speed
- ==ease-in== = slow to speed
- ==ease-out== = speed-slow
- ==ease-in-out== = slow-slow


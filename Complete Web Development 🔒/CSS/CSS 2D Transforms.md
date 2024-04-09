# Introduction
CSS Transforms allow you to move, rotate, scale, ans skew elements.

# 2D Transforms Method
- ==translate()==
- ==rotate()==
- ==scaleX()==
- ==scaleY()==
- ==scale()==
- ==skewX()==
- ==skewY()==
- ==skew()==
- ==matrix()==
# The ==translate()== Method
The ==translate()== method moves an element from its current position (according to the parameters given for the X-axis and Y-axis).
```css
div{
	transform: translate(x,y);
}
```
# The ==rotate()== Method
The ==rotate()== method rotates an element clockwise or counter-clockwise according to a given degree.
```css
div{
	transform: rotate(10deg);
}
```
Using negetive values will rotate the element counter-clockwise.
```css
div{
	transform: rotate(-40deg);
}
```
# The ==scale()== Method
The ==scale()== method increase or decrease the size of an element (according to the parameters given for the width and height).
Value ==1== is equal to current size of element.
Value ==below 1== is decrease of current size of element.
Value ==up 1== is increase of current size of element.
```css
div{
	transform: scale(0.5, 0.5);
	transform: scaleX(1.5);
	transform: scaleY(0.5);
}
```
# The ==skew()== Method
The ==skew()== method skews an element along the X and Y axis by the given angles. Like 3d painting.
```css
div{
	transform: skew(10deg, 20deg);
	transform: skewX(30deg);
	transform: skewY(20deg);
}
```
# The ==matrix()== Method
The ==matrix()== method combines all the 2D transforms method into one.
The ==matrix()== method take six parameters, containing mathematic functions, which allows you to rotate, scale, translate, skew elements.


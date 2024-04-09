# Introduction
- CSS gradients let you display smooth transitions between two or more specified colors.
- CSS defines three types of gradients:
	- Linear Gradients (goes down/up/left/right/diagonally)
	- Redial Gradients (defined by their center)
	- Conic Gradients (rotated around a center point)

# Linear Gradients
T create a linear gradient you must define at least two color stops. Color stops are the colors you want to render smooth transitions among. You can also set a starting point and direction (or an angle) along with the gradient effect.
###### syntax
```css
background-image: linear-gradient(direction, color-stop1, color-stop2...);
```

==Direction Top-Bottom== (this is default)
starts at the top to bottom
```css
background-image: linear-gradient(red,yellow);
```
==Direction Left-Right==
start at the left to right
```css
background-image: linear-gradient(to right, red,yellow);
```
==Direction Diagonal==
You can make a gradient diagonally by specifying both the horizontal and vertical starting position.
```css
background-image: linear-gradient(to bottom right, red , yellow);
```
==Using Angle==
If you want more control over the direction of the gradient, you can define and angle, instead of the predefined directions (to bottom, to top, to right, to left, to bottom right, etc). A value of 0deg is equivalent to "to top". 
```css
background-image: linear-gradient(90deg, red, yellow);
```
==Multiple colors==
```css
background-image: linear-gradient(to right, red, yellow, blue, green);
```
==Using Transparency==
CSS gradients also support transparency, which can be used to create fading effects.
To add transparency, we use the rgba() function to define the color stops. The last parameter of rgba can be a value from ==0 to 1==, and it defines the transparency of the color: ==0 indicates full transparency, 1 indicates full color (no transparency)== 

```css
background-image: linear-gradient(to right, rgba(255, 0, 0, 0), rgba(255, 0, 0, 0.8));
```


# Radial Gradients
- A radial gradient is defined by its center.
- To create a radial gradient you must also define at least two color stops.

###### Use of different size
- circle
- closest-side
- closest-corner
- farthest-corner
```css
background-image: radial-gradient(circle, red, yellow, black);
```

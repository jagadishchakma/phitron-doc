# Introduction
- With CSS you can add shadow to text and to elements.
- Two kinds of shadow:
	- ==tex-shadow==
	- ==box-shadow==
# ==tex-shadow== property
- The CSS ==text-shadow== property applies shadow to text.
- In its simples use, you only specify the ==horizontal== and ==vetical== shadow with ==blur== with ==color==.
```css
h1{
	text-shadow: 2px(horizontal) 2px(vertical) 3px(blur) red(color);
}
```
# ==box-shadow== property
- The CSS ==box-shadow== property is used to apply one or more shadows to an element.
- In it's simplest use, you only specify a ==horizontal== and a ==vertical== shadow with ==blur==  with ==color== . The default color of the shadow is the current text color.
```css
div{
	box-shadow: 4px 4px 1px red;
}
```
- The ==inset== parameter changes the shadow from an outer shadow (outset) to an inner shadow.
```css
div{
	box-shadow: 4px 4px 1px red inset;
}
```
- An element can also add ==multiple== shadows :
```css
div{
	box-shadow: 4px 4px 1px red, 3px 3px 1px green, 5px 5px 2px blue;
}
```

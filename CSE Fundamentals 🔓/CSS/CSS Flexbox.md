- The flexible box layout module, makes it easier to design flexible responsive layout structure without using float or positioning.
- ### Flex Container
```css
.flex-container{
	display: flex;
}
```
- ### Flex Direction
```css
.flex-container{
	display: flex;
	flex-direction: column,column-reverse,row,row-reverse;
}
```
- ### Flex Wrap
```css
.flex-container{
	display: flex;
	flex-wrap: wrap,nowrap,wrap-reverse;
}
```
- ### Justify Content
```css
.flex-container{
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: center,space-between,space-around,space-evenly, flex-start, flex-end;
}
```
- ### Align Items
```css
.flex-container{
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center, flex-start,flex-end, baseline,stretch;
}
```
- ### Order
```css
.flex-item1{
	order: 4;
}
```
- ### Flex Grow
```css
.flex-item1{
	flex-grow: 5;
}
```





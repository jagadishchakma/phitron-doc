# Introduction
Befor the flexbox layout module, there were four layout modes:
- Block, for sections in a web page.
- Inline, for text.
- Table, for two-dimensional  table data.
- Positioned, for explicit position of an element.
The flexible box layout module, makes it easier to design flexible responsive layout structure without using float or positioning.

# Flexbox Element
To start using the flexbox model, you need to first define a flex container.
The flex container becomes flexible by setting the ==display== property to ==flex==.
```css
.flex-container{
	display: flex;
}
```
# Flexbox Properties
- ==flex-direction==
- ==flex-wrap==
- ==flex-flow==
- ==justify-content==
- ==align-items==
- ==align-content==

# ==flex-direction==
The flex-direction property defines in which direction the container wants to stack the flex items.

==column== value stacks the flex items vertically (from top to bottom)
==column-reverse== value stack the flex items vertically (but bottom to top)
==row== value stack the flex items horizontally (from left to right)
==row-reverse== value stack the flex items horizontally (but right to left)


# ==flex-wrap==
The flex-wrap property specifies whether the flex items should wrap or not.
==wrap== value specifies that the flex items will wrap if necessary.
==nowrap== value spacifies that the flex items will not wrap (this is default)
==wrap-reverse== value specifies that the flexible items will wrap.


# ==flex-flow==
The flex-flow property is a shorthand property for setting both the flex-direction and flex-wrap properties.

==flex-flow== value of flex-direction and flex-wrap properties


# ==justify-content==
The justify-content property is used to align the flex items.
==center== value aligns the flex items at the center of the container
==flex-start== value aligns the flex items at the beginning of the container (this is default)
==flex-end== value aligns the flex items at the end of the container
==space-around== value displays the flex items with space before, between and after ther lines.
==space-between== value displays the flex items with space between the lines



# ==align-items== 
The align-items property is used to align the flex items.
==center== value aligns the flex items in the middle of the container 
==flex-start== value aligns the flex items at the top of the container
==flex-end== value aligns the flex items at the bottom of the container
==stretch==  value stretch the flex items to fill the container (this is default)
==baseline== value aligns the flex items such as their baselines aligns.


# ==align-content== 
The align-content property is used to align the flex line.
==space-between==
==space-around==
==stretch==
==center==
==flex-start==
==flex-end==

- CSS selectors selects the HTML element(s) you want to style.
- ### Types of Selectors
- Simple Selectors (select elements based on name,id,class,universal,grouping)
```css
h1{}
#id{}
.class{}
*{}
h1,h2,p{}
h1#id{}
p.class{}
```
- Combinator Selectors (select elements based on a specific relationship between them)
```css
ul li a{} /*descendant selector(space)*/
ul li>a{} /*child selector*/
ul+li{}
ul ~ li
```
- Pseudo-class Selectors (select elements based on a certain state)
- 
- Pseudo-element Selectors (select and style a part of an element)
- 
- Attribute Selectors (select elements based on an attribute or attribute value)
```css
input[type="radio"]{}
```



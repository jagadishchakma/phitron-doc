# Introduction
- The CSS ==object-fit== property is used to specify how an img or video should be resized to fit its container.
- This property tells the content to fill the container in a variety of ways; such as "preserve that aspect ratio" or "stretch up and take up as much space as possible".

# ==object-fit== property
- ==fill== = this is default. The image is resized to fill the given dimension.
- ==contain== = the image keeps its aspect ratio, but is resized to fit within the given dimension.
- ==cover== = image keeps its aspect ratio and fills the given dimension.
- ==none== = the image is not resized.
- ==scale-down== = none or conatin.

```css
img{
	width: 200px;
	height: 300px;
	object-fit: contain;
}
```

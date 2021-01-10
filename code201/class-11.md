 # Images:

Specifying image sizes helps pages to load more smoothly. Why? Because the HTML and CSS code will often load before the images. Telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download. 

Commonly used image sizes:
- Small portrait: 220 x 360
- Small landscape: 330 x 210
- Feature Photo: 620 x 400

### Aligning images:
Use the float property to move images to the right or left. You can use a class to effect multiple images at once. It is also a good idea to add a margin to your images. This ensures that the text does not touch the edges of the image. Ex: margin 10px

### Centering Images:
By default, images are inline elements. This means they flow within the surrounding text. In order to center an image , it should be turned into a block-level element using the display property with a value of block.
Ex: display: block;  
On the image itself you can use the margin property and set the values of the left and right margins to auto.
Ex: margin: 0px auto;

### Backround Images:
The backround- image property allows you to place an image behind any HTML element. This could be the entire page or just part of it. By default, a backround image will repeat itself to fill the the entire box. Backround images are often the last thing to load which makes seem slow to load. The larger the image, the longer it takes to download.
Ex: p {
backround-image: url ("examlpleimagepattern.gif);
}

### Repeating Images:
The backround-repeat property can have four values:
- repeat (the image is repeated horizontally and vertically. This is the default if you don't use a backround-repeat property). 
- repeat-x (the image is repeated horizontally only)
- repeat-y (the image is repeated vertically only)
- no-repeat (the image is only shown once)
The backround-attachment property specifies whether a backround image should stay in one position or move as the user scrolls up and down the page. It can have one of two values:
- fixed (the backroumd image stays in the same place on the page)
- scroll (the backround-imave moves up an down as the user scrolls up and down the page)

### Backround Position:
When an image is not being repeated, you can use this property to specify where in the browser window the backround image should be placed. The property usually has a set of values. The first represents the horizontal position and the second represents the vertical.
 Ex: left top
center bottom 
right center

You can also use a pair of pixels and percentages. These represent the distance from the top left corner of the browser window or containing box. The top left corner is equal to 0% 0%  To center the image vertically and horizontally is equal to 50% 50%  
The backround property acts as a shorthand for all of the properties listed above. 

### Image Rollover:
Rollover allows a link or button to change to a second style when the user mouses over it. You can add a third style when they click on it.
### Sprite:
When a single image is used for several different parts of an interface. The advantages of using sprites is that the web browser only needs to request one image rather then many images. This can make the page load faster. 


[<----Back to Home](../README.md)

# Images, Color and Text

## Images:  




Stock Photo sources:
- www.istockphoto.com
- www.gettyimages.com
- www.veer.com
- www.sxc.hu.com
- www.fotola.com

If you are building a website from scratch, it is a good idea to put all of your images in their own folder. It is better for organization and makes it easier to identify problems without threatening the rest of your project. 

You can also put folders within folders (eg. logos and buttons in "interface" or product photographs in "products").

1. Save images in the right format (eg. jpeg, gif or png). This results in better image quality.
1.  Save the image at the same height and width it will appear on the website (in pixels). This helps prevent image distortion and helps the image load faster on your page.

Tools to edit and save images:
- www.photoshop.com
- www.pixlr.com
- www.splashup.com
- www.ipiccy.com

_Flat Color_ : When a picture has an area that is filled with exactly the same color.

_Vector Images_:
line drawing(such as a logo, illistration or diagram). They are resolution independent. You can change the size witput effecting the quality. 

_Animated GIFs show several frames of an image in sequence. 

To include a photo with caption:
```
<figure>
  <img src="image.jpg" alt="photo of _____"/>
  <br/>
  <figcaption>image caption</figcaption>
</figure>
```

## Colors:

Ways to specify colors:

- RGB Values 
-These express colors in terms of how much red, green and blue are used in the photo.  
For example: rgb(100,100,9)  

- Hex Codes-They also express the amount of red, green and blue.   For example: #ee3e80

- Color Names-predefined color names that are recognized by browsers. For example: DarkCyan

- HSLA-This starts with the letters hs1 followed by individual values for hue, saturation and brightness.
Example: hs1(0, 100%, 78%)

If you do not specify a backround color then the backround is transparent! (often the web browser defaults to white).

## Text


```
 @font-face {


}
 ```
 
 This command allows you to use a font that is not installed on your computer.

 www.fontsquirrel.com/fontface/generator
 
This site provides you with the CSS code for the @front-face-rule.

_Leading_ ("ledding"): the vertical space between lines of text.

_Kerning_: the space inbetween the letters.

### Styling Links:


Use this psuedo class to set styling for links that have not been visited yet:
```
:link
```
Use this one to set styles for links that have already been clicked on (eg. changing the color of the link so users can tell what links they have already clicked on):
```
:visited
```

Attribute Selectors:
- Existence
- Equality
- Space
- Prefix
- Substring
- Suffix
   


[<-----Back to about me ](../README.md)




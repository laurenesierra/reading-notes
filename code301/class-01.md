# Shay Howe’s Intro to RWD
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.

Media features identify what attributes or properties will be targeted within the media query expression.

The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

__Flexible Media:__


One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

http://learn.shayhowe.com/advanced-html-css/responsive-web-design/

# All About Floats
Collapsing almost always needs to be dealt with to prevent strange layout and cross-browser problems. We fix it by clearing the float after the floated elements in the container but before the close of the container.

__Problems with Floats:__

Floats often get beat on for being fragile. The majority of this fragility comes from IE 6 and the slew of float-related bugs it has.
If you need text wrapping around images, there really aren’t any alternatives for float. Speaking of which, check out this rather clever technique for wrapping text around irregular shapes. But for page layout, there definitely are choices. Eric Sol right here on A List Apart has an article on Faux Absolute Positioning, which is a very interesting technique that in many ways combines the flexibility of floats with the strength of absolute positioning. CSS3 has the Template Layout Module that, when widely adopted, will prove to be the page layout technique of choice.

https://css-tricks.com/all-about-floats/


# Don’t Overthink It Grids
The vast majority of websites out there use a grid. They may not explicitly have a grid system in place, but if they have a “main content area” floated to the left a “sidebar” floated to the right, it’s a simple grid.

A block level element is as wide as the parent it’s inside (width: auto;). We can think of it as 100% wide. 

https://css-tricks.com/dont-overthink-it-grids/

# CSS Floats Explained By Riding An Escalator
Floats create alternate flows. This is the hardest part to understand. And once you introduce them, you then need to write your code so that it accounts for up to three flows: normal, left and right. This is a whole new set of rules, as opposed to manipulating the width of elements or their positioning.

If you had one line of people standing in the middle of the elevator, you would have limited options for new structures. But when you have a left and right column, suddenly you can specify that certain people stand on the right, other ones stay left, and another group can fill in the gaps.
This allows you to create more readable and understandable code, because the float property also gives an indication of an element’s relationship to surrounding elements.


The Clear Property:


 _Clear_ allows elements to specify where they should align in comparison to the floated elements.


https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/


## SMACCS Official Documentation:
http://smacss.com/

[<----Back Home](../README.md)
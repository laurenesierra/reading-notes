
# What Google Learned From It's Quest to Build the Perfect Team

(Charles Duhigg)

//////////////////////////////////////////////////////////////////////////////////


Why do some groups thrive and others falter?


Today, on corporate campuses and within university laboratories, psychologists, sociologists and statisticians are devoting themselves to studying everything from team composition to email patterns in order to figure out how to make employees into faster, better and more productive versions of themselves.

 ‘‘We’re living through a golden age of understanding personal productivity,’’ says Marshall Van Alstyne, a professor at Boston University who studies how people share information. ‘‘All of a sudden, we can pick apart the small choices that all of us make, decisions most of us don’t even notice, and figure out why some people are so much more effective than everyone else.’’


 Studies show that teams tend to:
 - innovate faster
 - see mistakes more quickly 
 - find better solutions to problems
 - achieve better results
 - higher job satisfaction

 If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.

Building the best teams means combining the right people.

Understanding and influencing group norms is the key to improving teams.

 The thing that distinguishes the good teams from the dysfunctional teams is:
 - how teammates treat one another
 - good conversational skills; everyone gets a chance to talk
 - social sensitivity; being aware of how others feel based on things like their tone of voice and facial experssions
 - having clear goals
 - creating a culture of dependability
 
 Create a group that has an enviroment of psycological safety.


‘‘I might be the luckiest individual on earth,’’ Sakaguchi (a mid-level manager at Google) told me.
‘‘I’m not really an engineer. I didn’t study computers in college. Everyone who works for me is much smarter than I am.’’ But he is talented at managing technical workers, and as a result, Sakaguchi has thrived at Google. 

Human bonds matter as much at work as anywhere else.

‘‘I think, until the off-site, I had separated things in my head into work life and life life,’’ Laurent told me. ‘‘But the thing is, my work is my life. I spend the majority of my time working. Most of my friends I know through work. If I can’t be open and honest at work, then I’m not really living, am I?’’

 No one wants to put on a ‘‘work face’’ when they get to the office. No one wants to leave part of their personality and inner life at home. We want to know that work is more then just "labor".

  ‘‘By putting things like empathy and sensitivity into charts and data reports, it makes them easier to talk about,’’ Sakaguchi told me. ‘‘It’s easier to talk about our feelings when we can point to a number...Why would I walk away from (work)? Why wouldn’t I spend time with people who care about me?’’

Everything is different now, data reigns supreme, today’s winners deserve to triumph because they are cleareyed enough to discard yesterday’s conventional wisdoms and search out the disruptive and the new.

In the best teams, members listen to one another and show sensitivity to feelings and needs.

It’s sometimes easy to forget that success is often built on experiences — like emotional interactions and complicated conversations and discussions of who we want to be and how our teammates make us feel.

# CSS Transforms


It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

The transform property comes in two different settings, _two-dimensional_ _and three-dimensional_. Each of these come with their own individual properties and values.


Working with two-dimensional transforms we are able to alter elements on the horizontal and vertical axes (x, y), however there is another axis along which we can transform elements. Using three-dimensional transforms we can change elements on the z axis, giving us control of depth (z) as well as length and width (x, y).

[CSS Transformations](https://learn.shayhowe.com/advanced-html-css/css-transforms/)


# Transitions and Animations

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transformations:

As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the:
- :hover
- :focus
- :active &
- :target 

pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.


### Animations:

Animations pick up where transistions leave off.

[CSS Transformations and Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

# 8 Simple CSS Transitions That Will Wow Your Users
(Sara Viera)
///////////////////////////////////////////////////////

CSS3 has introduced countless possibilities for UX designers, and the best thing about them is that the coolest parts are really simple to implement.

Just a couple of lines of code will give you an awesome transition effect that will excite your users, increase engagement and ultimately, when used well, increase your conversions.

### 1. Fade in
Having things fade in is a fairly common request from clients. It’s a great way to emphasize functionality or draw attention to a call to action.

Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover.

```
.fade {
  opacity:0.5;
}
.fade:hover
{
  opacity:1;
}
```
Make sure you set the class of your div to _fade_.

### 2. Change color
Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS.
```
.color:hover
{
  backround:#53a7ea;
}
```
### 3. Grow & Shrink
To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.

Set your div’s class to “grow” and then add this code to your style block:
```
.grow:hover
{
  -webkit-transform: scale(1.3);
  -ms-transform: scale(1.3);
  transform: scale(1.3);
}
```

Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1:
```
.shrink:hover
{
  -webkit-transform: scale(0.8);
  -ms-transform: scale(0.8);
  transform: scale(0.8);
}
```
### 4. Rotate elements
CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element. Give your div the class “rotate” and add the following to your CSS:
```
.rotate:hover
{
  -webkit-transform: rotateZ(-30deg);
  -ms-transform: rotateZ(-30deg);
  transform: rotateZ(-30deg);
}
```
### 5. Square to circle
A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.

Give your div the class “circle” and add this CSS to your styles:
```
.circle:hover
{
  border-radius:50%
}
```

### 6. 3D shadow
3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.

This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.

Give your div the class “threed” and then add the following code to your CSS:
```
.threed:hover
{
  box-shadow:
  1px 1px #53a7ea,
  2px 2px #53a7ea,
  3px 3px #53a7ea,
  -webkit-transform: translateX(-3px);
  transform: translateX(-3px);
}
```
# 7. Swing
Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration.

In this case, we’ll first define a CSS animation in your styles. You’ll notice that due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes (yes, Internet Explorer really is better than Chrome, in this respect at least).
```
@-webkit-keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
       transform: translateX(-5px);
    } 
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
@keyframes swing
{
    15%
    {
        -webkit-transform: translateX(5px);
        transform: translateX(5px);
    }
    30%
    {
        -webkit-transform: translateX(-5px);
        transform: translateX(-5px);
    }
    50%
    {
        -webkit-transform: translateX(3px);
        transform: translateX(3px);
    }
    65%
    {
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
    }
    80%
    {
        -webkit-transform: translateX(2px);
        transform: translateX(2px);
    }
    100%
    {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }
}
```
This animation simply moves the element left and right, now all we need to do is apply it:
```
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}
```

8. Inset border
One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.

Give your div the class “border” and add the following CSS to your styles:
```
.border:hover
{
  box-shadow: inset 0 0 0 25px #53a7ea;
}
```

[8 Simple CSS Transitions That Will Wow Your Users](http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

[6 Buttons Animated](https://codepen.io/retyui/pen/ByoaXV)

[CSS Animations: Keyframes](https://codepen.io/akshaychauhan/pen/oAfae)

[404](https://codepen.io/kieranfivestars/pen/MYdQxX)

[Pure CSS Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv)


////////////////////////////////////////////////////////////////////////////////////
[<-----Back to Home](README.md)
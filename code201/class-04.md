# Links

```
<a href= "example.https.com">the text people see and click on. explan where the link takes you</a>

```
These are absolute URLs.


You can also link to other pages within the same site:
```
<p>
  <ul>
    <li>Home</li>
    <li>About</li>
    <li>Contact</li>
  </ul>
</p>

```
These are relative URLs.

Pro tip! With large websites it is best to put the pages for each section of your site in different folders. Folders on a website are referred to as _directories_.

Email links:
```
<a href="mailto:soandso@example.com">Email So and So</a>
```
 You can also link to a specific part of the another page.

 # Layout

 Containing Elements:

 If one block-level element sits inside another block-level element, the outer box is known as the "parent" or "containing" element.

 You can control the positing of elements on your page with "CSS postioning schemes".
 - Normal flow
 - Relative positioning
 - Absolute postioning
     - Fixed Postioning (a form of absolute posioting)
 - floating elements

 When you have things that overlap, the _z-index_ property allows you to control which box overlaps the other.

When programing, keep in mind: screen size and screen resolution.
Developers often create pages of around 960-1000 pixels wide. 


Fixed Width Layouts:

These do not change sizes when the browser window changes size.


Liquid Layouts:
 

 These designs stretch and change as the user increases or decreases browser window.

 Layout Grids:

 Compisition = the placement or arrangement of visual elements-how they are organized on the page.

 Using a grid structure can be helpful to keep things organized.

 CSS frameworks provide rules for common tasks. This allows you to use build on preset CSS rather then building from scratch. 


 # Functions, Methods and Objects

 Functions:
 These consist of a series of statements thast have been grouped together to perform a specific task.

 Objects:
 Programers use these to create models of the world using data. They are made up of properties and methods.

 Built-In Objects:
The browser comes with a set of objects that act as a toolkit for creating interactive web pages.


Variable Scope:

- Local Variables (these are created inside the function using the _var_ keyword. It can only be used in the function)
- Global Variables (If you create a variable outside a function, then it can be used anywhere within the script.)

Global variables use more memeory as the browser has to remeber them as long as the web page using them is loaded. Local variables are only remembered during the period of time the function is being executed.

In an object, variables and functions take on new names:
- Object = property 
- Function = method

_Literal Notaion_ is the best way to create objects.

You can access the properties or methods of an object using _Dot Notation_ or square brackets [ ].

# Pair Programing

__Pair programming touches on four skills:__ 
- developers explain out loud what the code should do
 - listen to others’ guidance
- read code that others have written 
- write code themselves.

While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

### __Benefits__:
- when two people focus on the same code base, it is easier to catch mistakes in the making
-  the experience is more engaging and both programmers are more focused than if they were working alone
- working with a teammate can expose developers to techniques they otherwise would not have thought of
- The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.
- It improves communication and social skills
- ! Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome. !
- It makes coding enjoyable!


[<---- Back to About Me](../README.md)
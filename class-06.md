# Functions, Methods and Objects

_Functions_ let you group a series of statements together to perform a specific task.  If different parts of a script repeat the same task, reuse the function (think smarter, not harder!).

_Objects_ group together a set of variables and functions to create a model of something you would recognize from the real world. In an object variables and functions take on new names.

Storing data:
In Javascript, datais represented using name/value pairs.  To organize your data you can use an array or object to group together a set of related values.  In arrays and objects the name is also known as a key.

_Arrays_ are actually a special type of object.  They hold a related set of key/value pairs (like all objects) but the key for each value is it's _index number_.

 Each character in a string is automatically given an _index number_. _Index numbers always start at zero and not one (just like for items in an array).

 In Javascript there are six data types.

 Simple or primitive data types:

 - String
 - Number
 - Boolean
 - Undefined (a variable that has been declared but no value has been assgned yet)
 - Null (a variable with no value)

#### Complex data types:

 - Object

 Arrays and functions are considered types of objects.  They can be used to create complex data sets (and both can contain the other).

 # Document Object Model (DOM)

 The DOM specifies how browsers should create a model of an HTML page and how Javascript can access and update the contents of a web page while it is in the browser window.  When the browser loads a page it creates a model of the page in memory. The DOM specifies the way in which the browser should structure this content using a _DOM Tree_.  A DOM Tree consists of four main types of nodes:
 - Document Node
 - Element Nodes
 - Attribute Nodes
 - Text Nodes

 Each node is an object with methods and properties.  
 An element node is can contain several multiple text nodes and child elements that are siblings of each other.

 The DOM is called an object model because the model (DOM Tree) is made of objects.

 DOM Queries: Methods that find the elements in the DOM Tree.

 ```
 getEelementById() and querySelector()
```
These methods can search an entire document and return individual elements.

You can select element nodes by their id or class attributes, by tag name or CSS syntax.

When a DOM method can return more then one element, it returns a _Nodelist_.  A _Nodelist_ is acollection of element nodes. Each node is given an index number starting at zero.

When you have a Nodelist, you can loop through each node in the collection and apply the same statements to each.

_Traversing the DOM_: When you have an element node, you can select another element in relation to it using these five properties.
- parentNode
- previousSibling
- nextSibling
- firstChild
- lastChild


Adding or removing content from DOM tree:

- innerHTML property (better for updating entire fragments)
- DOM manipulation (easily targets individual nodes)

Once you have an element node, you can use other properties and methods on that element node to access and change it's attributes.




[<---- Back to home](README.md)


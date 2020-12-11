# Forms

_Forms_ allow you to collect information from vistors on your site.

Ex: Google search bar

### Form Contols

Form controls add information.  
Adding text:
- Text imuput (single-line)
- Password imput
- Text area (multi-line)

Making choices:
- Radio buttons
- Checkboxes
- Drop-down boxes

Submitting forms:
- Submit Buttons
- Image Buttons

Uploading files:
- File Upload


Never change a form control unless you know that the code on the server will understand this new value.

Form Structure...
```
<form action="http://example"
  method="get">
  <p>This is where the controls will appear<p>
</form>
```
The _form element_ contains the value for the page on the server that will be receiving the info that is entered from the user.


Forms can be sent using one of two methods:

- get

This will get the values from the form and add them to the end of the URL specified in the _action_ attribute. Use this for short forms or when you are just retrieving data from the web server.


- post

This will post (or send) the values in the HTTP header. Use this when you want the user to be able to upload a file, addeds or deletes info from data base, contains sensitive data or for long forms.

### Text Input ("user input" text bar):

```
<form action="http://example">
  <p>Username:
    <input type="text" name="username" size="15" 
    maxlength="30px" />
  <p>
</form>
```
The attribute _maxlength_ allows you to limit the amount of characters a user can enter into the text field.

The proccess up above will vary for other kinds of input (eg. password).

Form validation:
A message that tells the user they have filled out the form incorrectly.

Information collected form a form is sent in name/value pairs.


# Lists, Tables and Forms

You can use the _list-style-type_ elememt to control the shape or style of bullet points:

```
ul {
  list-style-type
}
```

You can also use:
- list-style-image (to have an image act as the bullet point)
- list-style-position: outside or inside (this lets you control whether the bullets sit inside or outside the text box)

The _curser_ property allows you to control the type of mouse curser that will be displayed on your page.

Make sure you style your forms in a way that lets the user know it is interactive.

# Events 

when you browse the web, your browser registers different types of events. This is the browser's way of letting you know something happened. Your script can then respond to these events.

- Interactions create events
(When users hover, click, type, etc.)
- Events trigger code (functions)
- Code responds to users
(The events trigger changes the DOM is capable of)

Event handling:

_Event handling_ is how Javascript triggers code.


It is comprised of 3 steps:

1. Select the element node(s) you want the script to respond to.
1. Indicate which event on the selected node(s) will trigger the response
1. Start the code you want to run when the event occurs


_Event handlers_ let you indicate which event you are waiting for on any particular event.  

There are 3 types of event handlers:

- HTML Event Handlers
- Traditional DOM Event Handlers
- Dom Level 2 Event Listeners

You can only attach one function to each event handler.

_Event listeners_ can deal with more then one function at a time but they are supported in older browsers.

You can't use parentheses after the function name in event handlers and listeners. _Parameters_ are used instead of parentheses.

### Event Flow

HTML elements nest inside other elements. If you hover or click on something you will also be hovering or clicking on it's parent elements.

Event Bubbling: The event starts at themost specific node and flows outwards towards the least specific one. This is the default type of event flow with very wide browser support.

Event Capturing: The event starts at the least specific node and flows inwards to the most specific one (This is not supported in older browsers).

The flow of events only really matters when your code has event handlers on an element and one of it's ancestor or descendant elements.

The Event Object:
When an event occures, the event object tells you info about the event, and the element it happed upon.

Event Delegation:
This allows you to delegate the job of _event listener_ to a parent of the elements.

When you call a function, the event object's target property is the best way to find out which element an event occured on.



Focus and Blur Events:


The HML elements you can interact with (ex. links or forms) can gain focus.  These events fire when they gain or lose focus.

Mouse Events:


These events are fired when the mouse is moved and also when it's buttons are clicked.



Tip! The _event_ object can tell you where the curser was positioned when an event was triggered.


Keyboard Events:

These events are fired when a user interacts with the keyboard.  They will fire on any device with a keyboard.

Form Events:

- submit
- change
- input

Mutation Events and Observers:

Whenever elements are added to or removed from the DOM, it's structure changes which triggers a mutaion event.

HTML 5 Events:

3 Examples:

- DOMContentLoaded
- hashChange
- beforeunload



_Binding_ is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 


__The most commonly used events are W3C DOM events, although there are others in the HTML5 specification as well as browser-specfic events.__









[<----Back to Home](README.md)
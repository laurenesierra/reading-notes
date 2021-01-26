# Sending Form Data

### Defining how to send data:

The ``` <form> ``` element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

### The action attribute:

The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.

### The method attribute:
The method attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method.

### The get method:
The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource.

### The post method:
The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

### Viewing HTTP requests:
HTTP requests are never displayed to the user (if you want to see them, you need to use tools such as the Firefox Network Monitor or the Chrome Developer Tools). As an example, your form data will be shown as follows in the Chrome Network tab. After submitting the form:

1. Open the developer tools.
1. Select "Network"
1. Select "All"
1. Select "foo.com" in the "Name" tab
1. Select "Headers"


...You can then get the form data.

## Sending Files

Sending files with HTML forms is a special case. Files are binary data — or considered as such — whereas all other data is text data. Because HTTP is a text protocol, there are special requirements for handling binary data.

### The encrypte attributte:
This attribute lets you specify the value of the Content-Type HTTP header included in the request generated when the form is submitted. This header is very important because it tells the server what kind of data is being sent. By default, its value is application/x-www-form-urlencoded. In human terms, this means: "This is form data that has been encoded into URL parameters."
If you want to send files, you need to take three extra steps:

1. Set the method attribute to POST because file content can't be put inside URL parameters.
1. Set the value of enctype to multipart/form-data because the data will be split into multiple parts, one for each file plus one for the text data included in the form body (if text is also entered into the form).
1. Include one or more <input type="file"> controls to allow your users to select the file(s) that will be uploaded.

## Be paranoid

So, how do you fight these threats? This is a topic far beyond this guide, but there are a few rules to keep in mind. The most important rule is: never ever trust your users, including yourself; even a trusted user could have been hijacked.

All data that comes to your server must be checked and sanitized. Always. No exception.

[Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

[HTML5 Forms Reference ](https://htmlreference.io/forms/)


[<----Back Home](../README.md)
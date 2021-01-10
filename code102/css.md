# Intro to CSS
##### HTML and CSS by Jon Ducket

- CSS allows you to create rules that specify how the content of an element should appear. 

-The key is to remember that there is an invisible box around every HTML element.
-CSS allows you to create rules that control the way each individual box (and the elements inside the box) is presented.

Styling Note: Simple is better. Some of the most beautiful websites out there have a simplistic design.

CSS works by associating rules with HTML elements.

A CSS rule contains two parts: a _selector_ and a _declaration_.

- Selectors indicate which element the rule should be applied to.
- Declarations in dicate how the elements refered to int hte selector should be styled.

CSS Declarations  are made up of a _property_ and a _value_. The declaration sit between curly brackets{}.

- Properties indicate the aspects of the element you want to change.
- Values specify the settings you want to apply to the chosen properties.
 
 eg:
 body {font - family: Arial, Verdana, sans-serif;}

 __External CSS__

 Include the link (<>)  element inside the head. This shows others where to find the CSS file used to style the page.

 It should use three attributes. 

 - href (specifies path to CSS file)
 - type (specifies the type of document being linked to)
 _- rel (specifies the relationship between the HTML page and the file it is linked to)

 This method aloows you to edit one line of code and it will apply to all your pages. (It is also much neater)

__Internal CSS__
 Use the style elemant (<>) to include your CSS within the head element. 

 Note: If you have one page that you want to add more rules or styling you might consider using CSS in the same flie as your HTML. Over all it is a better practice to use an external file.

 __CSS selectors__
 These allow you to target rules to specific elements in an HTML document.

 Before you launch your website, veiw it in different browsers so you can see what the page looks like.
 - BrowserCam.com
 - BrowserLab.Adobe.com
 - BrowserShots.org
 - CrossBrowserTesting.com

 When CSS does not display as expected it is generally refered to as a _browser quirk_ or _CSS bug_.

 You can use these sites to find a solution.
 - PostionIsEverything.net
 - QuirksMode.org

 #### Chapter 11

 __Color!__

 You can specify color in one of three ways.

 - RGB Values
 - Hex Codes
 - Color Names

 Color picking tools:
 - Photoshop
 -  GIMP
 - colorschemesdisigner.com

 When picking colors it is impertant to think about contrast. Readabilty is key.

CSS3 allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

 HSLA allows you to specify color properties using hue, saturation and lightness.

 CSS3 has an extra value for RGB colors to indicate opacity. It is known as HSLA.

 Color not only brings life to your site but also helps convey the mood and evokes reactions. 




 [<----](../README.md)



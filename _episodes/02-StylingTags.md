---
title: Styling and Tags
teaching: 10
exercises: 10
questions:
- "How apply styles to my text?"
- "How can I insert an image?"
- "How can we define further properties through a tag?"
objectives:
- "Insert and image and resize it"
- "Add in more text and apply styles for emphasis"
keypoints:
- "It gets tiring doing it all by hand and is why we will use CSS."
---

In our webpage so far we have simply added text and made it bold, or regular. However we can do more to style the text, and insert images, but this requires understanding tags.

## Tags

~~~
<!DOCTYPE html>
   <html>
   <head>
       <title>Welcome to my Webpage!</title>
   </head>
   <body>
       <p><b>My first Webpage</b></p>
       <p>Some text explaining the webpage<p>
   </body>
   </html>
~~~
{: .language-html}

In our worked example, we added a new paragraph of text, and made it regular text. This was achieved through the use of ```Tags```.


Tags all look the same, where the tag type is within angled brackets. For example ```<head>```.

If the type of tag can contain children elements, then the tag needs to be closed. In the case of ```<head>```, the closing tag is ```</head>```.

All tags that require being closed as closed in the same manner, with a forward slash at the start of the tag type name within the angled brackets.

Tags inform the browser how to interpret the text within.

```<head>``` is where we define the metadata of the webpage. This information is not rendered on the page, but is where we define styles we use, reference template html for our webpage to use, etc.

Within the ```<head>``` we have to define the ```<title>``` which informs search engines and the browser of the title of the webpage. This is not rendered in the browser, but does appear in the tab of our browser.

The ```<body>``` tag wraps around the elements that will be rendered in our webpage. This is images, text, tables, lists, etc.

Some tags do not need closing as they do not have children elements. Images are an example of this.

~~~
<!DOCTYPE html>
   <html>
   <head>
        <title>Welcome to my Webpage!</title>
   </head>
   <body>
        <img src="images/logo.jpg">
        <p><b>My first Webpage</b></p>
        <p>Some text explaining the webpage<p>
   </body>
   </html>
~~~
{: .language-html}

Notice that within the ```<img>``` tag we have define an ```attribute```. In this case the relative location of the image file with respect to the html file we are editing.




{% include links.md %}

---
title: Tags
teaching: 10
exercises: 10
questions:
- "Semantic and Non-semantic tags"
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


## Non-Semantic Elements

Some tags are ```non-semantic``` in nature. They have some default styles, but they are simply tags that have no other meaning when intepreted by the browser, but we can assocatiate to them styles through CSS. These tags
do not tell us anything about the content that they wrap around.

Here are some non-semantic tags that have some default styles

- ```<strong>``` similar to bold
- ```<i>``` italics
- ```<em>``` emphasis
- ```<mark>``` highlight the background of the text
- ```<small>``` shrinks the text
- ```<strike>``` strike through
- ```<u>``` underline
- ```<del>``` deleted
- ```<ins>``` inserted
- ```<sub>``` subscript
- ```<sup>``` superscript
- ```<div>```
- ```<span>```

Many tag attributes for styling are now unused due to the implentation of CSS.

Before HTML5, a non-semantic tag could have its purpose defined by defining a class and associating it to a tag through the class attribute.

~~~
<div class="header>Some Text</div>
~~~
{: .language-html}

## Semantics

In HTML5, ```semantic``` tags inform the browser how to interpret the content within, primarily informing the browser about the structure of the document, the the type of cotent. Tags can be semantic in nature, 
informing the broweser about the purpose of the code - in this case informing the browser
about structure and heirarchy of the content in the page, and if the content is text, and image, or a table. The browser will give default styles to content within tags, but these styles can be altered through CSS.

```<head>``` is where we define the metadata of the webpage. This information is not rendered on the page, but is where we define styles we use, reference template html for our webpage to use, etc.

Within the ```<head>``` we have to define the ```<title>``` which informs search engines and the browser of the title of the webpage. This is not rendered in the browser, but does appear in the tab of our browser.

The ```<body>``` tag wraps around the elements that will be rendered in our webpage. This is images, text, tables, lists, etc.

The ```<footer>``` tag is used to place credits and copyright information within the webpage. There can be mulitple footers, places after different sections within the body.

Some tags do not need closing as they do not have children elements. Images are an example of this.

A benefit of semantic tags is that they also improve the readability of the code.

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

Notice that within the ```<img>``` tag we have define an ```attribute```. In this case the relative location of the image file with respect to the html file we are editing. In the case of images, we can modify the width and and height using further attributes.


> ## Modify the height and width of an image?
>
> What happens if the height or width only is given as an attribute?
>
> How does this differ it the image is an svg file?
>
> > ## Solution 
> > ~~~
> > <!DOCTYPE html>
> >  <html>
> >  <head>
> >        <title>Welcome to my Webpage!</title>
> >   </head>
> >   <body>
> >        <img src="images/logo.jpg" height="100px">
> >        <p><b>My first Webpage</b></p>
> >        <p>Some text explaining the webpage<p>
> >   </body>
> >   </html>
> > ~~~
> > {: .language-html}
> > 
> > Modifying just the height or the width means the image is altered but the other attribute changes to retain the image ratios.
> >
> > Modifying both indepently causes an image to be distorted unless it is a svg.
> {: .solution}

We will look at the use of semantic tags later for structuring our HTML document.


{% include links.md %}

---
title: Rendering Lists
teaching: 10
exercises: 10
questions:
- "How can render lists?"
objectives:
- "Render an unordered list"
- "Render an ordered list"
- "Render a list with definitions"
keypoints:
- "Lists are have a few main routes to styling depending on the information you are trying to convey."
---

There are times where we want to present information as a list.

Our two main encapsulating tags are;

- ```<ul>``` unordered list
- ```<ol>``` ordered list

Within the tagged section, list items are wrapped by the ```<li>``` tag.

> ## Can you two lists, one ordered, the other ordered?
>
>
> > ## Solution 
> > ~~~
> >    <!DOCTYPE html>
> >    <html>
> >    <head>
> >        <title>Welcome to my Webpage!</title>
> >    </head>
> >    <body>
> >        <p><b>My first Webpage</b></p>
> >        <p>Some text explaining the webpage<p>
> >        <p><a href="https://www.leighton.com/">Link to Leighton</a></p>
> >        <ul>
> >               <li>Dog</li>
> >               <li>Cat</li>
> >               <li>Fish</li>
> >        </ul>
> >        <ol>
> >               <li>Dog</li>
> >               <li>Cat</li>
> >               <li>Fish</li>
> >        </ol>
> >    </body>
> >    </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}
>


{% include links.md %}

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

A definition list is styled so that there is a list of items, but under each item there is a definition. This would work well for
rendering a glossary.

The tags used for this is ```<dl>```, and an item is wrapped by the ```<dt>``` tag, and the definition is then wrapped by the tag ```<dd>```.

> ## Can you make a definition list for the subatomic particles that make up atoms; protons, electrons, and neutrons?
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
> >        <dl>
> >               <dt>Proton</dt>
> >               <dd>Positively charged subatomic particle.
> >               <dt>Neutron</dt>
> >               <dd>Neutrally charged subatomic particle.
> >               <dt>Electron</dt>
> >               <dd>Negatively charged subatomic particle.
> >        </dl>
> >    </body>
> >    </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}
>

{% include links.md %}

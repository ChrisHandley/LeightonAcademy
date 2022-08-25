---
title: Tables
teaching: 10
exercises: 10
questions:
- "How can display data in a table?"
objectives:
- "Render a table"
keypoints:
- "Not sure yet"
---

If we are not rendering text as paragraphs or as lists, then we are rendering tables.

A table is wrapped by the ```<table>``` tag, and within the bounds of that tag, we define the structure of the table.

A table consists of rows and columns, and within the table element we define the table in a nested manner, first the rows, and then
the columns within the row.

The tag, ```<tr>```, wraps all the contents of the row. This is our ```table row```.

Within a row, we define columns, using the ```<td>``` tag. Each entry, in each column, is the ```table data```.

> ## Can you make a table, that has in one column first names, the second column contains last names, and the third column contains age?
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
> >        <table>
> >             <tr>
> >                 <td>Chris</td>
> >                 <td>Handley</td>
> >                 <td>39</td>
> >             </tr>
> >             <tr>
> >                 <td>Jake</td>
> >                 <td>Trent</td>
> >                 <td>34</td>
> >             </tr>
> >             <tr>
> >                 <td>Sue</td>
> >                 <td>Lloyd</td>
> >                 <td>27</td>
> >             </tr>
> >               
> >        </table>
> >    </body>
> >    </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}
>

We can easily define the headings of the table, using the ```<th>``` tag for our row entries, rather than ```<td>```.

Further styling can be applied to the table by separating the rows into blocks. We can wrap our main table data in ```<tbody>```, while a table title
can be added using ```<thead>```. Similarly ```<tfoot>``` adds a table row to the bottom of the table.

Using the ```<caption>``` keyword we can also add a caption to the table.

Right now our table has no lines between entries. Using the ```<table>``` attribute ```frame="box"``` adds a box aroudn the entire table, while the attribute ```border``` allows us to define the boaders around
the entries.

Using these tags is important when it comes to further styling using CSS, and we will find that table styling is more easily managed using CSS.

{% include links.md %}

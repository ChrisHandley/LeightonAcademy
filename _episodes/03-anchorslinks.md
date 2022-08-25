---
title: Hyperlinking and Anchors
teaching: 10
exercises: 10
questions:
- "How to we link to other pages?"
- "How can we link to other places in the same page?"
- "How can we download a file that is linked?"
- "How can we link to emails?"
objectives:
- "Set up our login manager."
- "Access a database using python."
keypoints:
- "Python has many database libraries and queries are done using neat python syntax rather than SQL."
---

## Anchors?
The ```<a>``` tag defines an ```anchor``` element. The ```href``` attribute defines the ```hyperlink``` to a resource, such as a webpage, files, email addresses, or even locations within the same webpage.

The general structure of the anchor is as follows;

~~~
<a href="some address">Some text that is the hyperlink text</a>
~~~
{: .language-html}


> ## Can you create a hyperlink to Leighton.com?
>
> Can you create a hyperlin in your webpage?
> Can you make an image a link?
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
> >    </body>
> >    </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}
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
> >        <p><a href="https://www.leighton.com/"><img src="images/logo.svg"/></a></p>
> >    </body>
> >    </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}

Adding a hypertext link that opens your email client is just as easy

~~~
<a href=mailto:christopher.handley@leighton.com>Email Me!</a>
~~~
{: .language-html}

## Hyperlinks to Destinations on the Same Page?

We said that the anchor tag can create hyperlinks to allow us to jump to another point in the page.

To demonstrate this we need to start using tags to create structure in the document, and to identify sections.

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
        <h2>Section 1</h2>
        <p>Lorem Ipsum....</p>
        <h2>Section 2</h2>
        <p>Lorem Ipsum....</p>
   </body>
   </html>
~~~
{: .language-html}

We are using the ```<h2>``` tag to define a section heading.

By typing ```Lorem``` and then letting it auto complete by pressing tab, VS Code injects in the entire boilerplate text or Lorem Ipsum.

By doing the same but for example, typing a number after Lorem, eg ```Lorem50``` it will auto fill with text, repating the passage, until 50 words are injected.

With the text injected, it makes the hyperlinking meaningful, as we jump past sections of text.

We need to add in an attribute to each of our headings for our sections, using the ```id``` attribute. For example ```id="section_01"```.

To create a link to this section heading, using an anchor, you reference the section id.

~~~
<a href="#section_03">Jump to section 3</a>
~~~
{: .language-html}




> ## Can you create a hyperlink to a third section of text, where sections 1 and 2 have 300 words, and section 3 has 50?
>
> Can you create a hyperlin in your webpage?
> Can you make an image a link?
>
> > ## Solution 
> > ~~~
> > <!DOCTYPE html>
> > <html>
> >   <head>
> >     <title>Welcome to my Webpage!</title>
> >   </head>
> >   <body>
> >     <p><b>My first Webpage</b></p>
> >     <p><ins>Hello hello</ins></p>
> >     <img src="images/Chris.jpg" width="100px" style="float: left" />
> >     <a href="mailto:christopher.handley@leighton.com">Email Me!</a>
> >     <a href="#section_3">Jump!</a>
> >     <h2 id="section_1">Section 1</h2>
> >     <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sit quia saepe
      quam illo magni laborum est recusandae adipisci, dolor quaerat totam earum
      libero quas error voluptatum maiores sapiente odit quis eius perspiciatis?
      Iste, culpa, impedit natus inventore consectetur exercitationem vitae ipsa
      cupiditate similique enim assumenda adipisci optio earum at sint? Culpa
      voluptates expedita dolorum eius atque a obcaecati laudantium, nostrum
      magni nam excepturi eaque, ea in vitae rem ducimus ut facilis! Dolores
      voluptate doloremque nam quos modi tempora hic animi harum, ex voluptatum
      excepturi facilis facere quibusdam recusandae eveniet ratione neque
      distinctio quas suscipit aperiam sed iste similique in! Eaque molestias
      ipsum veniam delectus distinctio provident quidem pariatur recusandae ut
      aut est accusamus incidunt quos officia, expedita saepe vel ad, dicta iste
      amet alias minus! Sapiente quos est provident quo dicta? Perferendis
      doloremque vel aperiam placeat voluptatem quae nemo fugit! Animi sed
      voluptas laboriosam nulla voluptatibus illo dicta, praesentium dolore
      minus ipsam ab eos quis atque nam accusantium impedit sit perferendis
      commodi dolorum. Perferendis ea voluptatum, quas ipsum est natus iste esse
      quibusdam unde iure, ipsam quod quae. Voluptates, magnam? Dolores minus
      consequuntur aspernatur maxime facilis aut aliquam beatae fugiat nam
      recusandae vitae eos consequatur quas veritatis accusantium, odit libero,
      unde, suscipit officia expedita error? Quos debitis officiis rem eius, non
      facere, nostrum temporibus asperiores ullam, numquam doloremque! Iusto
      corrupti, doloribus deserunt dolorem tenetur voluptatem asperiores iste
      aliquid molestiae blanditiis eaque eius provident eligendi vitae
      perspiciatis in nisi culpa tempore nam laudantium fugit cum nobis sint
      ipsa. Iste sint beatae iure id neque a autem magnam eius ab tempora ex
      excepturi ullam placeat in accusamus doloremque repellat modi quia natus
      perferendis cumque, quibusdam voluptatem! Illum odit qui laudantium
      debitis tenetur voluptatibus atque esse omnis ut totam vero aperiam a
      accusantium, repellendus deserunt quibusdam corrupti, quasi quia eius
      eligendi soluta est?
> >     </p>
> >     <h2 id="section_2">Section 2</h2>
> >     <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione
      consequuntur reprehenderit obcaecati eaque quas consectetur temporibus
      dignissimos reiciendis! Doloremque nam possimus cumque hic saepe. Quasi
      harum ratione nisi in autem nesciunt similique qui illo suscipit nemo enim
      placeat excepturi provident perspiciatis, culpa nobis quam tempora
      possimus aspernatur facilis saepe ea cupiditate cumque. Aut, magnam vero
      facere facilis aperiam natus minima nemo nulla, incidunt officia nobis
      veritatis omnis fugit quos ex ipsa doloremque voluptas maiores sit, beatae
      perspiciatis quidem? Doloremque sit recusandae, quibusdam reprehenderit
      illo distinctio rem necessitatibus, quas ea adipisci aut cupiditate,
      quisquam aliquam non. Quos reprehenderit dolorum repudiandae corporis
      porro ipsa, distinctio necessitatibus nesciunt velit sapiente vero
      molestiae tempora minima magnam beatae similique? Natus esse optio qui
      asperiores voluptas inventore itaque laboriosam blanditiis repellendus
      mollitia, officiis explicabo deleniti aspernatur voluptate quasi hic ipsam
      recusandae, eveniet rem maxime? Sint blanditiis hic officia ipsam
      aspernatur consequuntur at magnam eum, autem vero? Dignissimos deserunt
      aut odit fuga quidem ipsa! In, doloribus aliquam? Consequatur placeat sit
      ipsa, sequi eaque beatae rem quos aperiam dolores enim rerum porro dolor
      impedit quisquam animi ut iusto, voluptatem facere dolorem explicabo
      consectetur soluta. Voluptatem nisi saepe dolorum accusantium unde velit,
      aut quo aperiam reiciendis perspiciatis quisquam aspernatur consectetur
      omnis, fugit nam tenetur rerum quae architecto nostrum odio doloribus
      totam numquam! Aut ipsa impedit, corrupti ex cumque in cupiditate velit
      veritatis beatae dolorem quis, eum dolor doloribus distinctio odit!
      Sapiente debitis delectus vero quisquam facilis labore ipsum tempore et
      modi, accusamus dolorem temporibus, animi quis facere quia? Nostrum cum
      perspiciatis dolores repellendus, autem voluptatem nulla! Omnis dolor cum
      id assumenda voluptas in officiis aperiam perspiciatis doloremque rem
      quibusdam totam expedita nihil, fuga non ipsa illum, repellat obcaecati
      dicta dolore maiores recusandae error ut? Voluptate, repudiandae impedit!
      Aperiam dolor molestiae et cum quas a illum libero, non ullam
      perspiciatis.
> >     </p>
> >     <h2 id="section_3">Section 3</h2>
> >     <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Quae architecto
      cum repudiandae dignissimos magnam eum placeat facilis. Natus quas itaque
      ducimus aperiam odit suscipit officiis a blanditiis vero deserunt error
      voluptatem quos ut fugiat ipsam nobis voluptate impedit id cumque, libero
      temporibus. Fugit dolorem et illum, cupiditate quod laboriosam alias.
> >     </p>
> >   </body>
> > </html>
> > ~~~
> > {: .language-html}
> > 
> {: .solution}

We will go into more detail about headings tags in a later lesson.


{% include links.md %}

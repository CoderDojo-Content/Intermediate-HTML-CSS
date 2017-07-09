1. Up until now you've used heading and paragraph tags for arranging your **content** so that it looks tidy and is easy to read. Let's look at some tags that you can use to group things together.
 * **Content** is all the "stuff" on your web page, like information and pictures
2. Go to the attractions.html file (or one of your own pages if you're not using the example Trinket project). Near the top, just _underneath_ the opening `<main>` tag, type the following on a new line: 
 ```
  <main>
   <article>
 ```
Delete the closing tag that Trinket automatically adds in for you.
3. At the bottom of the file, just _above_ the closing `</main>` tag, add a new line and close the `article` element:
 ```
   </article>
  </main>
 ```
4. Think of `article` element as a **container** for a piece of content, in this case a set of information about attractions in my home country, Ireland. If you have different bits of content that aren't related, you should put each one into its own `article` element instead of putting one set of the tags around the whole lot.
5. Now look at the content: can you break it up into chunks or sections? Another HTML element called `section` lets you do exactly this! Let's put the information about each different attraction in between its own set of `<section> </section>` tags. Here's two examples:
 ```
  <section>
    <h2>The Cliffs of Moher</h2>
    <p>
     The Cliffs of Moher are found in County Clare, where I am from. They are well worth a visit - look how cool they are!
    </p>
    <img src="cliffs.JPG" alt="The Cliffs of Moher" height="200px">
   </section>
   
  <section>
    <h2>Achill Island</h2>
    <p>
      This is a large island off the coast of County Mayo. It has a wild and
      beautiful landscape of mountains, bogs and cliffs.
    </p>
    <img src="achill.JPG" width="200px">
  </section>
 ```
6. Confused about this container thing? Remember when you created a menu and then put it in between `<nav> </nav>` tags. That's another example of one of these containers. What you are doing is telling the browser that everything in between these special tags belongs together. Like organising things in boxes and shelves in your home!
7. Once your content has been organised into `articles` and `sections` you can create CSS rules in the stylesheet to control how the different bits look! Here's an example of some CSS styling of the `article` and `section` containers. See if you can understand it and then make some of your own.
 ```
  section {
    border-top-style: solid;
    border-top-width: 2px;
    border-top-color: #F5FFFA;
    padding-bottom: 10px;
 }
 
 article {
    border-radius: 10px;
    background-color: #48D1CC;
    padding: 10px;
 }
```
8. Have a go at organising all of your HTML files in this way. If you get stuck, check out [***TODO*** dojo.soy/organised-html](https://trinket.io/html/3b6fa2e6ba?runMode=run) for an example!
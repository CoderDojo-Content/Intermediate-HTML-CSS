1. You can make your website more **interactive** by making cool stuff happen when you hover over things with the mouse! In styles.css, find the CSS rules for the class `.solidRoundBorders` and add a new block of rules right underneath: ......MAYBE ADD TO SECTION TAG INSTEAD??
  ```  
    .solidRoundBorders {
      border-style: solid;
      border-width: 2px;
      border-color: #F5FFFA;
      border-radius: 10px;
    }
    .solidRoundBorders:hover {
      border-style: dotted;
      border-width: 3px;
      border-color: #9900CC;
    }
  ```  
Check index.html and other html files to see what elements are using the `solidRoundBorders` class. Or add the class to some elements, such as an image. Then run the code and move the mouse over those elements to see what happens!
2. You've just used a special type of CSS block called a **pseudo-class**. The `:hover` bit is the **pseudo-class**. It's a bit like a class, but it comes built in so you don't need to add it to anything in your HTML code. All you need to do to use it is to create `:hover` style rules in your CSS file for whatever elements you want to use it on.
 * You can use the `:hover` pseudo-class with any selector in CSS: class selectors as above, or ID selectors (for example `#myCoolText:hover`, or element selectors (for example `img:hover`)
5. Let's use this new `:hover` **pseudo-class** together with a CSS class to make links glow when you hover over them! Add a link to your web page and include an attribute to specify the class name.  
  ```<a class="nice-links" href="http://www.failteireland.ie/">Irish Tourism website</a>
  ```
  * Remember links are defined using the `a` tag
6. Now add the following code to your stylesheet and then run your code to see your lovely links in action.
  ```
    .nice-links {
      text-decoration: none;
      color: Brown;
    }
    .nice-links:hover {
      color: purple;
      background-color: PapayaWhip;
      border-radius: 10px;
    }
  ```
 * Why not add the attribute `class="nice-links"` to all of the links in your menu bar as well? This will make your menu bar even more interactive!
7. You can combine all of these tricks with animations too! 
8. Add the following animation to your CSS file:
  ```
    @keyframes glow-pulse {
      0% {
        border-style: solid;
        border-width: 10px;
        border-color: papayawhip;
      }
      50% {
        border-style: solid;
        border-width: 10px;
        border-color: pink;
      }
      100% {
        border-style: solid;
        border-width: 10px;
        border-color: papayawhip;
      }
    }
  ```
9. In your `.nice-links:hover` block, add three more CSS rules:
  ```
    animation-name: glow-pulse;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  ```
10. Now your link should have a glowing border that appears to pulse on and off whenever you hover the mouse over it!


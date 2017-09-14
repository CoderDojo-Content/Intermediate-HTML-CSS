1. You can make your website more **interactive** by making cool stuff happen when you hover over things with the mouse! Find your CSS rules for the **img** elements, or create some if you don't have any. Add in a border, and then add a new block of rules right underneath:
  ```css
    img {
      border-radius: 30px;
      border: 2px solid White;
    }
    img:hover {
      border: 2px dashed Navy;
    }
  ```
  You've just used a special type of CSS block called a **pseudo-class**. The `:hover` bit is the **pseudo-class**. It's a bit like a **class**, but it comes built in: you can add `:hover` style rules to any **element**, **class** or **id** selector in your stylesheet without needing to add anything extra in your HTML code.

2. What do you think will happen? Check what pages on your website have pictures on them \(add a picture if there aren't any!\), then run your code and move the mouse over a picture to find out!

3. Let's use this new `:hover` **pseudo-class** together with a **CSS class** to make links glow when you hover over them! Add a link to your web page and include an **attribute** to specify the **class** name. Remember, links are defined using the **a** tag.
  ```html
      <p>
        Visit the <a class="niceLinks" href="https://en.wikipedia.org/wiki/Ireland">Wikipedia page</a> to learn even more about Ireland!
      </p>
  ```

4. Add the following code to your stylesheet, then run your code to see your lovely links in action.
  ```css
    .niceLinks {
      text-decoration: none;
      color: magenta;
    }
    .niceLinks:hover {
      color: deepskyblue;
    }
  ```

  Why not add the **attribute** `class="nice-links"` to all of the links in your menu bar as well?

5. You can combine all of these tricks with animations too! Add the following animation to your CSS file:
  ```css
    @keyframes glowPulse {
      0% {
        color: deepskyblue;
      }
      50% {
        color: lightgreen;
      }
      100% {
        color: deepskyblue;
      }
    }
  ```
6. In your `.nice-links:hover` block, add three more CSS rules:
  ```css
    animation-name: glowPulse;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  ```
  Now your link should have a glowing border that appears to pulse on and off whenever you hover the mouse over it!

7. For your final trick, you will teach Tito to roll over! First, give the picture of Tito an **id** of _imgTito_ \(if you are working with your own project you can use any picture\).
  ```html
    <img id="imgTito" src="tito.png" alt="Tito the dog" width="100px">  
  ```

8. Then add the following animation to your stylesheet file:
  ```css
    #imgTito {
      border-radius: 100%;
    }
    #imgTito:hover {
      animation: rollOver 1s 1;
    }
    @keyframes rollOver {
      0% {
        transform: rotate(0deg);
      }
      100% {
        transform: rotate(360deg);
      }
    }
  ```

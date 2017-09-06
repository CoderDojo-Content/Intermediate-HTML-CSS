1. Go to your stylesheet file and add the following. Be sure to include the dot in front!

   ```
          .purpleBackground {
              background-color: #9f80ff;
          }
   ```

   The dot makes this into a **class** selector. With a CSS **class** you can apply the same set of CSS rules to any element on your website by adding an **attribute** to the element.

2. Now go to attractions.html and add the following **attribute** to the `<article>` tag:

   ```
        <article class="purpleBackground">
   ```

   You should see the green background disappear from around the text on the Attractions page. Next you're going to make each section on that page have the green background instead!

3. Add the following class to your stylesheet:

   ```
        .greenBackground {
            background-color: #48D1CC;
        }
   ```

   Back in the attractions.html file, add the attribute `class="greenBackground"` to each of the section tags, just like you did for the `article` element. Click Run and look at the Attractions page. Compare it to the other pages that have `section` elements.

4. You can add more than one class to an element. Let's make another CSS class to give the sections some margin and padding. In styles.css, add the following code:
   ```
        .sectionSpacing {
          padding: 10px;
          margin-top: 20px;
        }
   ```
5. In attractions.html, add the new class to each of the sections. Simply put a space after the first class name, and type the new name inside the quotation marks, like this:

   ```
        <section class="greenBackground sectionSpacing">
   ```

   * You can add as many CSS classes to an element as you like. Just write the names of all the classes you want to use inside the `class` attribute, and separate them with spaces.

6. How about re-vamping the Food page? Add the following classes to your stylesheet:

   ```
        .yellowBackground {
          background-color: #FFFFCC;
          color: #A52A2A;
        }

        .solidRoundBorders {
          border-style: solid;
          border-width: 2px;
          border-color: #F5FFFA;
          border-radius: 10px;
        }
   ```

   In the food.html file, add the new classes as well as the `.sectionSpacing` class to each section:

   ```
        <section class="yellowBackground sectionSpacing solidRoundBorders">
   ```

   * Notice how you can mix and match the classes in your element attributes?

7. Using CSS classes lets you **reuse** the same set of style rules on lots of elements. You can apply them to any element that has the properties you've set. Go to index.html and add the `.solidRoundBorders` class to the picture of Tito.

   ```
        <img id="imgTito" class="solidRoundBorders" src="tito.png" alt="Tito the dog" width="100px">
   ```

8. Why not experiment with some more CSS classes to make each page on your website have a different theme? You can name a CSS class anything you like. It's common to give it a name that describes what it does or what it's for!




1. Let's design a theme for the Attractions page that's different from the homepage. Go to your stylesheet file and add the following. Be sure to include the dot in front!
   ```css
          .purpleBackground {
              background-color: #9f80ff;
          }
   ```
   The dot makes this into a **class selector**. With a CSS **class** you can apply a set of CSS rules to any element on your website by adding an **attribute** to the element.

2. Now go to attractions.html and add the following **attribute** to the `<article>` tag:

   ```html
        <article class="purpleBackground">
   ```
   You should see the green background disappear from around the text on the Attractions page. Next you're going to make each section on that page have the green background instead!

3. Add the following class to your stylesheet:

   ```css
        .greenBackground {
            background-color: #48D1CC;
        }
   ```

   Back in the attractions.html file, add the attribute `class="greenBackground"` to each of the section tags, just like you did for the **article** element. Click Run and look at the Attractions page. Compare it to the other pages that have **section** elements.

4. When you use a CSS **element selector** such as **section**, the style rules apply to _all_ the elements of that type on your website. With CSS **classes** you're able to just change _some_ of them. You can add more than one class to an element too. Let's make another CSS **class** to give the sections some margin and padding. In _styles.css_, add the following code:
   ```css
        .sectionSpacing {
          padding: 10px;
          margin-top: 20px;
        }
   ```
5. In attractions.html, add the new class to each of the sections like this:
   ```html
        <section class="greenBackground sectionSpacing">
   ```
   You can add as many CSS classes to an element as you like. Just write the names of all the classes you want to use inside the **class** attribute, and separate them with spaces.

6. How about re-vamping the Food page? Add the following classes to your stylesheet:

   ```css
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

   ```html
        <section class="yellowBackground sectionSpacing solidRoundBorders">
   ```

7. Notice how you can mix and match the classes in your element's class attribute? Using CSS classes lets you **reuse** the same set of style rules on lots of elements. You can apply them to any element that has the properties you've set. Go to index.html and add the `.solidRoundBorders` class to the picture of Tito.

   ```html
        <img id="imgTito" class="solidRoundBorders" src="tito.png" alt="Tito the dog" width="100px">
   ```

8. Why not experiment with some more CSS classes to make the other pages on your website have their own themes? You can name a CSS class anything you like. It's common to give it a name that describes what it does or what it's for!

9. Extra challenge: use CSS **classes** to define a few different picture sizes for your website, for example `.smallPictures` and `.mediumPictures`. Then remove the **width** attribute from each of your **img** elements and add the appropriate class instead.
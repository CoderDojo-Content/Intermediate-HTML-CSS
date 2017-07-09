1. What if you want to apply a set of CSS rules to _more than one element_ but you don't want to change _all_ the elements that use that tag on your website? You can, with a CSS **class**!
2. Go to your stylesheet file and add the following. Be sure to include the dot in front!
    ```
        .purpleBackground {
            background-color: #9f80ff;
        }
    ```
3. Now go to attractions.html and add the following **attribute** to the `<article>` tag.
    ```
        <article class="purpleBackground">
    ```
You should see the green background disappear from around the text on the Attractions page. Next you're going to make each section on that page have the green background instead!
4. Add the following class to your stylesheet:
    ```
        .greenBackground {
            background-color: #48D1CC;
        }
    ```
Back in the attractions.html file, add the attribute `class="greenBackground"` to each of the section tags, just like you did for the `article` element.
Click Run and look at the Attractions page. Compare it to the other pages that have `section` elements.
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
3. You decide the name for your CSS class can be called anything you like.

5. Create a CSS class called `orange-underline` in your stylesheet as follows
    ```
        .orange-underline {
            color: orange;
            text-decoration: underline;
        }
    ```
6. Now go to index.html and add a paragraph of text with both the first class and the new class added to it:
    ```
        <p class="cool-roundy-borders orange-underline">
            Here is some text with two sets of CSS rules! 
        </p>
    ```
    * Don't forget the space in between the two class names inside your `class` attribute!

7. 


```
.solidRoundBorders {
border-style: solid;
border-width: 2px;
border-color: #F5FFFA;
border-radius: 10px;
}
```
1. What if you want to apply a set of CSS rules to more than one element but you don't want to change _all_ the elements that use that tag on your website? You can, with a CSS **class**!
2. Go to your stylesheet file and add the following. Be sure to include the dot in front!
    ```
        .solidRedBorders {
            border-style: solid;
            border-width: 2px;
            border-color: #C71585;
        }
    ```
3. Now go to index.html and add the following **attribute** to the `<img>` tag
    ```
        class="cool-roundy-borders"
    ```
4. ** create classes "round corners" and "square corners" and show that they can be used on anything that has the border-radius property! **
2. Choose one of your `<article>` blocks and add the following **attribute** to the opening tag
    ```
        <article class="
3. You decide the name for your CSS class can be called anything you like.
4. You can add more than one CSS class to an element. In fact you can add as many as you like. Just write the names of all the classes you want to use inside the `class` attribute, and separate them with spaces. Let's try that now.
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
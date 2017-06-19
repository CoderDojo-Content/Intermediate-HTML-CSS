1. Let's say you want to make CSS rules to style a certain few elements the same way.
2. Go to your stylesheet file and add the following. Be sure to include the dot in front!
    ```
        .cool-roundy-borders {
            border-style: solid;
            border-width: 2px;
            border-color: #ffe680;
            border-radius: 10px;
        }
    ```
3. Now go to one of your html files that has an `<img>` tag on it and add the following **attribute** to the tag
    ```
        class="cool-roundy-borders"
    ```
3. ** use img as the example?? **
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
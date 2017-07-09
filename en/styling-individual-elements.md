1. You can create a unique set of CSS rules to style one specific element.
2. Add the following **attribute** to one of the `p` tags in the `index.html` file
    ```
        <p id="myCoolText">
            My website is about Ireland.
        </p> 
    ```
    * The `id` is a name you give to **identify** this particular element.
3. Now go to your stylesheet and add the following code
    ```
        #myCoolText {
            color: #ffff66;
            text-decoration: underline;
        }
    ```
    * This is an **ID selector**. You can tell because of the `#` in front of it.
    * The name of the rule should exactly match the name you put in the element's `id` attribute
    * This styling apples to only one individual element on your website.
4. You can style any individual element on your website by giving it an `id` and using the ID selector in your stylesheet. Let's do one for the `body` of the homepage.
5. Go to index.html and add an `id` to the `body` tag.
    ```
        <body id="frontPage">
    ```
6. In the stylesheet, add CSS rules for the body of the homepage. You can upload any image you like, or use the one included with the example project.
    ```
        #frontPage {
            background-image: url("leaves.png");
        }
    ```
    * When you style using the ID selector like this, you can put in any rules you like for the element you are styling.
7. Try giving another element an `id` and styling that element using the id selector with `#` as above. How about making the picture of Tito have a `border-radius` of `100%` so that it's fully rounded? Your other pictures will stay the same as they are when you do it with this method.
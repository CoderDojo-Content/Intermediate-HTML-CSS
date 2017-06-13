1. You can create a unique set of CSS rules to style one specific element.
2. Add the following code to one of your `.html` files
    ```
        <p id="myCoolText">
            This is a paragraph with it's own special style!
        </p>
    ```
    * notice there is an **attribute** called **id**. This is a name you give to **identify** this particular element.
3. Now go to your stylesheet and add the following code
    ```
        #myCoolText {
            color: yellow;
            text-decoration: underline;
        }
    ```
    * This is an ID selector. You can tell because of the `#` in front of it.
    * Notice the `#` in front of the rule.
    * The name of the rule should exactly match the name you put in the element's `id` attribute
    * This styling apples to only one individual element on your website.
4. Try giving another element an `id` and styling that element using the id selector with `#` as above.
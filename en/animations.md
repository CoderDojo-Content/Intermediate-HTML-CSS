1. Go to the bottom of your CSS file and add the following code
    ```
        @keyframes my-first-animation {
            from {
                background-color: #ffe680;
            }
            to {
                background-color: purple;
            }
        }
    ```
    * This code creates an animation called "my-first-animation" that you can add to any element on your website. What do you think it does?
2. Go to the file index.html and add the following code:
    ```
        <h1>Hey, now you can do animations!</h1>
        <h1 id="my-cool-heading">Cool!!</h1>
    ```
3. Go to the stylesheet and create CSS rules for the element, using the ID selector:
    ```
        #my-cool-heading {
            background-color: #ffe680;
            border-style: solid;
            border-width: 3px;
            padding: 20px;
            width: 80px;
        }
    ```
4. Now add the following rule to the same set of rules:
    ```
        animation-name: my-first-animation;
        animation-duration: 2s;
        animation-iteration-count: 1;
    ```
5. Run your code to see what happens! Did the colours change? 
6. Let's add some movement! Change your animation so that it looks like this
    ```
        @keyframes my-first-animation {
            from {
                background-color: #ffe680;
                transform: rotate(0deg);
            }
            to {
                background-color: purple;
                transform: rotate(360deg);
            }
        }
    ```
 * What do you think the new lines will do? Run your code and find out!
7. Another way to set start and end values is with **percentages** instead of the keywords `from` and `to`. That allows you to set in between values as well! Go to the bottom of your CSS file and add the following code
    ```
        @keyframes spin-around {
            0% {
                transform: rotate(0deg);
            }
            50% {
                transform: rotate(-90deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
    ```
    * You can set as many in between values as you like using different percentages
8. Go to the file index.html and add the following code below the new stuff:
    ```
        <p id="emoji-text">(",)</p>
    ```
9. Go to the stylesheet and create CSS rules for the element, using the ID selector:
    ```
        #emoji-text {
            animation-name: spin-around;
            animation-duration: 2s;
            animation-iteration-count: 3;
        }
    ```
10. Change the `animation-iteration-count` from `3` to `infinite`. What happens when you run your code now?
11. You can also play with different values for `animation-duration` to speed up or slow down your animation. 
12. Extra challenges:
 * Add some code to the `spin-around` animation to make the text change colour. Remember the property for text colour is called `color` 
 * Add another in-between value, for example 75%, which sets different rotation and colour values.
13. You can put the `animation` properties into the CSS rules for any element on your website. How about making one of your images spin around?
 * To learn about more things you can do with animation, visit dojo.soy/css-animation**TODO-LINK**
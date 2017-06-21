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
            width: 80px;
            padding: 20px;
            width: 80px;
        }
    ```
4. Now add the following rule to the same set of rules:
    ```
        animation: my-first-animation 2s 3;
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
10. Another way to set start and end values is with **percentages** instead of the keywords `from` and `to`. That allows you to set in between values as well! Go to the bottom of your CSS file and add the following code
    ```
        @keyframes spin-around {
            0% {
                background-color: #ffe680;

                transform: rotate(0deg);
            }
            50% {
                background-color: paleturquoise;
            }
            100% {
                background-color: #ffe680;

                transform: rotate(360deg);
            }
        }
    ```
    * You can set as many in between values as you like using different percentages
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
            width: 80px;
            padding: 20px;
            width: 80px;
        }
    ```
4. Now add the following rule to the same set of rules:
    ```
        animation: spin-around 2s 3;
    ```
5. **TODO** EXPLAIN THE PERCENTAGES AND STUFF


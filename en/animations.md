1. Go to the bottom of your CSS file and add the following code
    ```
        @keyframes spin-around {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
    ```
    * This code creates an animation called "spin-around" that you can add to any element on your website. What do you think it does?
2. **TODO** Go to the file index.html and add the following code.
    ```
        <h1 id="my-cool-heading">Hey cool, animations!!</h1>
    ```
3. Go to the stylesheet and create CSS rules for the element, using the ID selector:
    ```
        #my-cool-heading {
            background-color: #ffe680;
            border-style: solid;
            border-width: 3px;
            padding: 20px;
        }
    ```
4. Now add the following rule to the same set of rules:
    ```
        animate: spin-around 2s 3;
    ```
5. **TODO** EXPLAIN THE PERCENTAGES AND STUFF

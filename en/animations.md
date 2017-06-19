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
2. **TODO** Go to one of your HTML files. ..... Create some element with a unique ID.
3. Go to the stylesheet and create CSS rules for the element, using the ID selector:
    ```
        #cool-element {
            background-color: #something;
            border: something too;
        }
    ```
4. Now add the following rule to the same set of rules:
    ```
        animate: spin-around 2s 3;
    ```
5. **TODO** EXPLAIN THE PERCENTAGES AND STUFF

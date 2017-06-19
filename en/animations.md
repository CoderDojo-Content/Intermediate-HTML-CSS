1. Create some element with a unique ID.
2. Go to the stylesheet and create CSS rules for the element, using the ID selector:
    ```
        #cool-element {
            background-color: #something;
            border: something too;
        }
    ```
3. Now add the following rule to the same set of rules:
    ```
        animate: spin-around 2s 3;
    ```
4. Go to the bottom of your CSS file and add the following code
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
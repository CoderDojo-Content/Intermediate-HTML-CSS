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
2. Find your CSS rules for the ID `#myCoolText` and add the following properties inside the curly braces:
    ```
        animation-name: myFirstAnimation;
        animation-duration: 2s;
        animation-iteration-count: 1;
    ```
 * Check the index.html file to make sure you still have a paragraph with the attribute `id="myCoolText"`
3. Run your code to see what happens! Did the colours change?
4. Change the value of `animation-iteration-count` to another number instead of 1 and run your code again to see what it does.
5. Let's try another animation! Add the following code to the end of your CSS file: 
    ```
        @keyframes spinAroundAnimation {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
        
        .animateMe {
            animation-name: spinAroundAnimation;
            animation-duration: 1s;
            animation-iteration-count: 3;
        }
    ```
 * The second block is a new CSS class
6. In index.html, add the class `animateMe` to the picture of Tito and then click Run to see the new animation.
    ```
        <img id="imgTito" class="solidRoundBorders animateMe" src="tito.png" alt="Tito the dog" width="100px">
    ```
7. In the `.animateMe` CSS class, change the `animation-iteration-count` from `3` to `infinite`. What happens when you run your code now?
 * You can also play with different values for `animation-duration` to speed up or slow down your animation. 
8. Did you notice that in the second animation you used `0%` and `100%` instead of `from` and `to` to set the start and end values? With **percentages** you're able to set in between values as well as just start and end values. Change the animation code so that it looks like this: 
    ```
        @keyframes spinAroundAnimation {
            0% {
                transform: rotate(0deg);
            }
            25% {
                transform: rotate(-180deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }
    ```
    * You can set as many in between values as you like using different percentages
    * Values for rotate can go from 0deg up to 360deg (full circle). A **minus** number means it rotates backwards!
10. Try adding the `animateMe` class to other elements on your website (by adding the **attribute** `class="animateMe" inside the opening tag!) to make them spin too!
9. Extra challenges:
 * Add some code to the `myFirstAnimation` animation to make the text change colour. Remember the property for text colour is called `color` 
 * Add another in-between value, for example 75%, which sets different rotation and colour values.
13. You can put the `animation` properties into the CSS rules for any element on your website. How about making one of your images spin around?
 * To learn about more things you can do with animation, visit dojo.soy/css-animation**TODO-LINK**
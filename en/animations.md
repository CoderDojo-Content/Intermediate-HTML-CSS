1. Go to the bottom of your CSS file and add the following code
   ```css
        @keyframes myFirstAnimation {
            from {
                width: 100px;
            }
            to {
                width: 300px;
            }
        }
   ```
* This code creates an animation called "myFirstAnimation" that you can add to any element on your website. What do you think it does?

2. Find your CSS rules for the ID _#imgTito_ and add the following three properties:
   ```css
        animation-name: myFirstAnimation;
        animation-duration: 2s;
        animation-iteration-count: 1;
   ```

3. Run your code to see what happens! Change the value of **animation-iteration-count** to another number instead of _1_ and run your code again to see what it does.

5. Let's try another animation! Add the following code to the end of your CSS file:
   ```css
        @keyframes glowPulse {
            0% {
                color: DeepSkyBlue;
            }
            50% {
                color: LightGreen;
            }
            100% {
                color: DeepSkyBlue;
            }
        }
   ```
   Now find the _#myCoolText_ CSS rules from earlier and add in the animation code:
   ```css
    #myCoolText {
            animation-name: myFirstAnimation;
            animation-duration: 2s;
            animation-iteration-count: 1;
    }
   ```

6. When you use **percentages** instead of **from** and **to**, you're able to set in between values as well as just start and end values. You can set as many in between values as you like using different percentages. Try adding in more colours to the glowing sequence above, for example at _25%_ and _75%_!

7. Change the value of **animation-iteration-count** to _infinite_. What do you think will happen?
 * You can also play with different values for **animation-duration** to speed up or slow down your animation.

8. One final trick! Add this animation code:
   ```css
        @keyframes slide {
        0% {
            background-position-x: 0;
        }
        100% {
            background-position-x: 600vw;
        }
        }
   ```
   Now find the _#frontPage_ CSS rules from earlier and change them to:
   ```css
        #frontPage {
            background: repeating-linear-gradient(-45deg, red 0%, yellow 7.14%, lime 14.28%, cyan 21.42%, cyan 28.56%, blue 35.7%, magenta 42.84%, red 50%);
            background-size: 600vw 600vw;
            animation: slide 10s infinite linear forwards;
        }
   ```
   Don't worry about understanding _all_ of it... just sit back and enjoy!!
  
 9. Why not try making your own new animation using the **@keyframes** keyword and a name that you choose? Use the code you learned above to help you. You can add any properties you like in the animation blocks. How about animating your nav menu?
 
 10. To learn about more things you can do with animation, visit [dojo.soy/css-animation](https://www.w3schools.com/css/css3_animations.asp). Have fun!


1. Let's make images do something cool when you hover over them with the mouse! If you don't have any images on your page, upload one in the images tab, and then add it using the `<img>` tag. If you are working from the example project, you may use the photo of Tito the dog that's included.
2. Your html file should now contain something like the following code on it
    ```
        <img src="Tito.png" alt="Tito the dog" width="100px">
    ```  		
3. Add the following style code in the CSS file. The first part should look familiar. Run the code and move the mouse over the picture to see what happens!
  ```
    img {
      border-radius: 50%;
      border-style: dotted;
      border-width: 3px;
      border-color: #ffe680;
    }
    img:hover {
      border-style: solid;
      border-width: 3px;
      border-color: pink;
    }
  ```  
4. You've just used a special type of CSS block called a **pseudo-class**. Remember how you could assign a **class** name to any one or more elements to style them the same way? Well, `:hover` is a bit like that, but it comes built in so you don't need to add it to your elements. All you need to do to use it is to create `:hover` style rules in your CSS file for whatever elements you want to use it on.
 * You're not just limited to normal element selectors. You can use the `:hover` pseudo-class with any selector in CSS. So you could make hover styling for your classes too, or for individual elements with an ID.
5. Let's use this new `:hover` **pseudo-class** together with a CSS class to make links glow when you hover over them! Add a link to your web page and include an attribute to specify the class name.  
  ```<a class="nice-links" href="http://www.failteireland.ie/">Irish Tourism website</a>
  ```
  * Remember links are defined using the `a` tag
6. Now add the following code to your stylesheet and then run your code to see your lovely links in action.
  ```
    .nice-links {
      text-decoration: none;
      color: Brown;
    }
    .nice-links:hover {
      color: purple;
      background-color: PapayaWhip;
      border-radius: 10px;
    }
  ```
 * Why not add the attribute `class="nice-links"` to all of the links in your menu bar as well? This will make your menu bar even more interactive!
7. You can combine all of these tricks with animations too! 
8. Add the following animation to your CSS file:
  ```
    @keyframes glow-pulse {
      0% {
        border-style: solid;
        border-width: 10px;
        border-color: papayawhip;
      }
      50% {
        border-style: solid;
        border-width: 10px;
        border-color: pink;
      }
      100% {
        border-style: solid;
        border-width: 10px;
        border-color: papayawhip;
      }
    }
  ```
9. In your `.nice-links:hover` block, add three more CSS rules:
  ```
    animation-name: glow-pulse;
    animation-duration: 1.5s;
    animation-iteration-count: infinite;
  ```
10. Now your link should have a glowing border that appears to pulse on and off whenever you hover the mouse over it!


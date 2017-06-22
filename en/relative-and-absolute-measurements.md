1. Up until now you've been using **pixels** to set the size of things, e.g. `10px`. This is called an **absolute** measurement. It means you set an exact size and it doesn't change.
2. Another way to set the size of things is using **relative** measurements. That means how big elements are in relation to each other. So when one thing changes size, everything else will automatically change as well to keep the same **proportions**. 
 * Have you noticed that on many websites, when you make the window bigger or smaller, things on the page automatically shrink and grow to match the window size? This is an example of **relative** measurements in action.
3. Go to index.html where you have your picture of Tito (or the picture you uploaded). Delete the width attribute `width="100px"` and add an ID attribute for the image
 ```
  <img id="imgTito" src="tito.png" alt="Tito the dog">
 ``` 
4. In your CSS file and add the following code
 ```
  #imgTito {
    width: 50%;
  }
 ```
5. Try a few different percentages and see if you can work out what it's doing.
 * When you're using **relative** measurements it's important to know what the **parent** of your element is. The **parent** is the thing that your element is inside, and that's what the measurement will be in relation to. For example, parent of the image above is the `main` because the `img` tag is in between the `<main></main> tags`.
6. Now in your html file, put the image inside an `article` element. Include some text too. 
 ```
  <article>
     <img id="imgTito" src="tito.png" alt="Tito the dog">  		
     <p>
       This is Tito. He will be your tourguide! As you can see, Tito loves CoderDojo.
     </p>
   </article>
  ```
7. Add the following code to your stylesheet, so you can see what's going on more clearly
 ```
  article {
    width: 200px;
    background-color: white;
  }
 ```
 * If you don't give `article`s a width, they fill up all the space available, which is usually a good thing!
8. You should notice that the picture is much smaller now. That is because it is taking up 50% of the width of the `article` element instead of the `main` element (which is the width of the page).
9. Another **relative** unit of measurement is `em`, which is related to the size of your text. Add the following to your html file, outside of the article tags.
 ```
  <p class="funsize">A magical paragraph</p>
 ```
 Then, in your CSS file, add the following code
 ```
    .funsize {
      border: 2px solid slateblue;
      padding: 5px;
      font-family: "Helvetica", sans-serif;
      font-size: 1.5em;
    }
 ```
 * the border is included so you can see the spacing more easily
10. Set the font-size to different values for example `2em`, `3em`, `4em`. Can you see that the **padding** (space between the border and the text) doesn't change?
11. With the padding staying the same, the space starts to look too small as the text gets bigger. Let's give it a **relative** value instead of the **absolute** pixel value. Change it to
 ```
  padding: 1em;
 ```
12. Now experiment again with different values for **font-size**. You should see the spacing change to match the font size this time.
 * the number with `em` refers to the width of the letter **m**


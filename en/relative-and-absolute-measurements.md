1. Up until now you've been using **pixels** to set the size of things, e.g. `10px`. This is called an **absolute** measurement. It means you set an exact size and it doesn't change.
2. Another way to set the size of things is using **relative** measurements. That means how big elements are in relation to each other. So when one thing changes size, everything else will automatically change as well to keep the same **proportions**. 
 * Have you noticed that on many websites, when you make the window bigger or smaller, things on the page automatically shrink and grow to match the window size? This is an example of **relative** measurements in action.
3. ~~You have already used one relative measurement when you set font sizes in the Beginner Sushi series.~~ NOPE

3. Go to index.html where you have your picture of Tito (or the picture you uploaded). Delete the width attribute `width="100px"` and add an ID attribute for the image
 ```
  <img id="imgTito" src="tito.png" alt="Tito the dog">
 ``` 
4. Go to your CSS file and add the following code
 ```
  #imgTito {
   width: 50%;
  }
 ```
5. Try a few different percentages and see how it works.
 * When you're using **relative** measurements it's important to know what the **parent** of your element is. The **parent** is the thing that your element is inside. For example, parent of the image above is the `main` because the `img` tag is in between the `<main></main> tags`.
6. Now your html file, put the image inside an `article` element. Include some text too if you like. 
7. Add the following code to your stylesheet, so you can see what's going on more clearly
 ```
  article {
    width: 200px;
    background-color: white;
  }
 ```
 * If you don't give `article`s a width, they fill up all the space available, which is usually a good thing!
8. You should notice that the picture is much smaller now. That is because it is taking up 50% of the width of the `article` element instead of the `main` element (which is the width of the page).
9. Another **relative** unit of measurement is `em`, which is related to the size of your text.

10. It's a good idea to set the size in CSS rather than in the HTML tags. 
 * do example by id first, then show how to use classes cleverly %, vh, em) and absolute (p
11. put in a container (e.g. article) and set the height according to that
12. em for Margins and padding !! Also for font-size i.e. relative to the parent as opposed to setting font-size 12pt
13. SHOULD BE USING EM FOR FONT SIZES ALWAYS ANYWAY -- CHECK THIS IN THE BEGINNER SERIES! Can then just refer to it (he remember this?) and explain it now.

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
  
  }
 ```
10. It's a good idea to set the size in CSS rather than in the HTML tags. 
 * do example by id first, then show how to use classes cleverly %, vh, em) and absolute (p
11. put in a container (e.g. article) and set the height according to that
12. em for Margins and padding !! Also for font-size i.e. relative to the parent as opposed to setting font-size 12pt
13. SHOULD BE USING EM FOR FONT SIZES ALWAYS ANYWAY -- CHECK THIS IN THE BEGINNER SERIES! Can then just refer to it (he remember this?) and explain it now.

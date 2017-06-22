1. Up until now you've been using **pixels** to set the size of things, e.g. `10px`. This is called an **absolute** measurement. It means you set an exact size and it doesn't change.
2. Have you noticed that on many websites, when you make the window bigger or smaller, things on the page automatically shrink and grow to match the window size? You can make your website do this too by using **relative** measurements.
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
12. em for Margins and padding !!

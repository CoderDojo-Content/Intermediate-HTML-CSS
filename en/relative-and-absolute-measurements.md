1. Up until now you've been using **pixels** to set the size of things, e.g. `10px`. This is called an **absolute** measurement. It means you set an exact size and it doesn't change. Another way to set the size of things is using **relative** measurements. That means how big elements are in relation to each other. So when one thing changes size, everything else will automatically change as well to keep the same **proportions**. 
 * Have you noticed that on many websites, when you make the window bigger or smaller, things on the page automatically shrink and grow to match the window size? This is an example of **relative** measurements in action.

2. Go to index.html and find the `img` element with the picture of Tito. Delete the width attribute `width="100px"`.
  ```
    <img id="imgTito" src="tito.png" alt="Tito the dog">
  ``` 
4. In your CSS file find the `#imgTito` code block and add the `width` property below:
  ```
    #imgTito {
      border-radius: 100%;
      width: 50%;
    }
  ```
 50% (50 percent) is **half**. Try a few different percentages and see if you can work out what it's doing.

5. When you're using **relative** measurements it's important to know what the **parent** of your element is. The **parent** is the thing that your element is inside, and that's what the measurement will be in relation to. For example, **parent** of the image above is the `article` element because the `img` element is in between the `<article></article> tags`.
6. Now in your html file, put the image inside a `section` element with `id` "titoSection". Include some text too. 
  ```
    <section id="titoSection">
      <img id="imgTito" src="tito.png" alt="Tito the dog">  		
      <p>
        This is Tito. He will be your tourguide! As you can see, Tito loves CoderDojo.
      </p>
    </section>
  ```
7. Add the following code to your stylesheet, so you can see what's going on more clearly
 ```
  article {
    width: 200px;
    background-color: white;
  }
 ```
 * If you don't give `section` elements a width, they fill up all the space available, which is usually a good thing!
8. You should notice that the picture is much smaller now. That is because it is taking up 50% of the width of the `section` element instead of the `article` element \(which is the width of the page\).
9. Another **relative** unit of measurement is `em`, which is related to the size of your text. **Cut** the heading `<h1>Welcome to Ireland!</h1>` and **paste** it on a new line _above_ the opening `<article>` tag, so that it's outside of the `article` element. Add a class **attribute** to the heading as well.
  ```
    <main>	
      <h1 class="funsize">Welcome to Ireland!</h1>
      <article>
  ```
 Then, in your CSS file, add the following code. There is a border so you can see the spacing more easily.
 ```
    .funsize {
      border: 2px solid #FFFFFF;
      padding: 5px;
      font-family: "Helvetica", sans-serif;
      font-size: large;
    }
 ```

10. Set the font-size to different values for example `smaller`, `small`, `medium`, `larger`. Can you see that the **padding** (space between the border and the text) doesn't change?
11. With the padding staying the same, the space starts to look small as the text gets bigger. Let's give it a **relative** value instead of the **absolute** pixel value. Change it to
  ```
    padding: 1em;
  ```
12. Now experiment again with different values for **font-size**. You should see the spacing change to match the font size this time.
 * Setting the size of anything to `1em` makes it the same size as the text; setting it to `2em` makes it twice the size of the text, and so on.
13. You can use `em` values for anything you can set the size of, not just padding. Experiment with using it instead of `px` on borders, or instead of `%` on your image!


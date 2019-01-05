# Introduction to Basic CSS

https://learn.freecodecamp.org/responsive-web-design/basic-css

Cascading Style Sheets (CSS) tell the browser how to display the text and other content that you write in HTML. 

## <a name="indice">Índice</a>

1. [Change the Color of Text](#parte1)     
2. [Use CSS Selectors to Style Elements](#parte2)     
3. [Use a CSS Class to Style an Element](#parte3)     
4. [Style Multiple Elements with a CSS Class](#parte4)     
5. [Change the Font Size of an Element](#parte5)     
6. [Set the Font Family of an Element](#parte6)     
7. [Import a Google Font](#parte7)     
8. [Specify How Fonts Should Degrade](#parte8)     
9. [Size Your Images](#parte9)     
10. [Add Borders Around Your Elements](#parte10)     
11. [Add Rounded Corners with border-radius](#parte11)     
12. [Make Circular Images with a border-radius](#parte12)     
13. [Give a Background Color to a div Element](#parte13)     
14. [Set the id of an Element](#parte14)     
15. [Use an id Attribute to Style an Element](#parte15)     
16. [Adjust the Padding of an Element](#parte16)     
17. [Adjust the Margin of an Element](#parte17)     
18. [Add a Negative Margin to an Element](#parte18)     
19. [Add Different Padding to Each Side of an Element](#parte19)     
20. [Add Different Margins to Each Side of an Element](#parte20)     
21. [Use Clockwise Notation to Specify the Padding of an Element](#parte21)     
22. [Use Clockwise Notation to Specify the Margin of an Element](#parte22)     
23. [Use Attribute Selectors to Style Elements](#parte23)     
24. [Understand Absolute versus Relative Units](#parte24)     
25. [Style the HTML Body Element](#parte25)     
26. [Inherit Styles from the Body Element](#parte26)     
27. [Prioritize One Style Over Another](#parte27)     
28. [Override Styles in Subsequent CSS](#parte28)     
29. [Override Class Declarations by Styling ID Attributes](#parte29)     
30. [Override Class Declarations with Inline Styles](#parte30)     
31. [Override All Other Styles by using Important](#parte31)     
32. [Use Hex Code for Specific Colors](#parte32)     
33. [Use Hex Code to Mix Colors](#parte33)     
34. [Use Abbreviated Hex Code](#parte34)     
35. [Use RGB values to Color Elements](#parte35)     
36. [Use RGB to Mix Colors](#parte36)     
37. [Use CSS Variables to change several elements at once](#parte37)     
38. [Create a custom CSS Variable](#parte38)     
39. [Use a custom CSS Variable](#parte39)     
40. [Attach a Fallback value to a CSS Variable](#parte40)     
41. [Improve Compatibility with Browser Fallbacks](#parte41)     
42. [Cascading CSS variables](#parte42)     
43. [Change a variable for a specific area](#parte43)     
44. [Use a media query to change a variable](#parte44)     
---


## <a name="parte1">1 - Change the Color of Text</a>

Now let's change the color of some of our text.

We can do this by changing the style of your h2 element.

The property that is responsible for the color of an element's text is the color style property.

Here's how you would set your h2 element's text color to blue:

<h2 style="color: blue;">CatPhotoApp</h2>

Note that it is a good practice to end inline style declarations with a ; .


Change your h2 element's style so that its text color is red.

```html
<h2 style="color: red;">CatPhotoApp</h2>
<main>
  <p>Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Use CSS Selectors to Style Elements</a>

With CSS, there are hundreds of CSS properties that you can use to change the way an element looks on your page.

When you entered <h2 style="color: red">CatPhotoApp</h2>, you were styling that individual h2 element with inline CSS, which stands for Cascading Style Sheets.

That's one way to specify the style of an element, but there's a better way to apply CSS.

At the top of your code, create a style block like this:

```html
<style>
</style>
```

Inside that style block, you can create a CSS selector for all h2 elements. For example, if you wanted all h2 elements to be red, you would add a style rule that looks like this:

```html
<style>
  h2 {color: red;}
</style>
```

Note that it's important to have both opening and closing curly braces ({ and }) around each element's style rule(s). You also need to make sure that your element's style definition is between the opening and closing style tags. Finally, be sure to add a semicolon to the end of each of your element's style rules.

Delete your h2 element's style attribute, and instead create a CSS style block. Add the necessary CSS to turn all h2 elements blue.

```html
<style>
  h2{
    color:blue;
  }
</style>
<h2>CatPhotoApp</h2>
<main>
  <p>Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Use a CSS Class to Style an Element</a>

Classes are reusable styles that can be added to HTML elements.

Here's an example CSS class declaration:

```html
<style>
  .blue-text {
    color: blue;
  }
</style>
```

You can see that we've created a CSS class called blue-text within the <style> tag.

You can apply a class to an HTML element like this:

```html
<h2 class="blue-text">CatPhotoApp</h2>
```

Note that in your CSS style element, class names start with a period. In your HTML elements' class attribute, the class name does not include the period.


Inside your style element, change the h2 selector to .red-text and update the color's value from blue to red.

Give your h2 element the class attribute with a value of 'red-text'.

```html
<style>
  .red-text{
    color: red;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>
<main>
  <p>Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Style Multiple Elements with a CSS Class</a>

Classes allow you to use the same CSS styles on multiple HTML elements. You can see this by applying your red-text class to the first p element.

```html
<style>
  .red-text {
    color: red;
  }
  .red-text{

  }
</style>

<h2 class="red-text">CatPhotoApp</h2>
<main>
  <p class="red-text">Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Change the Font Size of an Element</a>

Font size is controlled by the font-size CSS property, like this:

```css
h1 {
  font-size: 30px;
}
```

Inside the same <style> tag that contains your red-text class, create an entry for p elements and set the font-size to 16 pixels (16px).

```html
<style>
  .red-text {
    color: red;
  }
  p{
    font-size: 16px;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>
<main>
  <p class="red-text">Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```

[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Set the Font Family of an Element</a>

You can set which font an element should use, by using the font-family property.

For example, if you wanted to set your h2 element's font to sans-serif, you would use the following CSS:

```css
h2 {
  font-family: sans-serif;
}
```

Make all of your p elements use the monospace font.

```html
<style>
  .red-text {
    color: red;
  }

  p {
    font-size: 16px;
     font-family: monospace;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>
<main>
  <p class="red-text">Click here to view more <a href="#">cat photos</a>.</p>
  
  <a href="#"><img src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
  
  <div>
    <p>Things cats love:</p>
    <ul>
      <li>cat nip</li>
      <li>laser pointers</li>
      <li>lasagna</li>
    </ul>
    <p>Top 3 things cats hate:</p>
    <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
  </div>
  
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor" checked> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label><br>
    <label><input type="checkbox" name="personality" checked> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Energetic</label><br>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</main>
```


[Voltar ao Índice](#indice)

---


## <a name="parte7">7 - Import a Google Font</a>



[Voltar ao Índice](#indice)

---


## <a name="parte8">8 - Specify How Fonts Should Degrade</a>



[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Size Your Images</a>



[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Add Borders Around Your Elements</a>



[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Add Rounded Corners with border-radius</a>



[Voltar ao Índice](#indice)

---


## <a name="parte12">12 - Make Circular Images with a border-radius</a>



[Voltar ao Índice](#indice)

---


## <a name="parte13">13 - Give a Background Color to a div Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte14">14 - Set the id of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte15">15 - Use an id Attribute to Style an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte16">16 - Adjust the Padding of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte17">17 - Adjust the Margin of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte18">18 - Add a Negative Margin to an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte19">19 - Add Different Padding to Each Side of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte20">20 - Add Different Margins to Each Side of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte21">21 - Use Clockwise Notation to Specify the Padding of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte22">22 - Use Clockwise Notation to Specify the Margin of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte23">23 - Use Attribute Selectors to Style Elements</a>



[Voltar ao Índice](#indice)

---


## <a name="parte24">24 - Understand Absolute versus Relative Units</a>



[Voltar ao Índice](#indice)

---


## <a name="parte25">25 - Style the HTML Body Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte26">26 - Inherit Styles from the Body Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte27">27 - Prioritize One Style Over Another</a>



[Voltar ao Índice](#indice)

---


## <a name="parte28">28 - Override Styles in Subsequent CSS</a>



[Voltar ao Índice](#indice)

---


## <a name="parte29">29 - Override Class Declarations by Styling ID Attributes</a>



[Voltar ao Índice](#indice)

---


## <a name="parte30">30 - Override Class Declarations with Inline Styles</a>



[Voltar ao Índice](#indice)

---


## <a name="parte31">31 - Override All Other Styles by using Important</a>



[Voltar ao Índice](#indice)

---


## <a name="parte32">32 - Use Hex Code for Specific Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte33">33 - Use Hex Code to Mix Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte34">34 - Use Abbreviated Hex Code</a>



[Voltar ao Índice](#indice)

---


## <a name="parte35">35 - Use RGB values to Color Elements</a>



[Voltar ao Índice](#indice)

---


## <a name="parte36">36 - Use RGB to Mix Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte37">37 - Use CSS Variables to change several elements at once</a>



[Voltar ao Índice](#indice)

---


## <a name="parte38">38 - Create a custom CSS Variable</a>



[Voltar ao Índice](#indice)

---


## <a name="parte39">39 - Use a custom CSS Variable</a>



[Voltar ao Índice](#indice)

---


## <a name="parte40">40 - Attach a Fallback value to a CSS Variable</a>



[Voltar ao Índice](#indice)

---


## <a name="parte41">41 - Improve Compatibility with Browser Fallbacks</a>



[Voltar ao Índice](#indice)

---


## <a name="parte42">42 - Cascading CSS variables</a>



[Voltar ao Índice](#indice)

---


## <a name="parte43">43 - Change a variable for a specific area</a>



[Voltar ao Índice](#indice)

---


## <a name="parte44">44 - Use a media query to change a variable</a>



[Voltar ao Índice](#indice)

---


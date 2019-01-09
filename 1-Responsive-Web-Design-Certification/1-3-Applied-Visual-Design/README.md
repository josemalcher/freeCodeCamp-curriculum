# Introduction to the Applied Visual Design Challenges

https://learn.freecodecamp.org/responsive-web-design/applied-visual-design

Visual Design in web development is a broad topic. It combines typography, color theory, graphics, animation, and page layout to help deliver a site's message. The definition of good design is a well-discussed subject, with many books on the theme. 

## <a name="indice">Índice</a>

1. [Create Visual Balance Using the text-align Property](#parte1)     
2. [Adjust the Width of an Element Using the width Property](#parte2)     
3. [Adjust the Height of an Element Using the height Property](#parte3)     
4. [Use the strong Tag to Make Text Bold](#parte4)     
5. [Use the u Tag to Underline Text](#parte5)     
6. [Use the em Tag to Italicize Text](#parte6)     
7. [Use the s Tag to Strikethrough Text](#parte7)     
8. [Create a Horizontal Line Using the hr Element](#parte8)     
9. [Adjust the background-color Property of Text](#parte9)     
10. [Adjust the Size of a Header Versus a Paragraph Tag](#parte10)     
11. [Add a box-shadow to a Card-like Element](#parte11)     
12. [Decrease the Opacity of an Element](#parte12)     
13. [Use the text-transform Property to Make Text Uppercase](#parte13)     
14. [Set the font-size for Multiple Heading Elements](#parte14)     
15. [Set the font-weight for Multiple Heading Elements](#parte15)     
16. [Set the font-size of Paragraph Text](#parte16)     
17. [Set the line-height of Paragraphs](#parte17)     
18. [Adjust the Hover State of an Anchor Tag](#parte18)     
19. [Change an Element's Relative Position](#parte19)     
20. [Move a Relatively Positioned Element with CSS Offsets](#parte20)     
21. [Lock an Element to its Parent with Absolute Positioning](#parte21)     
22. [Lock an Element to the Browser Window with Fixed Positioning](#parte22)     
23. [Push Elements Left or Right with the float Property](#parte23)     
24. [Change the Position of Overlapping Elements with the z-index Property](#parte24)     
25. [Center an Element Horizontally Using the margin Property](#parte25)     
26. [Learn about Complementary Colors](#parte26)     
27. [Learn about Tertiary Colors](#parte27)     
28. [Adjust the Color of Various Elements to Complementary Colors](#parte28)     
29. [Adjust the Hue of a Color](#parte29)     
30. [Adjust the Tone of a Color](#parte30)     
31. [Create a Gradual CSS Linear Gradient](#parte31)     
32. [Use a CSS Linear Gradient to Create a Striped Element](#parte32)     
33. [Create Texture by Adding a Subtle Pattern as a Background Image](#parte33)     
34. [Use the CSS Transform scale Property to Change the Size of an Element](#parte34)     
35. [Use the CSS Transform scale Property to Scale an Element on Hover](#parte35)     
36. [Use the CSS Transform Property skewX to Skew an Element Along the X-Axis](#parte36)     
37. [Use the CSS Transform Property skewY to Skew an Element Along the Y-Axis](#parte37)     
38. [Create a Graphic Using CSS](#parte38)     
39. [Create a More Complex Shape Using CSS and HTML](#parte39)     
40. [Learn How the CSS @keyframes and animation Properties Work](#parte40)     
41. [Use CSS Animation to Change the Hover State of a Button](#parte41)     
42. [Modify Fill Mode of an Animation](#parte42)     
43. [Create Movement Using CSS Animation](#parte43)     
44. [Create Visual Direction by Fading an Element from Left to Right](#parte44)     
45. [Animate Elements Continually Using an Infinite Animation Count](#parte45)     
46. [Make a CSS Heartbeat using an Infinite Animation Count](#parte46)     
47. [Animate Elements at Variable Rates](#parte47)     
48. [Animate Multiple Elements at Variable Rates](#parte48)     
49. [Change Animation Timing with Keywords](#parte49)     
50. [Learn How Bezier Curves Work](#parte50)     
51. [Use a Bezier Curve to Move a Graphic](#parte51)     
52. [Make Motion More Natural Using a Bezier Curve](#parte52)     
---


## <a name="parte1">1 - Create Visual Balance Using the text-align Property</a>

This section of the curriculum focuses on Applied Visual Design. The first group of challenges build on the given card layout to show a number of core principles.

Text is often a large part of web content. CSS has several options for how to align it with the text-align property.

text-align: justify; causes all lines of text except the last line to meet the left and right edges of the line box.

text-align: center; centers the text

text-align: right; right-aligns the text

And text-align: left; (the default) left-aligns the text.


Align the h4 tag's text, which says "Google", to the center. Then justify the paragraph tag which contains information about how Google was founded.

```html
<style>
  h4 {
    text-align: center;
  }
  p {
    text-align:justify;
  }
  .links {
    margin-right: 20px;
    
  }
  .fullCard {
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Adjust the Width of an Element Using the width Property</a>

You can specify the width of an element using the width property in CSS. Values can be given in relative length units (such as em), absolute length units (such as px), or as a percentage of its containing parent element. Here's an example that changes the width of an image to 220px:

```css
img {
  width: 220px;
}
```

Add a width property to the entire card and set it to an absolute value of 245px. Use the fullCard class to select the element.

```html
<style>
  h4 {
    text-align: center;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;
    text-align: left;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Adjust the Height of an Element Using the height Property</a>

You can specify the height of an element using the height property in CSS, similar to the width property. Here's an example that changes the height of an image to 20px:

```css
img {
  height: 20px;
}
```

Add a height property to the h4 tag and set it to 25px.

```html
<style>
  h4 {
    text-align: center;
    height:25px;
  }
  p {
    text-align: justify;
  }
  .links {
    margin-right: 20px;
    text-align: left;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at Stanford University.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Use the strong Tag to Make Text Bold</a>

To make text bold, you can use the strong tag. This is often used to draw attention to text and symbolize that it is important. With the strong tag, the browser applies the CSS of font-weight: bold; to the element.


Wrap a strong tag around "Stanford University" inside the p tag.

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were Ph.D. students at <strong>Stanford University</strong>.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Use the u Tag to Underline Text</a>

To underline text, you can use the u tag. This is often used to signify that a section of text is important, or something to remember. With the u tag, the browser applies the CSS of text-decoration: underline; to the element.


Wrap the u tag only around the text "Ph.D. students".

Note
Try to avoid using the u tag when it could be confused for a link. Anchor tags also have a default underlined formatting.

```html

<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Use the em Tag to Italicize Text</a>

To emphasize text, you can use the em tag. This displays text as italicized, as the browser applies the CSS of font-style: italic; to the element.


Wrap an em tag around the contents of the paragraph tag to give it emphasis.

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Google</h4>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte7">7 - Use the s Tag to Strikethrough Text</a>

To strikethrough text, which is when a horizontal line cuts across the characters, you can use the s tag. It shows that a section of text is no longer valid. With the s tag, the browser applies the CSS of text-decoration: line-through; to the element.


Wrap the s tag around "Google" inside the h4 tag and then add the word Alphabet beside it, which should not have the strikethrough formatting.

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4><s>Google</s> Alphabet </h4>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte8">8 - Create a Horizontal Line Using the hr Element</a>

You can use the hr tag to add a horizontal line across the width of its containing element. This can be used to define a change in topic or to visually separate groups of content.


Add an hr tag underneath the h4 which contains the card title.

Note
In HTML, hr is a self-closing tag, and therefore doesn't need a separate closing tag.

```html
<style>
  h4 {
    text-align: center;
    height: 25px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4><s>Google</s>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Adjust the background-color Property of Text</a>

Instead of adjusting your overall background or the color of the text to make the foreground easily readable, you can add a background-color to the element holding the text you want to emphasize. This challenge uses rgba() instead of hex codes or normal rgb().

rgba stands for:
  r = red
  g = green
  b = blue
  a = alpha/level of opacity
The RGB values can range from 0 to 255. The alpha value can range from 1, which is fully opaque or a solid color, to 0, which is fully transparent or clear. rgba() is great to use in this case, as it allows you to adjust the opacity. This means you don't have to completely block out the background.

You'll use background-color: rgba(45, 45, 45, 0.1) for this challenge. It produces a dark gray color that is nearly transparent given the low opacity value of 0.1.


To make the text stand out more, adjust the background-color of the h4 element to the given rgba() value.

Also for the h4, remove the height property and add padding of 10px.

```html
<style>
  h4 {
    text-align: center;
    background-color:rgba(45, 45, 45, 0.1);
    padding:10px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```


[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Adjust the Size of a Header Versus a Paragraph Tag</a>

The font size of header tags (h1 through h6) should generally be larger than the font size of paragraph tags. This makes it easier for the user to visually understand the layout and level of importance of everything on the page. You use the font-size property to adjust the size of the text in an element.


To make the heading significantly larger than the paragraph, change the font-size of the h4 tag to 27 pixels.

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size:27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Add a box-shadow to a Card-like Element</a>

The box-shadow property applies one or more shadows to an element.

The box-shadow property takes values for offset-x (how far to push the shadow horizontally from the element), offset-y (how far to push the shadow vertically from the element), blur-radius, spread-radius and a color value, in that order. The blur-radius and spread-radius values are optional.

Here's an example of the CSS to create multiple shadows with some blur, at mostly-transparent black colors:

box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);

The element now has an id of thumbnail. With this selector, use the example CSS values above to place a box-shadow on the card.

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
  }
  
  #thumbnail{
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
  
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte12">12 - Decrease the Opacity of an Element</a>

The opacity property in CSS is used to adjust the opacity, or conversely, the transparency for an item.

```
A value of 1 is opaque, which isn't transparent at all.
A value of 0.5 is half see-through.
A value of 0 is completely transparent.
```

The value given will apply to the entire element, whether that's an image with some transparency, or the foreground and background colors for a block of text.


Set the opacity of the anchor tags to 0.7 using links class to select them.

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
    opacity:0.7;
  }
  #thumbnail {
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte13">13 - Use the text-transform Property to Make Text Uppercase</a>

The text-transform property in CSS is used to change the appearance of text. It's a convenient way to make sure text on a webpage appears consistently, without having to change the text content of the actual HTML elements.

The following table shows how the different text-transformvalues change the example text "Transform me".

| Value | Result |
|---|---|
|  lowercase |  "transform me" |
|  uppercase |  "TRANSFORM ME" |
|  capitalize |  "Transform Me" |
|  initial | Use the default value  |
|  inherit | Use the text-transform value from the parent element  |
|  none | Default: Use the original text  |

```html
<style>
  h4 {
    text-align: center;
    background-color: rgba(45, 45, 45, 0.1);
    padding: 10px;
    font-size: 27px;
    text-transform:uppercase;
  }
  p {
    text-align: justify;
  }
  .links {
    text-align: left;
    color: black;
    opacity: 0.7;
  }
  #thumbnail {
    box-shadow: 0 10px 20px rgba(0,0,0,0.19), 0 6px 6px rgba(0,0,0,0.23);
  }
  .fullCard {
    width: 245px;
    border: 1px solid #ccc;
    border-radius: 5px;
    margin: 10px 5px;
    padding: 4px;
  }
  .cardContent {
    padding: 10px;
  }
  .cardText {
    margin-bottom: 30px;
  }
</style>
<div class="fullCard" id="thumbnail">
  <div class="cardContent">
    <div class="cardText">
      <h4>Alphabet</h4>
      <hr>
      <p><em>Google was founded by Larry Page and Sergey Brin while they were <u>Ph.D. students</u> at <strong>Stanford University</strong>.</em></p>
    </div>
    <div class="cardLinks">
      <a href="https://en.wikipedia.org/wiki/Larry_Page" target="_blank" class="links">Larry Page</a><br><br>
      <a href="https://en.wikipedia.org/wiki/Sergey_Brin" target="_blank" class="links">Sergey Brin</a>
    </div>
  </div>
</div>
```



[Voltar ao Índice](#indice)

---


## <a name="parte14">14 - Set the font-size for Multiple Heading Elements</a>

The font-size property is used to specify how large the text is in a given element. This rule can be used for multiple elements to create visual consistency of text on a page. In this challenge, you'll set the values for all h1 through h6 tags to balance the heading sizes.

```
Set the font-size of the h1 tag to 68px.
Set the font-size of the h2 tag to 52px.
Set the font-size of the h3 tag to 40px.
Set the font-size of the h4 tag to 32px.
Set the font-size of the h5 tag to 21px.
Set the font-size of the h6 tag to 14px.
```

```html
<style>
  h1{
    font-size:68px;
  }
  h2{
    font-size:52px;
  }
  h3{
    font-size:40px;
  }
  h4{
    font-size:32px;
  }
  h5{
    font-size:21px;
  }
  h6{
    font-size:14px;
  }
</style>
<h1>This is h1 text</h1>
<h2>This is h2 text</h2>
<h3>This is h3 text</h3>
<h4>This is h4 text</h4>
<h5>This is h5 text</h5>
<h6>This is h6 text</h6>
```

[Voltar ao Índice](#indice)

---


## <a name="parte15">15 - Set the font-weight for Multiple Heading Elements</a>

You set the font-size of each heading tag in the last challenge, here you'll adjust the font-weight.

The font-weight property sets how thick or thin characters are in a section of text.

```
Set the font-weight of the h1 tag to 800.
Set the font-weight of the h2 tag to 600.
Set the font-weight of the h3 tag to 500.
Set the font-weight of the h4 tag to 400.
Set the font-weight of the h5 tag to 300.
Set the font-weight of the h6 tag to 200.
```

```html
<style>
  h1 {
    font-size: 68px;
    font-weight:800 ;
  }
  h2 {
    font-size: 52px;
    font-weight:600 ;
  }
  h3 {
    font-size: 40px;
    font-weight:500 ;
  }
  h4 {
    font-size: 32px;
    font-weight:400 ;
  }
  h5 {
    font-size: 21px;
    font-weight:300 ;
  }
  h6 {
    font-size: 14px;
    font-weight:200 ;
  }
</style>
<h1>This is h1 text</h1>
<h2>This is h2 text</h2>
<h3>This is h3 text</h3>
<h4>This is h4 text</h4>
<h5>This is h5 text</h5>
<h6>This is h6 text</h6>
```


[Voltar ao Índice](#indice)

---


## <a name="parte16">16 - Set the font-size of Paragraph Text</a>

The font-size property in CSS is not limited to headings, it can be applied to any element containing text.


Change the value of the font-size property for the paragraph to 16px to make it more visible.

```html
<style>
  p {
    font-size: 16px;
  }
</style>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
```


[Voltar ao Índice](#indice)

---


## <a name="parte17">17 - Set the line-height of Paragraphs</a>

CSS offers the line-height property to change the height of each line in a block of text. As the name suggests, it changes the amount of vertical space that each line of text gets.


Add a line-height property to the p tag and set it to 25px.


```html
<style>
  p {
    font-size: 16px;
    line-height:25px ;
  }
</style>
<p>
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
```

[Voltar ao Índice](#indice)

---


## <a name="parte18">18 - Adjust the Hover State of an Anchor Tag</a>

This challenge will touch on the usage of pseudo-classes. A pseudo-class is a keyword that can be added to selectors, in order to select a specific state of the element.

For example, the styling of an anchor tag can be changed for its hover state using the :hover pseudo-class selector. Here's the CSS to change the color of the anchor tag to red during its hover state:

```css
a:hover {
  color: red;
}
```

The code editor has a CSS rule to style all a tags black. Add a rule so that when the user hovers over the a tag, the color is blue.

```html
<style>
  a {
    color: #000;
  }
  a:hover{
    color:blue;
  }
  
  
  
</style>
<a href="http://freecatphotoapp.com/" target="_blank">CatPhotoApp</a>
```


[Voltar ao Índice](#indice)

---


## <a name="parte19">19 - Change an Element's Relative Position</a>

CSS treats each HTML element as its own box, which is usually referred to as the CSS Box Model. Block-level items automatically start on a new line (think headings, paragraphs, and divs) while inline items sit within surrounding content (like images or spans). The default layout of elements in this way is called the normal flow of a document, but CSS offers the position property to override it.

When the position of an element is set to relative, it allows you to specify how CSS should move it relative to its current position in the normal flow of the page. It pairs with the CSS offset properties of left or right, and top or bottom. These say how many pixels, percentages, or ems to move the item away from where it is normally positioned. The following example moves the paragraph 10 pixels away from the bottom:

p {
  position: relative;
  bottom: 10px;
}
Changing an element's position to relative does not remove it from the normal flow - other elements around it still behave as if that item were in its default position.

Note
Positioning gives you a lot of flexibility and power over the visual layout of a page. It's good to remember that no matter the position of elements, the underlying HTML markup should be organized and make sense when read from top to bottom. This is how users with visual impairments (who rely on assistive devices like screen readers) access your content.


Change the position of the h2 to relative, and use a CSS offset to move it 15 pixels away from the top of where it sits in the normal flow. Notice there is no impact on the positions of the surrounding h1 and p elements.

```html
<style>
  h2 {
    position: relative;
    top:15px;
  }
</style>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```

[Voltar ao Índice](#indice)

---


## <a name="parte20">20 - Move a Relatively Positioned Element with CSS Offsets</a>

The CSS offsets of top or bottom, and left or right tell the browser how far to offset an item relative to where it would sit in the normal flow of the document. You're offsetting an element away from a given spot, which moves the element away from the referenced side (effectively, the opposite direction). As you saw in the last challenge, using the top offset moved the h2 downwards. Likewise, using a left offset moves an item to the right.

![](https://i.imgur.com/eWWi3gZ.gif)

Use CSS offsets to move the h2 15 pixels to the right and 10 pixels up.

```html
<head>
<style>
  h2 {
    position: relative;
    right:-15px;
    top:-10px;
  }
</style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```

[Voltar ao Índice](#indice)

---


## <a name="parte21">21 - Lock an Element to its Parent with Absolute Positioning</a>

The next option for the CSS position property is absolute, which locks the element in place relative to its parent container. Unlike the relative position, this removes the element from the normal flow of the document, so surrounding items ignore it. The CSS offset properties (top or bottom and left or right) are used to adjust the position.

One nuance with absolute positioning is that it will be locked relative to its closest positioned ancestor. If you forget to add a position rule to the parent item, (this is typically done using position: relative;), the browser will keep looking up the chain and ultimately default to the body tag.


Lock the #searchbar element to the top-right of its section parent by declaring its position as absolute. Give it top and right offsets of 50 pixels each.

```html
<style>
  #searchbar {
    
    position:absolute;
    top:50px;
    right:50px;
    
  }
  section {
    position: relative;
  }
</style>
<body>
  <h1>Welcome!</h1>
  <section>
    <form id="searchbar">
      <label for="search">Search:</label>
      <input type="search" id="search" name="search">
      <input type="submit" name="submit" value="Go!">
    </form>
  </section>
</body>
```

[Voltar ao Índice](#indice)

---


## <a name="parte22">22 - Lock an Element to the Browser Window with Fixed Positioning</a>

The next layout scheme that CSS offers is the fixed position, which is a type of absolute positioning that locks an element relative to the browser window. Similar to absolute positioning, it's used with the CSS offset properties and also removes the element from the normal flow of the document. Other items no longer "realize" where it is positioned, which may require some layout adjustments elsewhere.

One key difference between the fixed and absolute positions is that an element with a fixed position won't move when the user scrolls.


The navigation bar in the code is labeled with an id of navbar. Change its position to fixed, and offset it 0 pixels from the top and 0 pixels from the left. Notice the (lack of) impact to the h1 position, it hasn't been pushed down to accommodate the navigation bar and would need to be adjusted separately.

```html
<style>
  #navbar {
    position:fixed;
    top:0px;
    left:0px;
    width: 100%;
    background-color: #767676;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
  }
</style>
<body>
  <header>
    <h1>Welcome!</h1>
    <nav id="navbar">
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Contact</a></li>
      </ul>
    </nav>
  </header>
  <p>I shift up when the #navbar is fixed to the browser window.</p>
</body>
```

[Voltar ao Índice](#indice)

---


## <a name="parte23">23 - Push Elements Left or Right with the float Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte24">24 - Change the Position of Overlapping Elements with the z-index Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte25">25 - Center an Element Horizontally Using the margin Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte26">26 - Learn about Complementary Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte27">27 - Learn about Tertiary Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte28">28 - Adjust the Color of Various Elements to Complementary Colors</a>



[Voltar ao Índice](#indice)

---


## <a name="parte29">29 - Adjust the Hue of a Color</a>



[Voltar ao Índice](#indice)

---


## <a name="parte30">30 - Adjust the Tone of a Color</a>



[Voltar ao Índice](#indice)

---


## <a name="parte31">31 - Create a Gradual CSS Linear Gradient</a>



[Voltar ao Índice](#indice)

---


## <a name="parte32">32 - Use a CSS Linear Gradient to Create a Striped Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte33">33 - Create Texture by Adding a Subtle Pattern as a Background Image</a>



[Voltar ao Índice](#indice)

---


## <a name="parte34">34 - Use the CSS Transform scale Property to Change the Size of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte35">35 - Use the CSS Transform scale Property to Scale an Element on Hover</a>



[Voltar ao Índice](#indice)

---


## <a name="parte36">36 - Use the CSS Transform Property skewX to Skew an Element Along the X-Axis</a>



[Voltar ao Índice](#indice)

---


## <a name="parte37">37 - Use the CSS Transform Property skewY to Skew an Element Along the Y-Axis</a>



[Voltar ao Índice](#indice)

---


## <a name="parte38">38 - Create a Graphic Using CSS</a>



[Voltar ao Índice](#indice)

---


## <a name="parte39">39 - Create a More Complex Shape Using CSS and HTML</a>



[Voltar ao Índice](#indice)

---


## <a name="parte40">40 - Learn How the CSS @keyframes and animation Properties Work</a>



[Voltar ao Índice](#indice)

---


## <a name="parte41">41 - Use CSS Animation to Change the Hover State of a Button</a>



[Voltar ao Índice](#indice)

---


## <a name="parte42">42 - Modify Fill Mode of an Animation</a>



[Voltar ao Índice](#indice)

---


## <a name="parte43">43 - Create Movement Using CSS Animation</a>



[Voltar ao Índice](#indice)

---


## <a name="parte44">44 - Create Visual Direction by Fading an Element from Left to Right</a>



[Voltar ao Índice](#indice)

---


## <a name="parte45">45 - Animate Elements Continually Using an Infinite Animation Count</a>



[Voltar ao Índice](#indice)

---


## <a name="parte46">46 - Make a CSS Heartbeat using an Infinite Animation Count</a>



[Voltar ao Índice](#indice)

---


## <a name="parte47">47 - Animate Elements at Variable Rates</a>



[Voltar ao Índice](#indice)

---


## <a name="parte48">48 - Animate Multiple Elements at Variable Rates</a>



[Voltar ao Índice](#indice)

---


## <a name="parte49">49 - Change Animation Timing with Keywords</a>



[Voltar ao Índice](#indice)

---


## <a name="parte50">50 - Learn How Bezier Curves Work</a>



[Voltar ao Índice](#indice)

---


## <a name="parte51">51 - Use a Bezier Curve to Move a Graphic</a>



[Voltar ao Índice](#indice)

---


## <a name="parte52">52 - Make Motion More Natural Using a Bezier Curve</a>



[Voltar ao Índice](#indice)

---


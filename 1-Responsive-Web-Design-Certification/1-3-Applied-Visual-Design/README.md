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

The next positioning tool does not actually use position, but sets the float property of an element. Floating elements are removed from the normal flow of a document and pushed to either the left or right of their containing parent element. It's commonly used with the width property to specify how much horizontal space the floated element requires.


The given markup would work well as a two-column layout, with the section and aside elements next to each other. Give the #left item a float of left and the #right item a float of right.

```html
<head>
  <style>
  #left {
    float:left;
    width: 50%;
  }
  #right {
    float:right;
    width: 40%;
  }
  aside, section {
    padding: 2px;
    background-color: #ccc;
  }
  </style>
</head>
<body>
  <header>
    <h1>Welcome!</h1>
  </header>
  <section id="left">
    <h2>Content</h2>
    <p>Good stuff</p>
  </section>
  <aside id="right">
    <h2>Sidebar</h2>
    <p>Links</p>
  </aside>
</body>
```



[Voltar ao Índice](#indice)

---


## <a name="parte24">24 - Change the Position of Overlapping Elements with the z-index Property</a>

When elements are positioned to overlap, the element coming later in the HTML markup will, by default, appear on the top of the other elements. However, the z-index property can specify the order of how elements are stacked on top of one another. It must be an integer (i.e. a whole number and not a decimal), and higher values for the z-index property of an element move it higher in the stack than those with lower values.


Add a z-index property to the element with the class name of first (the red rectangle) and set it to a value of 2 so it covers the other element (blue rectangle).

```html
<style>
  div {
    width: 60%;
    height: 200px;
    margin-top: 20px;
  }
  
  .first {
    background-color: red;
    position: absolute;
    z-index:2;
  }
  .second {
    background-color: blue;
    position: absolute;
    left: 40px;
    top: 50px;
    z-index: 1;
  }
</style>

<div class="first"></div>
<div class="second"></div>
```



[Voltar ao Índice](#indice)

---


## <a name="parte25">25 - Center an Element Horizontally Using the margin Property</a>

Another positioning technique is to center a block element horizontally. One way to do this is to set its margin to a value of auto.

This method works for images, too. Images are inline elements by default, but can be changed to block elements when you set the display property to block.


Center the div on the page by adding a margin property with a value of auto.

```html
<style>
  div {
    background-color: blue;
    height: 100px;
    width: 100px;
    margin:auto;
  }
</style>
<div></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte26">26 - Learn about Complementary Colors</a>

Color theory and its impact on design is a deep topic and only the basics are covered in the following challenges. On a website, color can draw attention to content, evoke emotions, or create visual harmony. Using different combinations of colors can really change the look of a website, and a lot of thought can go into picking a color palette that works with your content.

The color wheel is a useful tool to visualize how colors relate to each other - it's a circle where similar hues are neighbors and different hues are farther apart. When two colors are opposite each other on the wheel, they are called complementary colors. They have the characteristic that if they are combined, they "cancel" each other out and create a gray color. However, when placed side-by-side, these colors appear more vibrant and produce a strong visual contrast.

Some examples of complementary colors with their hex codes are:

```
red (#FF0000) and cyan (#00FFFF)
green (#00FF00) and magenta (#FF00FF)
blue (#0000FF) and yellow (#FFFF00)
```

This is different than the outdated RYB color model that many of us were taught in school, which has different primary and complementary colors. Modern color theory uses the additive RGB model (like on a computer screen) and the subtractive CMY(K) model (like in printing). Read here for more information on this complex subject.

There are many color picking tools available online that have an option to find the complement of a color.

Note
For all color challenges: Using color can be a powerful way to add visual interest to a page. However, color alone should not be used as the only way to convey important information because users with visual impairments may not understand that content. This issue will be covered in more detail in the Applied Accessibility challenges.


Change the background-color property of the blue and yellow classes to their respective colors. Notice how the colors look different next to each other than they do compared against the white background.

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  .blue {
    background-color: #0000FF;
  }
  .yellow {
    background-color: #FFFF00;
  }
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="blue"></div>
<div class="yellow"></div>
```

[Voltar ao Índice](#indice)

---

## <a name="parte27">27 - Learn about Tertiary Colors</a>

Computer monitors and device screens create different colors by combining amounts of red, green, and blue light. This is known as the RGB additive color model in modern color theory. Red (R), green (G), and blue (B) are called primary colors. Mixing two primary colors creates the secondary colors cyan (G + B), magenta (R + B) and yellow (R + G). You saw these colors in the Complementary Colors challenge. These secondary colors happen to be the complement to the primary color not used in their creation, and are opposite to that primary color on the color wheel. For example, magenta is made with red and blue, and is the complement to green.

Tertiary colors are the result of combining a primary color with one of its secondary color neighbors. For example, red (primary) and yellow (secondary) make orange. This adds six more colors to a simple color wheel for a total of twelve.

There are various methods of selecting different colors that result in a harmonious combination in design. One example that can use tertiary colors is called the split-complementary color scheme. This scheme starts with a base color, then pairs it with the two colors that are adjacent to its complement. The three colors provide strong visual contrast in a design, but are more subtle than using two complementary colors.

Here are three colors created using the split-complement scheme:

| Color |  Hex Code  |
|---|---|
| orange | #FF7D00  |
| cyan  |  #00FFFF |
| raspberry  |  #FF007D |


Change the background-color property of the orange, cyan, and raspberry classes to their respective colors. Make sure to use the hex codes as orange and raspberry are not browser-recognized color names.

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  
  .orange {
    background-color: #FF7D00;
  }
  
  .cyan {
    background-color: #00FFFF;
  }
  
  .raspberry {
    background-color: #FF007D;
  }
  
  div {
    height: 100px;
    width: 100px;
    margin-bottom: 5px;
  }
</style>
  
<div class="orange"></div>
<div class="cyan"></div>
<div class="raspberry"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte28">28 - Adjust the Color of Various Elements to Complementary Colors</a>

The Complementary Colors challenge showed that opposite colors on the color wheel can make each other appear more vibrant when placed side-by-side. However, the strong visual contrast can be jarring if it's overused on a website, and can sometimes make text harder to read if it's placed on a complementary-colored background. In practice, one of the colors is usually dominant and the complement is used to bring visual attention to certain content on the page.


This page will use a shade of teal (#09A7A1) as the dominant color, and its orange (#FF790E) complement to visually highlight the sign-up buttons. Change the background-color of both the header and footer from black to the teal color. Then change the h2 text color to teal as well. Finally, change the background-color of the button to the orange color.

```html
<style>
  body {
    background-color: white;
  }
  header {
    background-color: #09A7A1;
    color: white;
    padding: 0.25em;
  }
  h2 {
    color: #09A7A1;
  }  
  button {
    background-color: #FF790E;
  }
  footer {
    background-color: #09A7A1;
    color: white;
    padding: 0.5em;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
</header>
<main>
  <article>
    <h2>Machine Learning in the Kitchen</h2>
    <p>Join this two day workshop that walks through how to implement cutting-edge snack-getting algorithms with a command line interface. Coding usually involves writing exact instructions, but sometimes you need your computer to execute flexible commands, like <code>fetch Pringles</code>.</p>
    <button>Sign Up</button>
  </article>
  <article>
    <h2>Bisection Vegetable Chopping</h2>
    <p>This week-long retreat will level-up your coding ninja skills to actual ninja skills. No longer is the humble bisection search limited to sorted arrays or coding interview questions, applying its concepts in the kitchen will have you chopping carrots in O(log n) time before you know it.</p>
    <button>Sign Up</button>
  </article>
</main>
<br>
<footer>&copy; 2018 FCC Kitchen</footer>
```

[Voltar ao Índice](#indice)

---


## <a name="parte29">29 - Adjust the Hue of a Color</a>

Colors have several characteristics including hue, saturation, and lightness. CSS3 introduced the hsl() property as an alternative way to pick a color by directly stating these characteristics.

Hue is what people generally think of as 'color'. If you picture a spectrum of colors starting with red on the left, moving through green in the middle, and blue on right, the hue is where a color fits along this line. In hsl(), hue uses a color wheel concept instead of the spectrum, where the angle of the color on the circle is given as a value between 0 and 360.

Saturation is the amount of gray in a color. A fully saturated color has no gray in it, and a minimally saturated color is almost completely gray. This is given as a percentage with 100% being fully saturated.

Lightness is the amount of white or black in a color. A percentage is given ranging from 0% (black) to 100% (white), where 50% is the normal color.

Here are a few examples of using hsl() with fully-saturated, normal lightness colors:

| Color  | HSL  |
|---|---|
| red  |  hsl(0, 100%, 50%) |
| yellow |  hsl(60, 100%, 50%) |
| green  | hsl(120, 100%, 50%)  |
| cyan  | hsl(180, 100%, 50%)  |
| blue  | hsl(240, 100%, 50%)  |
| magenta  | hsl(300, 100%, 50%)  |

Change the background-color of each div element based on the class names (green, cyan, or blue) using hsl(). All three should have full saturation and normal lightness.


```html
<style>
  body {
    background-color: #FFFFFF;
  }
  
  .green {
    background-color: hsl(120, 100%, 50%);
  }
  
  .cyan {
    background-color: hsl(180, 100%, 50%);
  }
  
  .blue {
    background-color: hsl(240, 100%, 50%);
  }
  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
  
<div class="green"></div>
<div class="cyan"></div>
<div class="blue"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte30">30 - Adjust the Tone of a Color</a>

The hsl() option in CSS also makes it easy to adjust the tone of a color. Mixing white with a pure hue creates a tint of that color, and adding black will make a shade. Alternatively, a tone is produced by adding gray or by both tinting and shading. Recall that the 's' and 'l' of hsl() stand for saturation and lightness, respectively. The saturation percent changes the amount of gray and the lightness percent determines how much white or black is in the color. This is useful when you have a base hue you like, but need different variations of it.


The navigation bar on this site currently inherits its background-color from the header element. Starting with that color as a base, add a background-color to the nav element so it uses the same cyan hue, but has 80% saturation and 25% lightness values to change its tone and shade.

```html
<style>
  header {
    background-color: hsl(180, 90%, 35%);
    color: #FFFFFF;
  }
  
  nav {
  background-color:hsl(180, 80%, 25%);
  }
  
  h1 {
    text-indent: 10px;
    padding-top: 10px;
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
    color: inherit;
  }
</style>
  
<header>
  <h1>Cooking with FCC!</h1>
  <nav>
    <ul>
      <li><a href="">Home</a></li>
      <li><a href="">Classes</a></li>
      <li><a href="">Contact</a></li>
    </ul>
  </nav>
</header>
```

[Voltar ao Índice](#indice)

---


## <a name="parte31">31 - Create a Gradual CSS Linear Gradient</a>

Applying a color on HTML elements is not limited to one flat hue. CSS provides the ability to use color transitions, otherwise known as gradients, on elements. This is accessed through the background property's linear-gradient() function. Here is the general syntax:

```css
    background: linear-gradient(gradient_direction, color 1, color 2, color 3, ...);
```

The first argument specifies the direction from which color transition starts - it can be stated as a degree, where 90deg makes a vertical gradient and 45deg is angled like a backslash. The following arguments specify the order of colors used in the gradient.

Example:

```css
    background: linear-gradient(90deg, red, yellow, rgb(204, 204, 255));
```

Use a linear-gradient() for the div element's background, and set it from a direction of 35 degrees to change the color from #CCFFFF to #FFCCCC.

Note  
While there are other ways to specify a color value, like rgb() or hsl(), use hex values for this challenge.

```html
<style>

  div{ 
    border-radius: 20px;
    width: 70%;
    height: 400px;
    margin: 50px auto;
    background: linear-gradient(35deg, #CCFFFF, #FFCCCC);
  }

</style>

<div></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte32">32 - Use a CSS Linear Gradient to Create a Striped Element</a>

The repeating-linear-gradient() function is very similar to linear-gradient() with the major difference that it repeats the specified gradient pattern. repeating-linear-gradient() accepts a variety of values, but for simplicity, you'll work with an angle value and color stop values in this challenge.

The angle value is the direction of the gradient. Color stops are like width values that mark where a transition takes place, and are given with a percentage or a number of pixels.

In the example demonstrated in the code editor, the gradient starts with the color yellow at 0 pixels which blends into the second color blue at 40 pixels away from the start. Since the next color stop is also at 40 pixels, the gradient immediately changes to the third color green, which itself blends into the fourth color value red as that is 80 pixels away from the beginning of the gradient.

For this example, it helps to think about the color stops as pairs where every two colors blend together.

```css
    0px [yellow -- blend -- blue] 40px [green -- blend -- red] 80px
```

If every two color stop values are the same color, the blending isn't noticeable because it's between the same color, followed by a hard transition to the next color, so you end up with stripes.


Make stripes by changing the repeating-linear-gradient() to use a gradient angle of 45deg, then set the first two color stops to yellow, and finally the second two color stops to black.

```html
 <style>
 
   div{ 
     border-radius: 20px;
     width: 70%;
     height: 400px;
     margin:  50 auto;
     background: repeating-linear-gradient(
       45deg,
       yellow 0px,
       yellow 40px,
       black 40px,
       black 80px
     );
   }
 
 </style>
 
 <div></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte33">33 - Create Texture by Adding a Subtle Pattern as a Background Image</a>

One way to add texture and interest to a background and have it stand out more is to add a subtle pattern. The key is balance, as you don't want the background to stand out too much, and take away from the foreground. The background property supports the url() function in order to link to an image of the chosen texture or pattern. The link address is wrapped in quotes inside the parentheses.


Using the url of https://i.imgur.com/MJAkxbh.png, set the background of the whole page with the body selector.

```html
<style>
  body {
    background: url(https://i.imgur.com/MJAkxbh.png);
  }
</style>
```

[Voltar ao Índice](#indice)

---


## <a name="parte34">34 - Use the CSS Transform scale Property to Change the Size of an Element</a>

To change the scale of an element, CSS has the transform property, along with its scale() function. The following code example doubles the size of all the paragraph elements on the page:

```css
    p {
      transform:scale(2);
    }
```

Increase the size of the element with the id of ball2 to 1.5 times its original size.

```html
<style>
  .ball { 
    width: 40px;
    height: 40px;
    margin: 50 auto;
    position: fixed;
    background: linear-gradient(
      35deg,
      #ccffff,
      #ffcccc
    );
    border-radius: 50%;
  }
  #ball1 {
    left: 20%;
  }
  #ball2 {
    left: 65%;
    transform:scale(1.5);
  }


</style>

<div class="ball" id= "ball1"></div>
<div class="ball" id= "ball2"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte35">35 - Use the CSS Transform scale Property to Scale an Element on Hover</a>

The transform property has a variety of functions that lets you scale, move, rotate, skew, etc., your elements. When used with pseudo-classes such as :hover that specify a certain state of an element, the transform property can easily add interactivity to your elements.

Here's an example to scale the paragraph elements to 2.1 times their original size when a user hovers over them:

```css
    p:hover {
      transform: scale(2.1);
    }
```

Add a CSS rule for the hover state of the div and use the transform property to scale the div element to 1.1 times its original size when a user hovers over it.

```html
<style>
  div { 
    width: 70%;
    height: 100px;
    margin:  50px auto;
    background: linear-gradient(
      53deg,
      #ccfffc,
      #ffcccf
    );
  }
  div:hover{
    transform: scale(1.1);
  }
  
  
</style>

<div></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte36">36 - Use the CSS Transform Property skewX to Skew an Element Along the X-Axis</a>

The next function of the transform property is skewX(), which skews the selected element along its X (horizontal) axis by a given degree.

The following code skews the paragraph element by -32 degrees along the X-axis.

```css
    p {
      transform: skewX(-32deg);
    }
```

Skew the element with the id of bottom by 24 degrees along the X-axis by using the transform property.

```html
<style>
  div { 
    width: 70%;
    height: 100px;
    margin:  50px auto;
  }
  #top {
    background-color: red;
  }
  #bottom {
    background-color: blue;
    transform: skewX(24deg);
  }
</style>

<div id="top"></div>
<div id="bottom"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte37">37 - Use the CSS Transform Property skewY to Skew an Element Along the Y-Axis</a>

Given that the skewX() function skews the selected element along the X-axis by a given degree, it is no surprise that the skewY() property skews an element along the Y (vertical) axis.


Skew the element with the id of top -10 degrees along the Y-axis by using the transform property.

```html
<style>
  div { 
    width: 70%;
    height: 100px;
    margin: 50px auto;
  }
  #top {
    background-color: red;
    transform: skewY(-10deg);
  }
  #bottom {
    background-color: blue;
    transform: skewX(24deg);
  }
</style>

<div id="top"></div>
<div id="bottom"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte38">38 - Create a Graphic Using CSS</a>

By manipulating different selectors and properties, you can make interesting shapes. One of the easier ones to try is a crescent moon shape. For this challenge you need to work with the box-shadow property that sets the shadow of an element, along with the border-radius property that controls the roundness of the element's corners.

You will create a round, transparent object with a crisp shadow that is slightly offset to the side - the shadow is actually going to be the moon shape you see.

In order to create a round object, the border-radius property should be set to a value of 50%.

You may recall from an earlier challenge that the box-shadow property takes values for offset-x, offset-y, blur-radius, spread-radius and a color value in that order. The blur-radius and spread-radius values are optional.


Manipulate the square element in the editor to create the moon shape. First, change the background-color to transparent, then set the border-radius property to 50% to make the circular shape. Finally, change the box-shadow property to set the offset-x to 25px, the offset-y to 10px, blur-radius to 0, spread-radius to 0, and color to blue.

```html
<style>
.center
{
  position: absolute;
  margin: auto;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  width: 100px;
  height: 100px;
  
  background-color: transparent;
  border-radius: 50%;
  box-shadow: 25px 10px 0px 0px blue; 
}

</style>
<div class="center"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte39">39 - Create a More Complex Shape Using CSS and HTML</a>

One of the most popular shapes in the world is the heart shape, and in this challenge you'll create one using pure CSS. But first, you need to understand the ::before and ::after pseudo-elements. These pseudo-elements are used to add something before or after a selected element. In the following example, a ::before pseudo-element is used to add a rectangle to an element with the class heart:

```css
    .heart::before {
      content: "";
      background-color: yellow;
      border-radius: 25%;
      position: absolute;
      height: 50px;
      width: 70px;
      top: -50px;
      left: 5px;
    }

```
For the ::before and ::after pseudo-elements to function properly, they must have a defined content property. This property is usually used to add things like a photo or text to the selected element. When the ::before and ::after pseudo-elements are used to make shapes, the content property is still required, but it's set to an empty string.

In the above example, the element with the class of heart has a ::before pseudo-element that produces a yellow rectangle with height and width of 50px and 70px, respectively. This rectangle has round corners due to its 25% border radius and is positioned absolutely at 5px from the left and 50px above the top of the element.


Transform the element on the screen to a heart. In the heart::after selector, change the background-color to pink and the border-radius to 50%.

Next, target the element with the class heart (just heart) and fill in the transform property. Use the rotate() function with -45 degrees. (rotate() works the same way that skewX() and skewY() do).

Finally, in the heart::before selector, set its content property to an empty string.

```html
<style>
.heart {
  position: absolute;
  margin: auto;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  background-color: pink;
  height: 50px;
  width: 50px;
  transform: rotate(-45deg);
}
.heart::after {
  background-color: pink;
  content: "";
  border-radius: 50%;
  position: absolute;
  width: 50px;
  height: 50px;
  top: 0px;
  left: 25px;
}
.heart::before {
  content: "";
  background-color: pink;
  border-radius: 50%;
  position: absolute;
  width: 50px;
  height: 50px;
  top: -25px;
  left: 0px;
}
</style>
<div class = "heart"></div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte40">40 - Learn How the CSS @keyframes and animation Properties Work</a>

To animate an element, you need to know about the animation properties and the @keyframes rule. The animation properties control how the animation should behave and the @keyframes rule controls what happens during that animation. There are eight animation properties in total. This challenge will keep it simple and cover the two most important ones first:

animation-name sets the name of the animation, which is later used by @keyframes to tell CSS which rules go with which animations.

animation-duration sets the length of time for the animation.

@keyframes is how to specify exactly what happens within the animation over the duration. This is done by giving CSS properties for specific "frames" during the animation, with percentages ranging from 0% to 100%. If you compare this to a movie, the CSS properties for 0% is how the element displays in the opening scene. The CSS properties for 100% is how the element appears at the end, right before the credits roll. Then CSS applies the magic to transition the element over the given duration to act out the scene. Here's an example to illustrate the usage of @keyframes and the animation properties:

```css
    #anim {
      animation-name: colorful;
      animation-duration: 3s;
    }
    @keyframes colorful {
      0% {
        background-color: blue;
      }
      100% {
        background-color: yellow;
      }
    }

```
For the element with the anim id, the code snippet above sets the animation-name to colorful and sets the animation-duration to 3 seconds. Then the @keyframes rule links to the animation properties with the name colorful. It sets the color to blue at the beginning of the animation (0%) which will transition to yellow by the end of the animation (100%). You aren't limited to only beginning-end transitions, you can set properties for the element for any percentage between 0% and 100%.


Create an animation for the element with the id rect, by setting the animation-name to rainbow and the animation-duration to 4 seconds. Next, declare a @keyframes rule, and set the background-color at the beginning of the animation (0%) to blue, the middle of the animation (50%) to green, and the end of the animation (100%) to yellow.

```html
<style>
  div {
    height: 40px;
    width: 70%;
    background: black;
    margin: 50px auto;
    border-radius: 5px;
  }

  #rect {
  animation-name: rainbow ;
  animation-duration: 4s;
  }
  @keyframes rainbow  {
  0% {
    background-color: blue;
  }
  50% {
    background-color: green;
  }
  100% {
    background-color: yellow;
  }
}
  
  
  
  
</style>
<div id="rect"></div>


```

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


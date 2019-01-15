# Introduction to the Responsive Web Design Challenges

https://learn.freecodecamp.org/responsive-web-design/responsive-web-design-principles

Today, there are many types of devices that can access the web. They range from large desktop computers to small mobile phones. These devices have different screen sizes, resolutions, and processing power. Responsive Web Design is an approach to designing web content that responds to the constraints of different devices. 

## <a name="indice">Índice</a>

1. [Create a Media Query](#parte1)     
2. [Make an Image Responsive](#parte2)     
3. [Use a Retina Image for Higher Resolution Displays](#parte3)     
4. [Make Typography Responsive](#parte4)     
---


## <a name="parte1">1 - Create a Media Query</a>

Media Queries are a new technique introduced in CSS3 that change the presentation of content based on different viewport sizes. The viewport is a user's visible area of a web page, and is different depending on the device used to access the site.

Media Queries consist of a media type, and if that media type matches the type of device the document is displayed on, the styles are applied. You can have as many selectors and styles inside your media query as you want.

Here's an example of a media query that returns the content when the device's width is less than or equal to 100px:

```css
    @media (max-width: 100px) { /* CSS Rules */ }

```

and the following media query returns the content when the device's height is more than or equal to 350px:


```css
    @media (min-height: 350px) { /* CSS Rules */ }
```

Remember, the CSS inside the media query is applied only if the media type matches that of the device being used.

Add a media query, so that the p tag has a font-size of 10px when the device's height is less than or equal to 800px.

```html
<style>
  @media (max-height: 800px) { 
    p {
    font-size: 10px;
  }
   }
  /* Add media query below */
  
</style>
  
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus quis tempus massa. Aenean erat nisl, gravida vel vestibulum cursus, interdum sit amet lectus. Sed sit amet quam nibh. Suspendisse quis tincidunt nulla. In hac habitasse platea dictumst. Ut sit amet pretium nisl. Vivamus vel mi sem. Aenean sit amet consectetur sem. Suspendisse pretium, purus et gravida consequat, nunc ligula ultricies diam, at aliquet velit libero a dui.</p>
```

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Make an Image Responsive</a>

Making images responsive with CSS is actually very simple. Instead of applying an absolute width to an element:

```css
    img { width: 720px; }

```

You can use:
```css
    img {
      max-width: 100%;
      display: block;
      height: auto;
    }

```
The max-width property of 100% scales the image to fit the width of its container, but the image won't stretch wider than its original width. Setting the display property to block changes the image from an inline element (its default), to a block element on its own line. The height property of auto keeps the original aspect ratio of the image.


Add style rules for the img tag to make it responsive to the size of its container. It should display as a block-level element, it should fit the full width of its container without stretching, and it should keep its original aspect ratio.

```html
<style>
  img{
      max-width:100%;
      display:block;
      height:auto;
  }
</style>

<img src="https://s3.amazonaws.com/freecodecamp/FCCStickerPack.jpg" alt="freeCodeCamp stickers set">
```

[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Use a Retina Image for Higher Resolution Displays</a>

The simplest way to make your images appear "retina" (and optimize them for retina displays) is to define their width and height values as only half of what the original file is.

Here is an example of an image that is only using half of the original height and width:

```html
    <style>
      img { height: 250px; width: 250px; }
    </style>
    <img src="coolPic500x500" alt="A most excellent picture">

```

Set the width and height of the img tag to half of their original values. In this case, both the original height and the original width are 200px.

```html
<style>
  img { height: 100px; width: 100px; }
</style>

<img src="https://s3.amazonaws.com/freecodecamp/FCCStickers-CamperBot200x200.jpg" alt="freeCodeCamp sticker that says 'Because CamperBot Cares'">
```

[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Make Typography Responsive</a>

Instead of using em or px to size text, you can use viewport units for responsive typography. Viewport units, like percentages, are relative units, but they are based off different items. Viewport units are relative to the viewport dimensions (width or height) of a device, and percentages are relative to the size of the parent container element.

The four different viewport units are:

- vw: 10vw would be 10% of the viewport's width.
- vh: 3vh would be 3% of the viewport's height.
- vmin: 70vmin would be 70% of the viewport's smaller dimension (height vs. width).
- vmax: 100vmax would be 100% of the viewport's bigger dimension (height vs. width).


Set the width of the h2 tag to 80% of the viewport's width and the width of the paragraph as 75% of the viewport's smaller dimension.


```html
<style>
  h2{
      width:80vw;
  }
  p{
      width:75vmin;
  }
</style>

<h2>Importantus Ipsum</h2>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus quis tempus massa. Aenean erat nisl, gravida vel vestibulum cursus, interdum sit amet lectus. Sed sit amet quam nibh. Suspendisse quis tincidunt nulla. In hac habitasse platea dictumst. Ut sit amet pretium nisl. Vivamus vel mi sem. Aenean sit amet consectetur sem. Suspendisse pretium, purus et gravida consequat, nunc ligula ultricies diam, at aliquet velit libero a dui.</p>
```

[Voltar ao Índice](#indice)

---


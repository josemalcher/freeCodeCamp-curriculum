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



[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Use a Retina Image for Higher Resolution Displays</a>



[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Make Typography Responsive</a>



[Voltar ao Índice](#indice)

---


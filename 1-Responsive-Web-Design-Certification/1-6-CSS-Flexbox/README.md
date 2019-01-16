# Introduction to the CSS Flexbox Challenges

https://learn.freecodecamp.org/responsive-web-design/css-flexbox

A website's User Interface ("UI") has two components. First, there are the visual elements, such as colors, fonts, and images. Second, there is the placement or positioning of those elements. In Responsive Web Design, a UI layout must accommodate many different browsers and devices accessing the content.

CSS3 introduced Flexible Boxes, or flexbox, to create page layouts for a dynamic UI. It is a layout mode that arranges elements in a predictable way for different screen sizes and browsers. While somewhat new, all popular modern browsers support flexbox. This section covers how to use flexbox and the different layout options it offers. 

## <a name="indice">Índice</a>

1. [Use display: flex to Position Two Boxes](#parte1)     
2. [Add Flex Superpowers to the Tweet Embed](#parte2)     
3. [Use the flex-direction Property to Make a Row](#parte3)     
4. [Apply the flex-direction Property to Create Rows in the Tweet Embed](#parte4)     
5. [Use the flex-direction Property to Make a Column](#parte5)     
6. [Apply the flex-direction Property to Create a Column in the Tweet Embed](#parte6)     
7. [Align Elements Using the justify-content Property](#parte7)     
8. [Use the justify-content Property in the Tweet Embed](#parte8)     
9. [Align Elements Using the align-items Property](#parte9)     
10. [Use the align-items Property in the Tweet Embed](#parte10)     
11. [Use the flex-wrap Property to Wrap a Row or Column](#parte11)     
12. [Use the flex-shrink Property to Shrink Items](#parte12)     
13. [Use the flex-grow Property to Expand Items](#parte13)     
14. [Use the flex-basis Property to Set the Initial Size of an Item](#parte14)     
15. [Use the flex Shorthand Property](#parte15)     
16. [Use the order Property to Rearrange Items](#parte16)     
17. [Use the align-self Property](#parte17)     
---


## <a name="parte1">1 - Use display: flex to Position Two Boxes</a>

This section uses alternating challenge styles to show how to use CSS to position elements in a flexible way. First, a challenge will explain theory, then a practical challenge using a simple tweet component will apply the flexbox concept.

Placing the CSS property display: flex; on an element allows you to use other flex properties to build a responsive page.


Add the CSS property display to #box-container and set its value to flex.

```html
<style>
  #box-container {
    height: 500px;
    display:flex;
  }
  
  #box-1 {
    background-color: dodgerblue;
    width: 50%;
    height: 50%;
    
  }

  #box-2 {
    background-color: orangered;
    width: 50%;
    height: 50%;
    
  }
</style>
<div id="box-container">
  <div id="box-1"></div>
  <div id="box-2"></div>
</div>

```

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Add Flex Superpowers to the Tweet Embed</a>

To the right is the tweet embed that will be used as the practical example. Some of the elements would look better with a different layout. The last challenge demonstrated display: flex. Here you'll add it to several components in the tweet embed to start adjusting their positioning.


Add the CSS property display: flex to all of the following items - note that the selectors are already set up in the CSS:

header, the header's .profile-name, the header's .follow-btn, the header's h3 and h4, the footer, and the footer's .stats.

```html

<style>
  body {
    font-family: Arial, sans-serif;
  }
  header {
    display: flex;
  }
  header .profile-thumbnail {
    width: 50px;
    height: 50px;
    border-radius: 4px;
  }
  header .profile-name {
    display:flex;
    margin-left: 10px;
  }
  header .follow-btn {
    display:flex;
    margin: 0 0 0 auto;
  }
  header .follow-btn button {
    border: 0;
    border-radius: 3px;
    padding: 5px;
  }
  header h3, header h4 {
    display:flex;
    margin: 0;
  }
  #inner p {
    margin-bottom: 10px;
    font-size: 20px;
  }
  #inner hr {
    margin: 20px 0;
    border-style: solid;
    opacity: 0.1;
  }
  footer {
    display: flex;
  }
  footer .stats {
    display:flex;
    font-size: 15px;
  }
  footer .stats strong {
    font-size: 18px;
  }
  footer .stats .likes {
    margin-left: 10px;
  }
  footer .cta {
    margin-left: auto;
  }
  footer .cta button {
    border: 0;
    background: transparent;
  }
</style>
<header>
  <img src="https://pbs.twimg.com/profile_images/378800000147359764/54dc9a5c34e912f34db8662d53d16a39_400x400.png" alt="Quincy Larson's profile picture" class="profile-thumbnail">
  <div class="profile-name">
    <h3>Quincy Larson</h3>
    <h4>@ossia</h4>
  </div>
  <div class="follow-btn">
    <button>Follow</button>
  </div>
</header>
<div id="inner">
  <p>I meet so many people who are in search of that one trick that will help them work smart. Even if you work smart, you still have to work hard.</p>
  <span class="date">1:32 PM - 12 Jan 2018</span>
  <hr>
</div>
<footer>
  <div class="stats">
    <div class="Retweets">
      <strong>107</strong> Retweets
    </div>
    <div class="likes">
      <strong>431</strong> Likes
    </div>
  </div>
  <div class="cta">
    <button class="share-btn">Share</button>
    <button class="retweet-btn">Retweet</button>
    <button class="like-btn">Like</button>
  </div>
</footer>

```

[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Use the flex-direction Property to Make a Row</a>



[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Apply the flex-direction Property to Create Rows in the Tweet Embed</a>



[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Use the flex-direction Property to Make a Column</a>



[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Apply the flex-direction Property to Create a Column in the Tweet Embed</a>



[Voltar ao Índice](#indice)

---


## <a name="parte7">7 - Align Elements Using the justify-content Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte8">8 - Use the justify-content Property in the Tweet Embed</a>



[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Align Elements Using the align-items Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Use the align-items Property in the Tweet Embed</a>



[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Use the flex-wrap Property to Wrap a Row or Column</a>



[Voltar ao Índice](#indice)

---


## <a name="parte12">12 - Use the flex-shrink Property to Shrink Items</a>



[Voltar ao Índice](#indice)

---


## <a name="parte13">13 - Use the flex-grow Property to Expand Items</a>



[Voltar ao Índice](#indice)

---


## <a name="parte14">14 - Use the flex-basis Property to Set the Initial Size of an Item</a>



[Voltar ao Índice](#indice)

---


## <a name="parte15">15 - Use the flex Shorthand Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte16">16 - Use the order Property to Rearrange Items</a>



[Voltar ao Índice](#indice)

---


## <a name="parte17">17 - Use the align-self Property</a>



[Voltar ao Índice](#indice)

---


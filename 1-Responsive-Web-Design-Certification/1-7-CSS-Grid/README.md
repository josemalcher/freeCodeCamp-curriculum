# Introduction to the CSS Grid Challenges

https://learn.freecodecamp.org/responsive-web-design/css-grid

CSS Grid helps you easily build complex web designs. It works by turning an HTML element into a grid container with rows and columns for you to place children elements where you want within the grid. 

## <a name="indice">Índice</a>

1. [Create Your First CSS Grid](#parte1)     
2. [Add Columns with grid-template-columns](#parte2)     
3. [Add Rows with grid-template-rows](#parte3)     
4. [Use CSS Grid units to Change the Size of Columns and Rows](#parte4)     
5. [Create a Column Gap Using grid-column-gap](#parte5)     
6. [Create a Row Gap using grid-row-gap](#parte6)     
7. [Add Gaps Faster with grid-gap](#parte7)     
8. [Use grid-column to Control Spacing](#parte8)     
9. [Use grid-row to Control Spacing](#parte9)     
10. [Align an Item Horizontally using justify-self](#parte10)     
11. [Align an Item Vertically using align-self](#parte11)     
12. [Align All Items Horizontally using justify-items](#parte12)     
13. [Align All Items Vertically using align-items](#parte13)     
14. [Divide the Grid Into an Area Template](#parte14)     
15. [Place Items in Grid Areas Using the grid-area Property](#parte15)     
16. [Use grid-area Without Creating an Areas Template](#parte16)     
17. [Reduce Repetition Using the repeat Function](#parte17)     
18. [Limit Item Size Using the minmax Function](#parte18)     
19. [Create Flexible Layouts Using auto-fill](#parte19)     
20. [Create Flexible Layouts Using auto-fit](#parte20)     
21. [Use Media Queries to Create Responsive Layouts](#parte21)     
22. [Create Grids within Grids](#parte22)     
---


## <a name="parte1">1 - Create Your First CSS Grid</a>

Turn any HTML element into a grid container by setting its display property to grid. This gives you the ability to use all the other properties associated with CSS Grid.

Note  
In CSS Grid, the parent element is referred to as the container and its children are called items.


Change the display of the div with the container class to grid.

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    width: 100%;
    background: LightGray;
    /* add your code below this line */
    display:grid;
    
    /* add your code above this line */
  }
</style>
  
<div class="container">
  <div class="d1">1</div>
  <div class="d2">2</div>
  <div class="d3">3</div>
  <div class="d4">4</div>
  <div class="d5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Add Columns with grid-template-columns</a>

Simply creating a grid element doesn't get you very far. You need to define the structure of the grid as well. To add some columns to the grid, use the grid-template-columns property on a grid container as demonstrated below:

```css
.container {
  display: grid;
  grid-template-columns: 50px 50px;
}
```

This will give your grid two columns that are 50px wide each.

The number of parameters given to the grid-template-columns property indicates the number of columns in the grid, and the value of each parameter indicates the width of each column.


Give the grid container three columns that are 100px wide each.

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* add your code below this line */
     grid-template-columns: 100px 100px 100px;
    
    /* add your code above this line */
  }
</style>
  
<div class="container">
  <div class="d1">1</div>
  <div class="d2">2</div>
  <div class="d3">3</div>
  <div class="d4">4</div>
  <div class="d5">5</div>
</div>
```


[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Add Rows with grid-template-rows</a>



[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Use CSS Grid units to Change the Size of Columns and Rows</a>



[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Create a Column Gap Using grid-column-gap</a>



[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Create a Row Gap using grid-row-gap</a>



[Voltar ao Índice](#indice)

---


## <a name="parte7">7 - Add Gaps Faster with grid-gap</a>



[Voltar ao Índice](#indice)

---


## <a name="parte8">8 - Use grid-column to Control Spacing</a>



[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Use grid-row to Control Spacing</a>



[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Align an Item Horizontally using justify-self</a>



[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Align an Item Vertically using align-self</a>



[Voltar ao Índice](#indice)

---


## <a name="parte12">12 - Align All Items Horizontally using justify-items</a>



[Voltar ao Índice](#indice)

---


## <a name="parte13">13 - Align All Items Vertically using align-items</a>



[Voltar ao Índice](#indice)

---


## <a name="parte14">14 - Divide the Grid Into an Area Template</a>



[Voltar ao Índice](#indice)

---


## <a name="parte15">15 - Place Items in Grid Areas Using the grid-area Property</a>



[Voltar ao Índice](#indice)

---


## <a name="parte16">16 - Use grid-area Without Creating an Areas Template</a>



[Voltar ao Índice](#indice)

---


## <a name="parte17">17 - Reduce Repetition Using the repeat Function</a>



[Voltar ao Índice](#indice)

---


## <a name="parte18">18 - Limit Item Size Using the minmax Function</a>



[Voltar ao Índice](#indice)

---


## <a name="parte19">19 - Create Flexible Layouts Using auto-fill</a>



[Voltar ao Índice](#indice)

---


## <a name="parte20">20 - Create Flexible Layouts Using auto-fit</a>



[Voltar ao Índice](#indice)

---


## <a name="parte21">21 - Use Media Queries to Create Responsive Layouts</a>



[Voltar ao Índice](#indice)

---


## <a name="parte22">22 - Create Grids within Grids</a>



[Voltar ao Índice](#indice)

---


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

The grid you created in the last challenge will set the number of rows automatically. To adjust the rows manually, use the grid-template-rows property in the same way you used grid-template-columns in previous challenge.


Add two rows to the grid that are 50px tall each.

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
    grid-template-columns: 100px 100px 100px;
    /* add your code below this line */
    grid-template-rows: 50px 50px;
    
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


## <a name="parte4">4 - Use CSS Grid units to Change the Size of Columns and Rows</a>

You can use absolute and relative units like px and em in CSS Grid to define the size of rows and columns. You can use these as well:

- fr: sets the column or row to a fraction of the available space,
- auto: sets the column or row to the width or height of its content automatically,
- %: adjusts the column or row to the percent width of its container.

Here's the code that generates the output in the preview:

```css
    grid-template-columns: auto 50px 10% 2fr 1fr;
```
This snippet creates five columns. The first column is as wide as its content, the second column is 50px, the third column is 10% of its container, and for the last two columns; the remaining space is divided into three sections, two are allocated for the fourth column, and one for the fifth.


Make a grid with three columns whose widths are as follows: 1fr, 100px, and 2fr.

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
    /* modify the code below this line */

    grid-template-columns: 1fr 100px 2fr;
    
    /* modify the code above this line */
    grid-template-rows: 50px 50px;
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


## <a name="parte5">5 - Create a Column Gap Using grid-column-gap</a>

So far in the grids you have created, the columns have all been tight up against each other. Sometimes you want a gap in between the columns. To add a gap between the columns, use the grid-column-gap property like this:

```css
    grid-column-gap: 10px;
```
This creates 10px of empty space between all of our columns.

Give the columns in the grid a 20px gap.

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    /* add your code below this line */
     grid-column-gap:20px;
    
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


## <a name="parte6">6 - Create a Row Gap using grid-row-gap</a>

You can add a gap in between the rows of a grid using grid-row-gap in the same way that you added a gap in between columns in the previous challenge.


Create a gap for the rows that is 5px tall.

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    /* add your code below this line */
    grid-row-gap:5px;
    
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


## <a name="parte7">7 - Add Gaps Faster with grid-gap</a>

grid-gap is a shorthand property for grid-row-gap and grid-column-gap from the previous two challenges that's more convenient to use. If grid-gap has one value, it will create a gap between all rows and columns. However, if there are two values, it will use the first one to set the gap between the rows and the second value for the columns.


Use grid-gap to introduce a 10px gap between the rows and 20px gap between the columns.

```html
<style>
  .d1{background:LightSkyBlue;}
  .d2{background:LightSalmon;}
  .d3{background:PaleTurquoise;}
  .d4{background:LightPink;}
  .d5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    /* add your code below this line */
    
    grid-gap:10px 20px;
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


## <a name="parte8">8 - Use grid-column to Control Spacing</a>

Up to this point, all the properties that have been discussed are for grid containers. The grid-column property is the first one for use on the grid items themselves.

The hypothetical horizontal and vertical lines that create the grid are referred to as lines. These lines are numbered starting with 1 at the top left corner of the grid and move right for columns and down for rows, counting upward.

This is what the lines look like for a 3x3 grid:

![](img/grid-column.png)

To control the amount of columns an item will consume, you can use the grid-column property in conjunction with the line numbers you want the item to start and stop at.

Here's an example:
```css
    grid-column: 1 / 3;
```

This will make the item start at the first vertical line of the grid on the left and span to the 3rd line of the grid, consuming two columns.


Make the item with the class item5 consume the last two columns of the grid.

```html

<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  
  .item5 {
    background: PaleGreen;
    /* add your code below this line */
    
    grid-column: 2/4;
    /* add your code above this line */
  }
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>

```

[Voltar ao Índice](#indice)

---


## <a name="parte9">9 - Use grid-row to Control Spacing</a>

Of course, you can make items consume multiple rows just like you can with columns. You define the horizontal lines you want an item to start and stop at using the grid-row property on a grid item.


Make the element with the item5 class consume the last two rows.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  
  .item5 {
    background: PaleGreen;
    grid-column: 2 / 4;
    /* add your code below this line */
    
    grid-row:2/4;
    /* add your code above this line */
  }
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte10">10 - Align an Item Horizontally using justify-self</a>

In CSS Grid, the content of each item is located in a box which is referred to as a cell. You can align the content's position within its cell horizontally using the justify-self property on a grid item. By default, this property has a value of stretch, which will make the content fill the whole width of the cell. This CSS Grid property accepts other values as well:

- start: aligns the content at the left of the cell,
- center: aligns the content in the center of the cell,
- end: aligns the content at the right of the cell.


Use the justify-self property to center the item with the class item2.

```html
<style>
  .item1{background: LightSkyBlue;}
  
  .item2 {
    background: LightSalmon;
    /* add your code below this line */
    
    justify-self:center;
    /* add your code above this line */
  }
  
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte11">11 - Align an Item Vertically using align-self</a>

Just as you can align an item horizontally, there's a way to align an item vertically as well. To do this, you use the align-self property on an item. This property accepts all of the same values as justify-self from the last challenge.


Align the item with the class item3 vertically at the end.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  
  .item3 {
    background: PaleTurquoise;
    /* add your code below this line */
    
    align-self:end;
    
    /* add your code above this line */
  }
  
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte12">12 - Align All Items Horizontally using justify-items</a>

Sometimes you want all the items in your CSS Grid to share the same alignment. You can use the previously learned properties and align them individually, or you can align them all at once horizontally by using justify-items on your grid container. This property can accept all the same values you learned about in the previous two challenges, the difference being that it will move all the items in our grid to the desired alignment.


Use this property to center all our items horizontally.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
    /* add your code below this line */
    
    justify-items:center;
    
    /* add your code above this line */
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte13">13 - Align All Items Vertically using align-items</a>

Using the align-items property on a grid container will set the vertical alignment for all the items in our grid.


Use it now to move all the items to the end of each cell.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
    /* add your code below this line */
    
    align-items:end;

    /* add your code above this line */
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte14">14 - Divide the Grid Into an Area Template</a>

You can group cells of your grid together into an area and give the area a custom name. Do this by using grid-template-areas on the container like this:

```
grid-template-areas:
  "header header header"
  "advert content content"
  "footer footer footer";
```

The code above merges the top three cells together into an area named header, the bottom three cells into a footer area, and it makes two areas in the middle row; advert and content.

Note  
Every word in the code represents a cell and every pair of quotation marks represent a row.

In addition to custom labels, you can use a period (.) to designate an empty cell in the grid.


Place the area template so that the cell labeled advert becomes an empty cell.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
    /* change code below this line */
    
    grid-template-areas:
      "header header header"
      ". content content"
      "footer footer footer";
    /* change code above this line */
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte15">15 - Place Items in Grid Areas Using the grid-area Property</a>

After creating an areas template for your grid container, as shown in the previous challenge, you can place an item in your custom area by referencing the name you gave it. To do this, you use the grid-area property on an item like this:

```css
    .item1 { grid-area: header; }
```
This lets the grid know that you want the item1 class to go in the area named header. In this case, the item will use the entire top row because that whole row is named as the header area.


Place an element with the item5 class in the footer area using the grid-area property.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  
  .item5 {
    background: PaleGreen;
    /* add your code below this line */
    
    grid-area: footer;
    
    /* add your code above this line */
  }
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
    grid-template-areas: 
      "header header header"
      "advert content content"
      "footer footer footer";
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```


[Voltar ao Índice](#indice)

---


## <a name="parte16">16 - Use grid-area Without Creating an Areas Template</a>

The grid-area property you learned in the last challenge can be used in another way. If your grid doesn't have an areas template to reference, you can create an area on the fly for an item to be placed like this:

```css
    item1 { grid-area: 1/1/2/4; }
```

This is using the line numbers you learned about earlier to define where the area for this item will be. The numbers in the example above represent these values:

```css
    grid-area: horizontal line to start at / vertical line to start at / horizontal line to end at / vertical line to end at;
```
So the item in the example will consume the rows between lines 1 and 2, and the columns between lines 1 and 4.


Using the grid-area property, place the element with item5 class between the third and fourth horizontal lines and between the first and fourth vertical lines.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  
  .item5 {
    background: PaleGreen;
    /* add your code below this line */
    
    grid-area:3/1/4/4;
    
    /* add your code above this line */
  }
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte17">17 - Reduce Repetition Using the repeat Function</a>

When you used grid-template-columns and grid-template-rows to define the structure of a grid, you entered a value for each row or column you created.

Lets say you want a grid with 100 rows of the same height. It isn't very practical to insert 100 values individually. Fortunately, there's a better way - by using the repeat function to specify the number of times you want your column or row to be repeated, followed by a comma and the value you want to repeat.

Here's an example that would create the 100 row grid, each row at 50px tall.

```css
    grid-template-rows: repeat(100, 50px);
```
You can also repeat multiple values with the repeat function, and insert the function amongst other values when defining a grid structure. Here's what I mean:

```css
    grid-template-columns: repeat(2, 1fr 50px) 20px;
```

This translates to:

```css
    grid-template-columns: 1fr 50px 1fr 50px 20px;
```

Note  
1fr 50px is repeated twice followed by 20px.


Use repeat to remove repetition from the grid-template-columns property.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* change the code below this line */
    
    grid-template-columns: repeat(3,1fr);
    
    /* change the code above this line */
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte18">18 - Limit Item Size Using the minmax Function</a>

There's another built-in function to use with grid-template-columns and grid-template-rows called minmax. It's used to limit the size of items when the grid container changes size. To do this you need to specify the acceptable size range for your item. Here is an example:

```css
    grid-template-columns: 100px minmax(50px, 200px);
```

In the code above, grid-template-columns is set to create two columns; the first is 100px wide, and the second has the minimum width of 50px and the maximum width of 200px.


Using the minmax function, replace the 1fr in the repeat function with a column size that has the minimum width of 90px and the maximum width of 1fr, and resize the preview panel to see the effect.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* change the code below this line */
    
    grid-template-columns: repeat(3, minmax(90px,1fr));
    
    /* change the code above this line */
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte19">19 - Create Flexible Layouts Using auto-fill</a>

The repeat function comes with an option called auto-fill. This allows you to automatically insert as many rows or columns of your desired size as possible depending on the size of the container. You can create flexible layouts when combining auto-fill with minmax.

In the preview, grid-template-columns is set to

```css
    repeat(auto-fill, minmax(60px, 1fr));

```

When the container changes size, this setup keeps inserting 60px columns and stretching them until it can insert another one.

Note  
If your container can't fit all your items on one row, it will move them down to a new one.


In the first grid, use auto-fill with repeat to fill the grid with columns that have a minimum width of 60px and maximum of 1fr. Then resize the preview to see auto-fill in action.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 100px;
    width: 100%;
    background: LightGray;
    display: grid;
    /* change the code below this line */
    
    grid-template-columns: repeat(auto-fill, minmax(60px, 1fr));
    
    /* change the code above this line */
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
  
  .container2 {
    font-size: 40px;
    min-height: 100px;
    width: 100%;
    background: Silver;
    display: grid;
    grid-template-columns: repeat(3, minmax(60px, 1fr));
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
<div class="container2">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte20">20 - Create Flexible Layouts Using auto-fit</a>

auto-fit works almost identically to auto-fill. The only difference is that when the container's size exceeds the size of all the items combined, auto-fill keeps inserting empty rows or columns and pushes your items to the side, while auto-fit collapses those empty rows or columns and stretches your items to fit the size of the container.

Note  
If your container can't fit all your items on one row, it will move them down to a new one.


In the second grid, use auto-fit with repeat to fill the grid with columns that have a minimum width of 60px and maximum of 1fr. Then resize the preview to see the difference.

```html
<style>
  .item1{background:LightSkyBlue;}
  .item2{background:LightSalmon;}
  .item3{background:PaleTurquoise;}
  .item4{background:LightPink;}
  .item5{background:PaleGreen;}
  
  .container {
    font-size: 40px;
    min-height: 100px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: repeat( auto-fill, minmax(60px, 1fr));
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
  
  .container2 {
    font-size: 40px;
    min-height: 100px;
    width: 100%;
    background: Silver;
    display: grid;
    /* change the code below this line */
    
    grid-template-columns: repeat(auto-fit, minmax(60px, 1fr));
    
    /* change the code above this line */
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
  }
</style>
  
<div class="container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
<div class="container2">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
  <div class="item5">5</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte21">21 - Use Media Queries to Create Responsive Layouts</a>

CSS Grid can be an easy way to make your site more responsive by using media queries to rearrange grid areas, change dimensions of a grid, and rearrange the placement of items.

In the preview, when the viewport width is 300px or more, the number of columns changes from 1 to 2. The advertisement area then occupies the left column completely.


When the viewport width is 400px or more, make the header area occupy the top row completely and the footer area occupy the bottom row completely.

```html
<style>
  .item1 {
    background: LightSkyBlue;
    grid-area: header;
  }
  
  .item2 {
    background: LightSalmon;
    grid-area: advert;
  }
  
  .item3 {
    background: PaleTurquoise;
    grid-area: content;
  }
  
  .item4 {
    background: lightpink;
    grid-area: footer;
  }
  
  .container {
    font-size: 1.5em;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: 1fr;
    grid-template-rows: 50px auto 1fr auto;
    grid-gap: 10px;
    grid-template-areas:
      "header"
      "advert"
      "content"
      "footer";
  }
  
  @media (min-width: 300px){
    .container{
      grid-template-columns: auto 1fr;
      grid-template-rows: auto 1fr auto;
      grid-template-areas:
        "advert header"
        "advert content"
        "advert footer";
    }
  }
  
  @media (min-width: 400px){
    .container{
      /* change the code below this line */
    
      grid-template-areas:
        "header header"
        "advert content"
        "footer footer";
    
    /* change the code above this line */
    }
  }
</style>
  
<div class="container">
  <div class="item1">header</div>
  <div class="item2">advert</div>
  <div class="item3">content</div>
  <div class="item4">footer</div>
</div>
```

[Voltar ao Índice](#indice)

---


## <a name="parte22">22 - Create Grids within Grids</a>

Turning an element into a grid only affects the behavior of its direct descendants. So by turning a direct descendant into a grid, you have a grid within a grid.

For example, by setting the display and grid-template-columns properties of the element with the item3 class, you create a grid within your grid.


Turn the element with the item3 class into a grid with two columns with a width of auto and 1fr using display and grid-template-columns.

```html
<style>
  .container {
    font-size: 1.5em;
    min-height: 300px;
    width: 100%;
    background: LightGray;
    display: grid;
    grid-template-columns: auto 1fr;
    grid-template-rows: auto 1fr auto;
    grid-gap: 10px;
    grid-template-areas:
      "advert header"
      "advert content"
      "advert footer";
  }
  .item1 {
    background: LightSkyBlue;
    grid-area: header;
  }
  
  .item2 {
    background: LightSalmon;
    grid-area: advert;
  }
  
  .item3 {
    background: PaleTurquoise;
    grid-area: content;
    /* enter your code below this line */
    
    display:grid;
    grid-template-columns:auto 1fr;
    
    /* enter your code above this line */
  }
  
  .item4 {
    background: lightpink;
    grid-area: footer;
  }
  
  .itemOne {
    background: PaleGreen;
  }
  
  .itemTwo {
    background: BlanchedAlmond;
  }
  
</style>
  
<div class="container">
  <div class="item1">header</div>
  <div class="item2">advert</div>
  <div class="item3">
    <div class="itemOne">paragraph1</div>
    <div class="itemTwo">paragraph2</div>
  </div>
  <div class="item4">footer</div>
</div>
```

[Voltar ao Índice](#indice)

---


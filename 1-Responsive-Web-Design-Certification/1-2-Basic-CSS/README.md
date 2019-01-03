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



[Voltar ao Índice](#indice)

---


## <a name="parte2">2 - Use CSS Selectors to Style Elements</a>



[Voltar ao Índice](#indice)

---


## <a name="parte3">3 - Use a CSS Class to Style an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte4">4 - Style Multiple Elements with a CSS Class</a>



[Voltar ao Índice](#indice)

---


## <a name="parte5">5 - Change the Font Size of an Element</a>



[Voltar ao Índice](#indice)

---


## <a name="parte6">6 - Set the Font Family of an Element</a>



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


## CSS Notes

- HTML is the barebones of a website while CSS is what makes your page all pretty and nice to look at.
- The key to understanding how CSS works is to imagine there is an invisible box around every HTML element.
- CSS work by associating **rules** with HTML elements. These **rules** govern how th content of specified elements should be displayed. A CSS **rule** contains two parts a **selector** and a **declaration**.
    - **Selectors** indicate which element the rule applies to. The same rule can apply to more than one element if you separate the element names with commas.
    - **Declarations** indicate how the elements reffered to in the selector should be styled. Declarations are split into two parts (a property and a value), and are separated by a colon.
        - *Properties* indicate the aspects of the element you want to change. Ex.) color, font, width, height and border.
        - *Values* specify the settings you want to use for the chosen properties. ex.) the value is a the color you want to specify the font to be.
  
   Selector --> `p{
                   font-family: Arial;}` <--Declaration
    
### CSS Colors

- The color property allows you to specify the color of text inside of an element. You can specify any color in CSS in one of three ways:
    - **RGB Values** express colors in terms of how much red, green, and blue are used to make it up. Ex.) `rgb(100.100.90)`.
    - **Hex codes** are six-digit codes that represent the amount of red, green and blue in a color preceded by a pound or a `#` sign. Ex.) `#ee3e80`
    - The **Color Names** are 147 predefined names that are recognized by browsers. Ex.) `DarkCyan`

- CSS treats each HTML element as if it appears in a box, and the **backround-color** property sets the color of the background for that box.

- Color pickers like [this one](https://color.adobe.com/create/color-wheel) can help you find the color you want.

- It is important to ensure there is enough contrast between any text and background color, otherwise people cannot read your content.

## CSS3

- CSS3 introduces the opacity property which allows you to specify the opacity of an elemnt and any of its child elements. The value is a nukber between 0.0 and 1.0.
- CSS3 rgba property allows you to specify a color just like with an RGB value, but adds a fourth value. This is the alpha value and is a number between 0.0 and 1.0.
- **Hue** is near to the colliquial idea of color. This is expressed as an angle beteween 0 and 360 degrees.
- **Saturation** refers to the amount of gray in a color. At max saturation there would be no gray and at min the color would be mostly gray. This is expressed as a percentage.
- **Brightness** (or value) is how much black is in a color. At max brightness there would be no black and at min the color would be very dark. This is ecpressed as a percentage with 0% being white 50% being normal and 100% being black.

-The hsla color property allows you to specify color properties using hue, saturation, and lightness as above, and adds a fourth value which represents transparency (just like the rgba property). The a stands for:
    - **Alpha**, expressed as a number between b0 and 1.0. Ex.) 0.5 represents 50% transparency, and 0.75 represents 75% transparency.

hsla example:
```
body {
background-color: #C8C8C8;
background-color: hsl(0,0%,78%);}
p {
background-color: #ffffff;
background-color: hsla(0,100%,100%,0.5);}
```


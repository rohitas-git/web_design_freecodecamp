# Color models

There are two main color models:

-   The Additive RGB (red, green, blue) model used in electronic devices, and
-   The Subtractive CMYK (cyan, magenta, yellow, black) model used in print.
-   The HSL color model(hue, saturation, and lightness) 


## Additive RGB Color Model
In this project, you'll work with the RGB model.
This means that colors begin as black, and change as different levels of red, green, and blue are introduced.
An easy way to see this is with the CSS rgb function.

The CSS rgb function accepts values, or arguments, for red, green, and blue, and produces a color:
rgb(red,green,blue)

### Primary, Secondary, Tertiary colors 

In the additive RGB color model, colors begin as black, and change as different levels of red, green, and blue are introduced.

-   Black: rgb(0,0,0)

Primary colors are colors that, when combined, create pure white.

-   Red: rgb(255, 0, 0)
-   Green: rgb(0, 255, 0)
-   Blue: rgb(0, 0, 255)

Secondary colors are the colors you get when you combine primary colors.

-   Cyan: rgb(0, 255, 255)
-   Magenta: rgb(255, 0, 255)
-   Yellow: rgb(255, 255, 0)

Tertiary colors are created by combining a primary with a nearby secondary color.

-   Orange: rgb(255, 127, 0)
-   Spring green: rgb(0, 255, 127)
-   Purple: rgb(127, 0, 255)
-   Chartreuse green: rgb(127, 255, 0)
-   Azure: rgb(0, 127, 255)
-   Rose (Bright Pink): rgb(255, 0, 127)

## Color Wheel and Complementary Color 
A color wheel is a circle where similar colors, or hues, are near each other, and different ones are further apart.

Two colors that are opposite from each other on the color wheel are called complementary colors. 
- If two complementary colors are combined, they produce gray. 
- But when they are placed side-by-side, these colors produce strong visual contrast and appear brighter.

Bad practice:
Notice that the red and cyan colors are very bright right next to each other. This contrast can be distracting if it's overused on a website, and can make text hard to read if it's placed on a complementary-colored background.

Best practice:
It's better practice to choose one color as the dominant color, and use its complementary color as an accent to bring attention to certain content on the page.

There are several other important color combinations outside of complementary colors, but you'll learn those a bit later.

## HEX Values (Another form of RGB values)

A very common way to apply color to an element with CSS is with hexadecimal or hex values. While hex values sound complicated, they're really just another form of RGB values.

Hexadecimal, or base 16 values, go from 0 - 9, then A - F:
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F

Hex color values start with a # character and take six characters from 0-9 and A-F. 
The first pair of characters represent red, the second pair represent green, and the third pair represent blue. For example, #4B5320.

With hex colors, 00 is 0% of that color, and FF is 100%. So #00FF00 translates to 0% red, 100% green, and 0% blue, and is the same as rgb(0, 255, 0).

## HSL Model
HSL stands for Hue, Saturation, Lightness

The CSS hsl function accepts 3 values: 
- Hue: 0 - 360 degrees, 
- Saturation: 0 - 100 % 
- Lightness: 0 - 100 %  

Hue (imagine a color wheel, x hue is color at x degrees)
- 0 : Red, 120: Green, 240: Blue
  
Saturation (the intensity of a color) (amount of grey in the color)
- 0%: Gray,     100%: Pure color
  
Lightness (how bright a color appears) (amount of white add to hue)
- 0%: Black,    100%: White,   50%: Netural
  
### Ways learnt to set flat colors:
- RGB(r,g,b), HEX Value,  HSL

### Using a color transition, or gradient, on an element.
A gradient is when one color transitions into another. 

The CSS linear-gradient function lets you control the direction of the transition along a line, and which colors are used.

One thing to remember is that the linear-gradient function actually creates an image element, and is usually paired with the background property which can accept an image as a value.

    background: linear-gradient(gradientDirection, color1, color2, ...);

- gradientDirection is the direction of the line used for the transition. 
- color1 and color2 are color arguments, which are the colors that will be used in the transition itself. These can be any type of color, including color keywords, hex, rgb, or hsl.

#### Color-stops
Color-stops allow you to fine-tune where colors are placed along the gradient line. They are a length unit like px or percentages that follow a color in the linear-gradient function.

>! box-shadow: offsetX offsetY blurRadius spreadRadius color;
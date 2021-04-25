# Colors in CSS
The *color property* allows you to specify the color of text inside an element/ the color of background. 
You can specify any color in CSS in one of these ways:



## 1. rgb values
An RGB color value is specified with the rgb() function, which has the following syntax: 
**``` rgb(red, green, blue)```**

Each parameter (red, green, and blue) defines the intensity of the color and can be an integer between 0 and 255 or a percentage value (from 0% to 100%).

For example, the rgb(0,0,255) value is rendered as blue, because the blue parameter is set to its highest value (255) and the others are set to 0.

Also, the following values define equal color: rgb(0,0,255) and rgb(0%,0%,100%). 


  ### 1.1 rgb**a** = rgb + **opacity** 
* RGBA color values are an extension of RGB color values with an alpha channel - which specifies the opacity of the object.

* An RGBA color is specified with the rgba() function, which has the following syntax:

  **```rgba(red, green, blue, alpha)```**

* The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (fully opaque).

---



## 2. hex codes
* A hexadecimal color is specified with: ***#RRGGBB***, where the RR (red), GG (green) and BB (blue) hexadecimal integers specify the components of the color. All values must be between 00 and FF.

* For example, the **``#0000ff``** value is rendered as blue, because the blue component is set to its highest value (ff) and the others are set to 00.


---

## 3. color names
* 140 color names are predefined in the HTML and CSS color specification.
   * For example: blue, red, coral, brown, etc..


---



## 4. HSL & HSLA
* HSL stands for hue, saturation, and lightness.
* HSL color values are specified with: hsl(*hue, saturation, lightness*).
  * ***Hue*** is a degree on the color wheel from 0 to 360. 0 is red, 120 is green, 240 is blue.
  * ***Saturation*** is a percentage value; 0% means a shade of gray and 100% is the full color.
  * ***Lightness*** is also a percentage; 0% is black, 100% is white.



  ### 4.1  HSLA
* The hsla() function define colors using the Hue-saturation-lightness-alpha model (HSLA).
* HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity of the color.
  * alpha	Defines the opacity as a number between 0.0 (fully transparent) and 1.0 (fully opaque).



-----

[***colorhunt***](https://colorhunt.co/)


-----

*&copy; Masalha96*
  [GitHub account](https://github.com/masalha-96)









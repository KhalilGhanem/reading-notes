# Images, Color, Text
## Images
We use `<img>` tage to add images to our web page.

`<img>` tag attributes:
* src: Specifies the path to the image.
* alt: Specifies an alternate text for the image.
* width :specify the width  of an image.
* height :specify the height of an image.

***

## Color

Color brings your site to life 

 How to specify colors in CSS: 
* predefined color names
* RBG
* HSL
* HEX

 Examples:
```
color name: <h1 style="color:lime;">Hello World</h1>
RBG :<h1 style="color:rgb(60, 60, 60);">Hello World</h1>
HSL: <h1 style="color:hsl(240, 100%, 50%);">Hello World</h1>
Hex : <h1 style="color:#ee82ee;">Hello World</h1>
```
It is important to ensure that there is enough contrast between any text and the background color
*This will make your site more readable.


 RBG & HEX Are using an alpha channel that indicate to the opacity.

***
## Text
CSS attributes to customize the text:
* font-family in  CSS there are five generic font families:
  1. Serif: it have extra details on the end of the main strokes of the letters.
  2. Sans-serif: have straight ends to letters and therefore have a much cleaner design.
  3. Monospace: Every letter in a monospace typeface is the same width. 
  4. Cursive: Cursive fonts either have joining strokes or other cursive characteristics, such as handwriting styles.
  5. Fantasy: Fantasy fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text. 
* font-size: sets the size of the text.
* @font-face allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to 
   specify  a path to a copy of the font, which will be downloaded if it is not on the user's machine.
* font-weight:sets how thick or thin characters in text should be displayed.font-weight values:
  * normal
  * bold
* The font-style: specifies the font style for a text.font-style Values:
  * normal
  * italic
  * oblique
* Text-transform:is is used to change the case of text. Text-transform values:
  * uppercase
  * lowercase
  * capitalize
* Text-decoration: specifies the decoration added to text. Text-decoration values:
  * none
  * underline 
  * overline
  * line-through
* Text-align: allows you to control the alignment of text.Text-align values:
  * left
  * right
  * center
  * justify

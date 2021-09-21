# HTML & CSS: Design and Build Websites

## Chapters 3 & 4:
1. There are three main types of lists in HTML: ordered, unordered, and definition. What are the differences?
  - Ordered: an ordered list is typically a numbered list of items
    * Tag: <ol> </ol>
  - Unordered: an unordered list is typically a non-numbered, bulleted list of items
    * Tag: <ul> </ul>
  - Both ordered and unordered lists when created will look like:
    <ol or ul>
      <li> </li>
      <li> </li>
    </ol or /ul>
  - Defintion: used to enclose a list of groups of terms and their associated descriptions
    * Tags: terms (<dt>), descriptions (<dd>)

2. What is the basic structure of an element used to link to another site?
  - <a href="https://www.google.com">Google</a>
  - <a> tag that includes attribute href="" to provide link, text that will be hyperlinked, and the </a> closing tag

3. What attribute should you include in a link to open a new tab with the link is clicked?
  - After the href="" attribute that includes the site URL, include the attribute target= with the value of "_blank"
  - ex: <a href="https://www.google.com" target="_blank">Google</a>
  - Interestingly enough there is evidence from Google that shows using the new tab attribute opens your site up to phising attacks and malware (called: "tabnabbing"), therefore you should use the following attribute prior to the target="_blank" attribute:
    * rel="noopener noreferrer"

4. How do you link a specific part of the same page?
  - Instead of href="" to the URL of another site, you would use id="" with the same name of the id you gave that specific element you want it to link to

## Chapters 10-12:

1. What is the purpose of CSS?
  - CSS is the language for describing the presentation of a webpage
  - Includes: colors, layouts, fonts, etc
  - Allows adapting of presentation to different types of devices: large screens, small screens, printers, etc
  - Independent of HTML and can be used with any XML-based markup language

2. What does CSS stand for? What does cascading mean in this case?
  - Cascading Style Sheets
  - Cascading refers to the "cascade", an algorithm that defines how to combine property values originating from different sources
  - Only CSS declarations, property/value pairs, participate in the cascade

3. What is the basic structure of a CSS rule?
  - The CSS rule is a statement that defines the style of one or more elements in the webpage
  - The syntax for CSS consists of a *selector* and a *declaration*. A *declaration block* consists of several declarations for a given selector
  - Multiple selectors can be combined in a rule
  - ex: selector {declaration}
  - ex: h1 {font-weight: bold; color: green;}

4. How do you link a CSS stylesheet to your HTML document?
  - An external stylesheet is a plain text file that contains CSS Style formats only
  - File extension should always end in .css
  - You can link to your HTML using the <link> tag, placing it within the <head> section, but only after the <title> tag
  - ex: <link rel="stylesheet" type="text/css" href="styles.css" />
  - The value of the rel attribute must be style sheet. The href attribute indicates the location and name of the style sheet file. In the above code , external file name is "style.css" and it is stored in the same directory location of your HTML file. If you want to store .css file in another directory location, then you should specify the path of your css file in the href.

5. When is it useful to use stylesheets as opposed to using internal CSS?
  - Using CSS files separates the CSS from the HTML, allowing you to make sure that your styles are correct and making sure your files are easy to modify later
  - External CSS stylesheets allow your browser to cached the file, increasing your application efficiency

6. Describe what a color hex code is:
  - Hex color codes are values that tell the computer how much color to show
  - The values are a special code that represent color values from 0 to 255
  - If RGB are all represented at the minimum of 0 (shown as 00 in the code), the color expressed will be black
  - Red = (255, 0, 0)
  - Green = (0, 128, 0)
  - Blue = (0, 0, 255)
  - White = (255, 255, 255)

7. What are the three parts of an HSL color property?
  - HSL stands for Hue, Saturation, Light
  - HSL was developed to evolve the RGB color system making it easier to visualize
  - Biggest benefit of HSL color wheel is complementary colors are located across from each other
  - Hue: determines the color of the rainbow, represented by 360 degrees
  - Saturation: the distance from the middle of the color wheel, or "how much" of a given color is present (the further away from the center of the wheel, the brighter/more vivid a color becomes)
  - Light(ness): the value is actually in the third dimension, making the wheel a cylinder where the "bottom" is black and the "top" is white, considering the lightness of a color its gradient between black and white

8. In the world of typeface, what are the three main categories of fonts? What are the differences between them?
  - A *typeface* is the design of lettering that can include variations in size, weight (bold), slope (italic), width (condensed), etc
  - Basic classifications of typefaces: *serif*, *sans serif*, *script*, *monospaced*, and *display*
  - serif + sans serif: used for either body copy or headlines (incl. titles, logos, etc)
  - script + dispaly: only used for headlines
  - monospaced: _generally_ used for displaying code, thought can also be used for body/headline copy
    - *serif* type styles: Old Style, Transitional, Neoclassical & Didone, Slab, Clarendone, Glyphic
    - *sans serif* type styles: Grotesque, Square, Humanistic, Geometric
    - *script* type styles: Formal, Casual, Calligraphic, Blackletter & Lombardic

9. When specifying font-size, what are the main three units used?
  - Pixels (px): good choice for when you need pixel accuracy because it is a static value
    * OS-independent and cross-browser way of literally telling the browsers to render the letters EXACTLY the number of pixels in height you specified
    * Typically used for font-size or images
  - Ems (em): creates a dynamic and computed font size, with the numeric value acting as a multiplier of the inherited font-size property of the element in which is is used on
    * p {font-size: 2em;} means that the text will be 2x the inherited size of the <p> element font
    * Typically used for width values and font-size
  - Percentage (%): if the inherited font-size is set to 100%, 110% would increase the inherited size by 10%
    * Typically used for width values and font-size
  - *ALL OF THESE* are altered differently depending on the font-family

[CODE PEN](https://codepen.io/alexmfritz/pen/qBjKPbW)

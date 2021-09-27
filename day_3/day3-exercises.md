# HTML & CSS Design

### Chapter 7 - Forms:

1. If you're using an input element in a form, what attribute controls the behavior of that input?
  - The type="" attribute controls the behavior of that input because it will determine what kind of input it is. If no type is specified, it will automatically create a text input, or a single-line text box
  - ex: type= "text", "password", "textarea", "radio", "checkbox", "file", "submit", "image", "hidden", "date", "email", "search"

2. What element is used to create a dropdown list?
  - The <select> element is used to create a dropdown list, meanwhile the <option> element is used to create the options the user can choose from
  - multiple="multiple" attribute can be used to allow the user to select multiple options within the dropdown list

3. If you're using an input element to send form data to a server, what should the type attribute be set to?
  - method="post" is the attribute that should be used when an input element needs to send form data to a server
  - method="get" is the attribute that should be used when you are just retrieving form data from the web server
  - if method="post" is not used, method="get" effects will be defaulted to the input element

4. What element is used to group similar form items together?
  - The <fieldset> element is used to group similar form items together
  - <fieldset> can take few attributes: disabled="", form="", and name=""
  - desiabled="" if assigned, all form controls within <fieldset> will be disabled
  - form="" takes the value of the id attribute of a <form> element you want the <fieldset> to be apart of, even if it's not inside them
    * Please note: if you want the <input> elements inside the <fieldset> to be associated with the form, you need to use the form attribute directly on those elements
  - name="" is the name associated with the group


### Chapter 13 + 15 - Boxes + Layouts:

1. Describe the differences between border, margin, and padding:
  - Border is the literal "box" that CSS puts each HTML element into. Borders by default will be transparent and 0px wide
  - Margin is the distance outside of the border between adjacent elements
  - Padding is the distance between the contents inside of the box and the border of the box

2. For a CSS rule padding: 1px 2px 5px 10px, what sides of the content box does each pixel value correspond to?
  - Clockwise order: top, right, bottom, left

3. Describe the difference between block-level and inline elements:
  - Block-level elements are elements that are defaulted to start on the next new line on the webpage
  - Block-level elements will always take up the full width of the webpage
  - Block-level elements have top and bottom margins
    * ex: <div>, <h1>, <p>, <ul>, <li>
  - Inline elements are elements that can flow around text, not required to start a new line on the webpage
  - Inline elements will only take up as much space as necessary
  - Inline elements do not have top and bottom margins
    * ex: <span>, <img>, <b>, <i>

4. What is the role of fixed positioning, and why is z-index important in the scenario of using fixed positioning?
  - An element with a fixed position means it always stays in the same place even when the page is scrolled
  - A fixed element does not leave a gap in the page where it normally would have been located
  - Top, Right, Bottom, Left properties are used to position the element
  - The z-index property in CSS controls the vertical stacking order of elements that overlap, as in which one appears physically closer to you
  - Without a z-index value, static/fixed elements will appear in the order they appear in the DOM

5. What is the difference between a fixed and liquid layout?
  - A liquid layout would allow those elements to move while the page is scrolled


[Day 3 CodePen Completed](https://codepen.io/alexmfritz/pen/qBjKPbW)

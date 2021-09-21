# HTML & CSS: Design and Build Websites

1. On a website, what is the purpose of HTML code?
  - You can think of HTML as the skeleton/bare bones of the website. This is where you write all of your text, import your links, images, and anything else that providing information to the user. Here, you format them simply into things like headers, paragraphs, sections, or groups.

2. What is the difference between an element and a tag?
  - A *tag* is used to open and close various pieces of data in HTML into a specific segment or style of info
    - ex: <h> </hr> or <p> </p>, the tags tell the user what **kind** of information is being show(paragraph, header, image, etc)
    - All close tags will include the same characters as opener, prefaced by a backslash /
  - An *element* is the entire line of code, including both open/close tags and everything inbetween
    - ex: <h>Hello World!</h>, ALL of that is an element
    - ex: <p>This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph.</p>

3. Why do we use attributes in HTML elements?
  - HTML element attributes allow us to provide additional information about elements
  - They are always specified within the start tag of the element and typically come in the form of name/value pairs (ex: name="value")
  - ex: the <a> tag defines a hyperlink, meanwhile the href attribute specifies the URL of the page that the link goes to

4. Describe the purpose of the head, title, and body HTML elements:
  - The *Head* element is the first part of an HTML document that is used to import additional information into the document.
    - Head contains meta information, the title of the page, internal style, internal JavaScript, external JavaScript file linking
    - There should only ever be one Head in an HTML document, it's never required but highly recommended
    - The Head is NOT used to add information to the HTML document
  - The *body* element is the second part of the HTML document that contains the content of the page
    - The Body contains things like <header>, <section>, <article>, <p>, <img>, <table>
  - The *title* element is found within the Head element and the text within the Title will be shown on the browsers title bar/page's tab
    - Text-only, tags within the element are ignored

5. In your browser (Chrome), how do you view the source of the website?
  - Right click on page, click View source

6. List five different HTML elements and their purpose:
  - The <header> element, not to be confused with <title>, is used to head the page. It will be the largest text at the very top of the page that will create the title of the webpage itself (not the tab)
  - The <img> element is used to embed an image into the browswer via an image source URL or a file, also including caption text that will only be visible if the image fails to load on render
  - The <a> element is used to turn a block of text into a link, including an href="" attribute to invoke the URL
  - The <h1> through <h6> elements are a sort of section header that scales in size depending on which number is used. <h1> is the largest, <h6> is the smallest
  - The <footer> element is typically used for the final section of information passed through the HTML document. Information found in here usually is related to the author, copyright data, or links to related documents.

7. What are empty elements?
  - Empty elements are elements that contain no content and should not use a close tag
  - The <br> element defines a line break, does not require a close tag

8. What is semantic markup?
  - To use a word semantically is to use it in a way that is properly aligned with the meaning of the word
  - HTML tags have semantic meaning, therefore the element itself conveys information about the type of content
  - Semantic markup requires two practices:
    * HTML elements be used according to their intended purpose
    * The separation of content and presentation
  - Using HTML elements correctly means we are not only using the correct tags that correspond with the content, but they are also human-readable AND machine-readable
  - Seperating content and presentation means using HTML to provide content, and CSS to make changes to the presentation of that content
  - Define "semantic markup": Semantic markup is the use of a markup language such as HTML to convey information about the meaning of each element in a document through proper selection of markup elements, and to maintain complete separation between the markup and the visual presentation of the elements contained in the document.

9. What are three new semantic markup elements introduced in HTML5?
  - <article>
  - <figure>
  - <footer>
  - <header>
  - <main>
  - <nav>
  - <summary>
  - https://www.freecodecamp.org/news/semantic-html5-elements/


[CODE PEN ACTIVITY](https://codepen.io/alexmfritz/pen/qBjKPbW)

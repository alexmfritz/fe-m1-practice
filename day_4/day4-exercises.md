## Chapter 5: Images

1. In an image element, why is the alt attribute important?
  - The alt="" attribute is extremely important when adding images to your webpage because it provides a detailed description of the contents of the image in case the image does not load on render. It's also known as "alt text" and will provide information to screen reader software for those that are visually impaired, as well as search engines.

2. What determines if an image element is inline or block?
  - The image element is considered inline or block-level based on where the element is placed compared to text or other block-level elements. If the image element is placed BEFORE a block-level element then the image will also be a block-level element and any sibling elements will automatically default to starting on the next line. If the image element is placed within a block-level element, like a <p>, it will act as an inline element and the text will flow around it. That being said, the text will need help flowing around it appropriately with other attributes such as align="" and others

3. What are the benefits of jpg or png image file formats?
  - The biggest benefit of using JPEG is the fact that it can handle large groups of colors very well. If you are dealing with photos that are heavily multicolored, editing jpg images are much better
    - The biggest downside to JPEG is when you start to downsize an image too far, the process of downsizing means jpg files will begin grouping "similar" colors together and can cause a major loss in quality
  - The biggest benefit of using PNG is the compression of those files is lossless, meaning that no matter how many times you edit and resave the file, the quality of the image is the same.


## Chapter 16: Images

1. What is the benefit of specifying the height and width of images in CSS compared to specifying in the HTML?
  - The benefit of specifying images in CSS allows you to determine sizing for large groups of images across multiple pages of your site. It is *good* practice to determine 2-3 common sizes you will use for images across your entire site (ex: small, medium, large) and then appropriately assign each image a class="size" in HTML so you can size ALL of that class within CSS
2. What is an image sprite, and why is it useful?
  - A sprite is when a single image is used over several different parts of the the size. One example of this is taking the image of a companies logo and incorporating it into all the different buttons or bullet points throughout the site. The benefit is that the browser only needs to search and load **one** image instead of many, allowing the site to render faster and smoother.

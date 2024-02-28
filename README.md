# HTML

## 1. What is HTML?

-> HTML is a acronym of HyperText Markup Language. It is the standard markup language for creating web pages.

HyperText refers to links that connect web pages to one another, either a single website or between websites. Links are a fundamental aspect of the Web.

HTML uses Markup to annotate text, images and other contents for display in a web browser

## Lesson-1-HTML Structure

---

what is tag and element?

-: In HTML (Hypertext Markup Language), a "tag" is a keyword or abbreviation enclosed within angle brackets (< and >) that specifies how a particular element should be formatted or displayed on a web page. Tags are fundamental building blocks of HTML and are used to define the structure and content of a webpage.

-: An "element" in HTML consists of a pair of tags and the content enclosed within them. There are two types of elements:

1. Empty Elements: These elements do not have any content between opening and closing tags. For example, the img tag for displaying images or the br tag for line breaks.
   Example:

   ```html
   <img src="image.jpg" alt="Description" />
   ```

2. Container Elements: These elements have an opening tag, content, and a closing tag. Content can include text, other elements, or multimedia. Common container elements include headings (h1, h2, etc.), paragraphs (p), lists (ul, ol, li), and divs (div).

   Example:

   ```html
   <p>This is a paragraph element.</p>
   ```

-: In HTML, the head section of a document contains metadata, which provides information about the HTML document itself. Metadata typically includes data such as the title of the document, character encoding, stylesheets, scripts, and other important information about the document. This metadata is not displayed directly on the webpage but instead provides essential information to browsers, search engines, and other web services.

### HTML Structure

The basic structure of an HTML document consists of several key elements that define its content, structure, and presentation. Here's a breakdown of the basic structure:

1. **Document Type Declaration (DOCTYPE)**: The `<!DOCTYPE>` declaration is not an HTML tag; rather, it informs the browser which version of HTML the document is written in. It should be placed at the very beginning of the HTML document.

   Example:

   ```html
   <!DOCTYPE html>
   ```

2. **HTML Element**: The `<html>` element is the root element of an HTML document. All other elements are nested inside it.

   Example:

   ```html
   <html>
     <!-- Content goes here -->
   </html>
   ```

3. **Head Section**: The `<head>` element contains metadata about the HTML document, such as the title, character encoding, stylesheets, scripts, and other important information. This section is not displayed on the webpage itself.

   Example:

   ```html
   <head>
     <title>My Website</title>
     <meta charset="UTF-8" />
     <link rel="stylesheet" type="text/css" href="styles.css" />
   </head>
   ```

4. **Body Section**: The `<body>` element contains the content of the HTML document that is displayed in the browser window. This is where you put text, images, links, and other elements that you want to appear on the webpage.

   Example:

   ```html
   <body>
     <h1>Welcome to My Website</h1>
     <p>This is a paragraph of text.</p>
     <img src="image.jpg" alt="Description" />
     <!-- Other content goes here -->
   </body>
   ```

5. **Elements and Tags**: Inside the `<body>` section, you can include various HTML elements and tags to structure and format your content. Elements can be nested within each other to create a hierarchical structure.

   Example:

   ```html
   <h1>This is a heading</h1>
   <p>This is a paragraph of text.</p>
   <ul>
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ul>
   ```

This basic structure outlines the essential components of an HTML document. It provides a framework for organizing content and presenting it on the web.

---

## Lesson-2-Text Basics

---

In HTML and CSS, elements are classified into two main categories based on how they behave in the document flow: block-level elements and inline-level elements. Understanding these categories is crucial for controlling the layout and structure of a webpage.

### Block-Level Elements:-

1. **Definition:** Block-level elements are elements that typically start on a new line and occupy the full width available to them by default, extending from the left edge of their containing element to the right edge. They create a "block" of content.

2. **Examples:** Common block-level elements include headings (`<h1>` through `<h6>`), paragraphs (`<p>`), divs (`<div>`), lists (`<ul>`, `<ol>`, `<li>`), and structural elements like `<header>`, `<footer>`, `<section>`, `<article>`, and `<nav>`.

3. **Behavior:**
   - Block-level elements stack on top of one another vertically in the document flow.
   - By default, block-level elements will stretch to fill the width of their containing element unless a specific width is defined.
   - They can contain other block-level and inline-level elements, including other block-level elements.
   - Examples of block-level elements include elements that typically represent larger structural parts of the webpage.

### Inline-Level Elements:-

1. **Definition:** Inline-level elements are elements that do not start on a new line and only occupy the space bounded by the tags themselves. They flow alongside adjacent elements.

2. **Examples:** Common inline-level elements include spans (`<span>`), anchors (`<a>`), images (`<img>`), bold and italic text (`<strong>`, `<em>`), and most form elements like `<input>`, `<button>`, and `<select>`.

3. **Behavior:**
   - Inline-level elements do not force a new line to begin after them; they flow within the text or other inline-level elements.
   - They only take up as much width as necessary and do not start on a new line by default.
   - Inline-level elements cannot contain block-level elements, but they can contain other inline-level elements.
   - Examples of inline-level elements include elements that typically represent smaller parts of content or text-level semantics.

**Differentiation and Usage:**

- Block-level elements are often used to structure the layout and create larger sections of content on a webpage, such as headers, paragraphs, and sidebars.
- Inline-level elements are commonly used for smaller, more granular elements like text formatting, links, and inline images.

Understanding the distinction between block-level and inline-level elements is fundamental for creating well-structured and visually appealing web pages and for applying CSS styling effectively.

### Replaced inline elements

Replaced inline elements are inline elements that are replaced by external resources such as images, videos, etc. These elements behave more like block-level elements in terms of layout because they have intrinsic dimensions or can have their dimensions explicitly set.
Note-: "intrinsic dimensions" specifically refer to the inherent width and height of certain elements, particularly replaced elements like images, videos, and other media.

### Non-replaced inline elements

Non-replaced inline elements on the other hand, are typically text-level elements that do not have intrinsic dimensions and are not directly controllable with width and height attributes. They flow within the text and their size is determined by the content they contain or the properties applied to them through CSS.

### HTML entity

An HTML entity is a sequence of characters that represents a special character or symbol in HTML markup. HTML entities are used to display characters that have special meaning in HTML or that cannot be easily typed on a keyboard, such as reserved characters like `<`, `>`, `&`, and non-breaking space (`&nbsp;`).

HTML entities are written using an ampersand (`&`) followed by a specific code or name representing the character, followed by a semicolon (`;`). The format is `&entity_name;` or `&#entity_number;`, where `entity_name` refers to the name of the entity, and `entity_number` refers to the numeric code of the entity in decimal.

For example:

- `&lt;` represents the less-than symbol `<`.
- `&gt;` represents the greater-than symbol `>`.
- `&amp;` represents the ampersand symbol `&`.
- `&nbsp;` represents a non-breaking space.
- `&copy;` represents the copyright symbol ©.
- `&#8364;` represents the Euro currency symbol € (using its numeric code).

HTML entities are commonly used when you want to display reserved characters as text rather than interpreted as part of the HTML markup. They are also useful for displaying characters in character sets that are not easily supported by the document's encoding.

For example, if you want to display a copyright symbol (`©`) in an HTML document, you would use the `&copy;` entity:

```html
<p>This document is protected by copyright &copy; 2024.</p>
```

This would render as:

"This document is protected by copyright © 2024."

HTML entities provide a way to include special characters and symbols in HTML documents without causing syntax errors or misinterpretations by the browser.

## Lesson-3-List Types

---

In HTML, there are several types of lists that you can use to organize and structure content. The main types of lists are:

1. **Ordered Lists (`<ol>`)**: Ordered lists are used to present a list of items in a specific order, typically indicated by sequential numbers or letters. Each item in the list is marked with an ordinal number or letter. Ordered lists are created using the `<ol>` element, and each list item is defined using the `<li>` (list item) element.

   Example:

   ```html
   <ol>
     <li>Item 1</li>
     <li>Item 2</li>
     <li>Item 3</li>
   </ol>
   ```

   Output:

   1. Item 1
   2. Item 2
   3. Item 3

   By default, ordered lists are displayed with decimal numbers, but you can change the numbering style using CSS.

2. **Unordered Lists (`<ul>`)**: Unordered lists are used to present a list of items in no particular order, typically indicated by bullet points. Each item in the list is marked with a bullet point. Unordered lists are created using the `<ul>` element, and each list item is defined using the `<li>` element.

   Example:

   ```html
   <ul>
     <li>Item A</li>
     <li>Item B</li>
     <li>Item C</li>
   </ul>
   ```

   Output:

   - Item A
   - Item B
   - Item C

   By default, unordered lists are displayed with bullet points, but you can change the bullet style using CSS.

3. **Description Lists (`<dl>`)**: Description lists are used to present a list of terms and their corresponding descriptions or definitions. Each term is defined using the `<dt>` (description term) element, and each description is defined using the `<dd>` (description details) element.

   Example:

   ```html
   <dl>
     <dt>Term 1</dt>
     <dd>Description 1</dd>
     <dt>Term 2</dt>
     <dd>Description 2</dd>
   </dl>
   ```

   Output:

   Term 1
   Description 1
   Term 2
   Description 2

   Description lists are often used for glossaries, metadata, or any situation where you need to pair terms with their explanations.

These are the main types of lists in HTML. You can use them to organize and structure content in various ways, depending on the requirements of your webpage. Additionally, you can style the appearance of lists using CSS to achieve the desired visual presentation.

## Lesson-4-Adding Links

---

In HTML, a link is an element that allows users to navigate between different webpages or resources. Links are created using the `<a>` (anchor) element and are one of the fundamental components of the web. Here's a discussion of links in HTML:

1. **Anchor Element (`<a>`)**:

   - The `<a>` element is used to create links in HTML.
   - It can point to different types of resources, including webpages, images, files, email addresses, and specific locations within a webpage (known as anchor links or internal links).
   - The `href` attribute specifies the URL or destination of the link.

2. **Link Text**:

   - The text enclosed within the opening and closing `<a>` tags is known as the link text. This is the visible part of the link that users click on.
   - It's important to choose descriptive and meaningful link text that accurately describes the destination of the link. This helps users understand where the link will take them.

3. **Absolute and Relative URLs**:

   - Links can use absolute URLs, which specify the complete web address (e.g., `https://www.example.com/page.html`), or relative URLs, which specify the path relative to the current webpage (e.g., `page.html`).
   - Absolute URLs are used when linking to resources on external websites, while relative URLs are used for links within the same website.

4. **Link Behavior**:

   - By default, clicking on a link opens the destination in the same browser window or tab. However, you can specify a different target using the `target` attribute. Common target values include `_blank` to open the link in a new tab and `_self` to open it in the same tab.
   - Additionally, you can use the `rel` attribute to specify the relationship between the current document and the linked document, such as `rel="nofollow"` to instruct search engines not to follow the link.

5. **Styling Links**:

   - Links can be styled using CSS to change their appearance, such as color, font, underline, and hover effects. Styling can help make links more visually appealing and prominent on the webpage.
   - The default styles for links vary between browsers, so it's common practice to override these styles with custom CSS to ensure consistency across different platforms.

6. **Accessibility**:
   - Links play a crucial role in web accessibility. It's important to ensure that links are easily identifiable and distinguishable from surrounding text, especially for users who rely on screen readers or keyboard navigation.
   - Providing descriptive link text and using semantic HTML elements (such as headings) can improve the accessibility of links for all users.

In summary, links are essential for navigating the web and connecting different webpages and resources. By using the `<a>` element with appropriate attributes and link text, you can create effective and accessible links within your HTML documents.

## Lesson-5-Images

---

### image format

1. **PNG (Portable Network Graphics)**:

   - **Quality**: High-quality images with sharp edges and text.
   - **Transparency**: Supports transparent backgrounds.
   - **Use Cases**: Logos, icons, graphics with transparency.

2. **JPG/JPEG (Joint Photographic Experts Group)**:

   - **Compression**: Smaller file sizes for photos.
   - **No Transparency**: Doesn't support transparent backgrounds.
   - **Use Cases**: Photographs, natural scenes, images with no transparency needed.

3. **SVG (Scalable Vector Graphics)**:
   - **Scalability**: Images can be resized without losing quality.
   - **Vector-Based**: Defined by shapes, not pixels.
   - **Interactive**: Supports interactivity and animation.
   - **Use Cases**: Icons, logos, graphics that need to be scalable or interactive.

In summary, PNG is best for graphics with sharp edges and transparency, JPG is ideal for photos and images with no transparency, while SVG is great for scalable and interactive graphics.

### names of image formats

The names of image formats like PNG, JPG/JPEG, and SVG may seem unfamiliar or "weird" at first, but they actually have logical explanations behind them:

1. **PNG (Portable Network Graphics)**:

   - **Portable**: The term "portable" in PNG refers to the format's portability across different platforms and systems. PNG was designed to be platform-independent and widely supported by various software and hardware.
   - **Network Graphics**: PNG was developed as a replacement for the GIF (Graphics Interchange Format) format, primarily for use on the internet and networked environments. The "network graphics" part of the name emphasizes its suitability for web graphics and online distribution.

2. **JPG/JPEG (Joint Photographic Experts Group)**:

   - **Joint Photographic**: The "Joint Photographic" part of the name refers to the collaboration of experts from various fields, including photography, graphics, and technology, who contributed to the development of the JPEG format.
   - **Experts Group**: The term "Experts Group" denotes the organization responsible for creating and standardizing the JPEG format, known as the Joint Photographic Experts Group.

3. **SVG (Scalable Vector Graphics)**:
   - **Scalable**: SVG stands for "Scalable Vector Graphics." The term "scalable" highlights one of the key features of SVG, which is its ability to scale to any size without losing quality. Vector graphics, as opposed to raster graphics (like PNG and JPG), are defined by mathematical equations and can be scaled infinitely without loss of detail.
   - **Vector Graphics**: The "Vector Graphics" part of the name emphasizes the format's use of geometric shapes (vectors) to represent images, allowing for smooth scalability and efficient representation of graphics.

While the names of these image formats may seem arbitrary or technical, they actually provide insights into their purpose, development history, and key features. Understanding the meaning behind the names can help demystify these image formats and provide context for their usage in digital media.

### 'alt` attribute

The purpose of the `alt` attribute in an image element (`<img>`) is to provide alternative text that describes the content or function of the image. The `alt` attribute serves several important purposes:

1. **Accessibility**: The primary purpose of the `alt` attribute is to improve web accessibility for users who may not be able to see the image. Screen reader software used by visually impaired users will read out the content of the `alt` attribute, allowing them to understand the context and meaning of the image.

2. **Fallback Content**: If an image fails to load for any reason (slow internet connection, broken link, etc.), the text provided in the `alt` attribute will be displayed in place of the image. This ensures that users still receive relevant information even if the image cannot be displayed.

3. **SEO (Search Engine Optimization)**: Search engines use the `alt` attribute to understand the content and context of images on a webpage. Providing descriptive and relevant text in the `alt` attribute can improve the accessibility and search engine ranking of your webpage.

4. **Contextual Information**: The `alt` attribute allows you to provide additional context or information about the image that may not be apparent from the visual content alone. This can be especially useful for images that convey important information or serve a specific function within the webpage.

When writing the `alt` attribute for an image, it's important to follow these best practices:

- Be descriptive: Provide a concise and accurate description of the image content or function.
- Avoid redundancy: Don't repeat information that is already present in the surrounding text or other nearby images.
- Keep it relevant: Focus on the most important aspects of the image that convey its purpose or meaning.
- Use keywords: Incorporate relevant keywords that help improve the image's SEO value and relevance to the webpage content.

Here's an example of how the `alt` attribute is used in an image element:

```html
<img src="example.jpg" alt="A red apple on a wooden table" />
```

In this example, the `alt` attribute describes the content of the image, which is a red apple on a wooden table.

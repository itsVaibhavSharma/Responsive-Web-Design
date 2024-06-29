# Responsive-Web-Design

HTML elements have an opening and closing tag with content in between.
Here is the basic syntax:
```html
<openingTag>content</closingTag>
```

#### Heading
The first element you will learn about is the `h1` element. The `h1` element is a heading element and is used for the main heading of a webpage.

```html
<h1>This is a main heading</h1>
```

```html
<html>

  <body>

    <h1>Hello World</h1>

  </body>

</html>
```

The `h1` through `h6` heading elements are used to signify the importance of content below them. The lower the number, the higher the importance, so `h2` elements have less importance than `h1` elements.

```html
<h1>most important heading element</h1>
<h2>second most important heading element</h2>
<h3>third most important heading element</h3>
<h4>fourth most important heading element</h4>
<h5>fifth most important heading element</h5>
<h6>least important heading element</h6>
```

Only use one `h1` element per page and place lower importance headings below higher importance headings.

#### Paragraph
The `p` element is used to create a paragraph of text on websites.
```html
<p>See more cat photos in our gallery.</p>
```

#### Comments
Commenting allows you to leave messages without affecting the browser display. It also allows you to make code inactive. A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.

Here is an example of a comment with the `TODO: Remove h1`:

```html
<!-- TODO: Remove h1 -->
```

#### main element
HTML5 has some elements that identify different content areas. These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.

The `main` element is used to represent the main content of the body of an HTML document. Content inside the `main` element should be unique to the document and should not be repeated in other parts of the document.

Example Code

```html
<main>
  <h1>Most important content of the document</h1>
  <p>Some more important content...</p>
</main>
```

In the previous step, you put the `h1`, `h2`, comment, and `p` elements inside the `main` element. This is called _nesting_. Nested elements should be placed two spaces further to the right of the element they are nested in. This spacing is called indentation and it is used to make HTML easier to read.

#### Images
You can add images to your website by using the `img` element. `img` elements have an opening tag without a closing tag. A tag for an element without a closing tag is known as a self-closing tag.

HTML attributes are special words used inside the opening tag of an element to control the element's behavior. The `src` attribute in an `img` element specifies the image's URL (where the image is located).

Here is an example of an `img` element with a `src` attribute pointing to the freeCodeCamp logo:

Example Code

```html
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_secondary.svg">
```
All `img` elements should have an `alt` attribute. The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.

Here is an example of an `img` element with an `alt` attribute:

```html
<img src="cat.jpg" alt="A cat">
```

#### Link (anchor tag)
You can link to another page with the anchor (`a`) element.
Here is an example linking to `https://www.freecodecamp.org`:

```html
<a href="https://www.freecodecamp.org"></a>
```
A link's text must be placed between the opening and closing tags of an anchor (`a`) element.
Here is an example of a link with the text `click here to go to freeCodeCamp.org`:

```html
<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>
```

You can turn any text into a link, such as the text inside of a `p` element.

```html
<p>I think <a href="https://www.freecodecamp.org">freeCodeCamp</a> is great.</p>
```

To open links in a new tab, you can use the `target` attribute on the anchor (`a`) element.

The `target` attribute specifies where to open the linked document. `target="_blank"` opens the linked document in a new tab or window.

Here is the basic syntax for an `a` element with a `target` attribute:

```html
<a href="https://www.freecodecamp.org" target="_blank">freeCodeCamp</a>
```

In previous steps you used an anchor element to turn text into a link. Other types of content can also be turned into a link by wrapping it in anchor tags.

Here is an example of turning an image into a link:

```html
<a href="example-link">
  <img src="image-link.jpg" alt="A photo of a cat.">
</a>
```

#### section element
Before adding any new content, you should make use of a `section` element to separate the cat photos content from the future content.

The `section` element is used to define sections in a document, such as chapters, headers, footers, or any other sections of the document. It is a semantic element that helps with SEO and accessibility.

Example Code

```html
<section>
  <h2>Section Title</h2>
  <p>Section content...</p>
</section>
```

### List
To create an unordered list of items, you can use the `ul` element.

The `li` element is used to create a list item in an ordered or unordered list.
Here is an example of list items in an unordered list:

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

The code for an ordered list (`ol`) is similar to an unordered list, but list items in an ordered list are numbered when displayed.
```html
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>
```
#### figure element
The `figure` element represents self-contained content and will allow you to associate an image with a caption.

A figure caption (`figcaption`) element is used to add a caption to describe the image contained within the `figure` element.

Here is an example of a `figcaption` element with the caption of `A cute cat`:

```html
<figure>
  <img src="image.jpg" alt="A description of the image">
  <figcaption>A cute cat</figcaption>
</figure>
```

#### Emphasize
To place emphasis on a specific word or phrase, you can use the `em` element.
```html
 <figcaption>Cats <em>love</em> lasagna.</figcaption>
```

#### strong element
The `strong` element is used to indicate that some text is of strong importance or urgent.
```html
<figcaption>Cats <strong>hate</strong> other cats.</figcaption>
```

#### Form
Now you will add a web form to collect information from users.
The `form` element is used to get information from a user like their name, email, and other details.

The `action` attribute indicates where form data should be sent.

Here is an example of a `form` element with an `action` attribute:

```html
<form action="/submit-url"></form>
```

In the example, `action="/submit-url"` tells the browser that the form data should be sent to the path `/submit-url`.

The `input` element allows you several ways to collect data from a web form. Like `img` elements, `input` elements are self-closing and do not need closing tags.
There are many kinds of inputs you can create using the `type` attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer.

In order for a form's data to be accessed by the location specified in the `action` attribute, you must give the text field a `name` attribute and assign it a value to represent the data being submitted.

Here is an example of an `input` element with a `name` attribute:

```html
<input type="text" name="name">
```
Placeholder text is used to give people a hint about what kind of information to enter into an input.

Here is an example of an `input` element with a placeholder set to `Ex. Jane Doe`:

```html
<input type="text" placeholder="Ex. Jane Doe">
```

To prevent a user from submitting your form when required information is missing, you need to add the `required` attribute to an `input` element. There's no need to set a value to the `required` attribute. Instead, just add the word `required` to the `input` element, making sure there is space between it and other attributes.

```html
<input type="text" name="catphotourl" placeholder="cat photo URL" required>
```

The `button` element is used to create a clickable button.
```html
<button>Submit</button>
```
Even though you added your button below the text input, they appear next to each other on the page. That's because both `input` and `button` elements are inline elements, which don't appear on new lines.

The button you added will submit the form by default. However, relying on default behavior may cause confusion. Add the `type` attribute with the value `submit` to the `button` to make it clear that it is a submit button.

```html
<button type ="submit">Submit</button>
```

You can use radio buttons for questions where you want only one answer out of multiple options.

Here is an example of a radio button with the option of `cat`:

```html
<input type="radio"> cat
```

Remember that `input` elements are self-closing.

`label` elements are used to help associate the text for an `input` element with the `input` element itself (especially for assistive technologies like screen readers).

Here is an example of a `label` element with a `radio` button:

```html
<label><input type="radio"> cat</label>
```

The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other `id` values for the entire page.

Here is an example of an `input` element with an `id` attribute:

```html
<input id="email">
```

Notice that both radio buttons can be selected at the same time. To make it so selecting one radio button automatically deselects the other, both buttons must have a `name` attribute with the same value.

Here is an example of two radio buttons with the same `name` attribute:

```html
<input type="radio" name="meal"> Breakfast
<input type="radio" name="meal"> Lunch
```

If you select the `Indoor` radio button and submit the form, the form data for the button is based on its `name` and `value` attributes. Since your radio buttons do not have a `value` attribute, the form data will include `indoor-outdoor=on`, which is not useful when you have multiple buttons.
Add a `value` attribute to both radio buttons. For convenience, set the button's `value` attribute to the same value as its `id` attribute.

```html
<label><input value="indoor" id="indoor" type="radio" name="indoor-outdoor"> Indoor</label>

<label><input value="outdoor" id="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
```

The `fieldset` element is used to group related inputs and labels together in a web form. `fieldset` elements are block-level elements, meaning that they appear on a new line.

The `legend` element acts as a caption for the content in the `fieldset` element. It gives users context about what they should enter into that part of the form.

```html
<fieldset>

<legend>Is your cat an indoor or outdoor cat?</legend>

<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>

<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>

</fieldset>
```

Forms commonly use checkboxes for questions that may have more than one answer. The `input` element with a `type` attribute set to `checkbox` creates a checkbox.

```html
<input type="checkbox"> Loving
```

There's another way to associate an `input` element's text with the element itself. You can nest the text within a `label` element and add a `for` attribute with the same value as the `input` element's `id` attribute.

Here is an example of using the `for` attribute to associate a `label` with an `input` element:

```html
<label for="breakfast"> Breakfast </label>
<input id="breakfast" type="radio" name="meal" value="breakfast">
```

Like radio buttons, form data for selected checkboxes are `name` / `value` attribute pairs. While the `value` attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.

In order to make a checkbox checked or radio button selected by default, you need to add the `checked` attribute to it.

Here is an example of a radio button with the `checked` attribute:

```html
<input checked type="radio" name="meal" value="breakfast"> Breakfast
```

There's no need to set a value to the `checked` attribute. Instead, just add the word `checked` to the `input` element, making sure there is space between it and other attributes.

#### Footer
The `footer` element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.
```html
<footer>
	<p>No copyright: @itsVaibhavSharma</p>
</footer>
```

#### Header
Notice that everything you've added to the page so far is inside the `body` element. All page content elements that should be rendered to the page go inside the `body` element. However, other important information goes inside the `head` element.

The `head` element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page.

The `title` element determines what browsers show in the title bar or tab for the page.

```html
<head>
    <title>CatPhotoApp</title>
</head>
```

You can set browser behavior by adding self-closing `meta` elements in the `head`. Here's an example:

```html
<meta attribute="value">
```

Inside the `head` element, nest a `meta` element with an attribute named `charset`. Set to the value to `utf-8` which tells the browser how to encode characters for the page.

Note that `meta` elements are self-closing.

```html
<meta charset="utf-8">
```
#### Html Tag
Notice that the entire contents of the page are nested within an `html` element. The `html` element is the root element of an HTML page and wraps all content on the page.
You can also specify the language of your page by adding the `lang` attribute to the `html` element.

All pages should begin with `<!DOCTYPE html>`. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.
`<!DOCTYPE html>` tells browsers that the document is an HTML5 document which is the latest version of HTML.

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset = "utf-8">
		<title></title>
	</head>
	<body>
		<main>
		</main>
		<footer>
		</footer>
	</body
</html
```

# CSS (Cascading Style Sheet)
Up until now, you have been limited regarding the presentation and appearance of the content you create.

```html
<head>
	<style>
	</style>
</head>
```

You can add style to an element by specifying it in the `style` element and setting a property for it like this:

```css
element {
 property: value;
}
```

#### Type selector and Center Align
```html
 <style>
      h1 {
        text-align : center;
      }
    </style>
```

You now have three type selectors with the exact same styling. You can add the same group of styles to many elements by creating a list of selectors. Each selector is separated with commas like this:

Example Code

```css
selector1, selector2 {
  property: value;
}
```

### Separate CSS file
Instead of writing the css code in the same file, it is better to create a different CSS file for styling.
Lets create a styles.css.

Make sure to exclude the opening and closing `style` tags.

Now you need to link the `styles.css` file, so the styles will be applied again. Inside the `head` element, add a `link` element. Give it a `rel` attribute with the value of `"stylesheet"` and a `href` attribute with the value of `"styles.css"`.

```html
<head>
    <meta charset="utf-8" />
    <title>Title</title>
    <link rel="stylesheet" href="styles.css">
  </head>
```

For the styling of the page to look similar on mobile as it does on a desktop or laptop, you need to add a `meta` element with a special `content` attribute.

Add the following within the `head` element:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

### Properties
```CSS
background-color: brown;
width: 300px; /*fixed */
width: 80%; /*80% of the entire screen*/
max-width: 500px;

text-align: left / center / right;

/*center horizontally*/
margin-left : auto;
margin-right: auto;

/*Background image*/
background-image : url(https://cdn.freecodecamp.org/curriculum/css-cafe/beans.jpg);

/*Making an element inline*/
display : inline-block;

/*making an element behave as block*/
display: block;

/*padding*/
padding-left: 20px;
padding-right: 20px;
padding-top: 20px;
padding-bottom: 20px;
/*or only below for padding all side*/
padding: 20px;

/*Font*/
font-family: sans-serif | Impact (for headings) ;

/*You can add a fallback value for the font-family by adding another font name separated by a comma. Fallbacks are used in instances where the initial is not found/available.*/
font-family: Impact, serif;

/* Style */
font-style: italic;

font-size: 40px; 

/* For hr elements*/
height: 2px;
background-color: brown;
border-color: brown;

/* To reduce top margin, There is an easier way, simply add a negative top margin to the `img` elements to pull them up from their current positions. Negative values are created using a `-` in front of the value.*/
margin-top: -25px;

```


#### Div
The `div` element is used mainly for design layout purposes unlike the other content elements you have used so far.

```html
<div>
</div>
```
The goal now is to make the `div` not take up the entire width of the page. The CSS `width` property is perfect for this.

You can use the `id` selector to target a specific element with an `id` attribute. An `id` selector is defined by placing the hash symbol `#` directly in front of the element's `id` value. For example, if an element has the `id` of `cat` then you would target that element like this:

```css
#cat {
  width: 250px;
}
```

#### Comment
Comments in CSS look like this:

```css
/* comment here */
```


#### Margin
Next, you want to center the `#menu` horizontally. You can do this by setting its `margin-left` and `margin-right` properties to `auto`. Think of the margin as invisible space around an element.

```css
margin-left : auto;
margin-right: auto;
```

#### Class Selector
So far you have been using type and id selectors to style elements. However, it is more common to use a different selector to style your elements.

A class selector is defined by a name with a dot directly in front of it, like this:

Example Code
```html
<div class = "class-name"></div>
```

```css
.class-name {
  styles
}
```

#### Article
`article` elements commonly contain multiple elements that have related information.
```html
<article>
</article>
```

#### Styling Nested elements
The `p` elements are nested in an `article` element with the class attribute of `item`. You can style all the `p` elements nested anywhere in elements with a class named `item` like this:

Example Code

```css
.item p { }
```

#### Making inline
 Instead, use the back space key on your keyboard to move the `p` element with the class `price` next to the `p` element with the class `flavor` so that they are on the same line in the editor. Make sure there is no space between the two elements.
 ```html
 <article class="item">
	<p class="flavor">French Vanilla</p><p class="price">3.00</p>
 </article>
```

```css
.item p {
  display: inline-block;
}
  
.flavor {
  text-align: left;
  width: 50%;
}
  
.price {
  text-align: right;
  width: 50%;
}
```

#### hr element
You can use an `hr` element to display a divider between sections of different content.
Note that `hr` elements are self closing.
```html
<hr>
```
The default properties of an `hr` element will make it appear as a thin light grey line. You can change the height of the line by specifying a value for the `height` property.

```css
hr {
  height: 3px;
}
```

Notice the grey color along the edges of the line. Those edges are known as borders. Each side of an element can have a different color or they can all be the same.

Notice how the thickness of the line looks bigger? The default value of a property named `border-width` is `1px` for all edges of `hr` elements. By changing the border to the same color as the background, the total height of the line is `5px` (`3px` plus the top and bottom border width of `1px`).

```css
hr {
  height: 2px;
  background-color: brown;
  border-color: brown;
}
```

#### Styling link elements
The default color of a link that has not yet been clicked on is typically blue. The default color of a link that has already been visited from a page is typically purple.

To make the `footer` links the same color regardless if a link has been visited, use a type selector for the anchor element (`a`) and use the value `black` for the `color` property.
```css
a {
  color: black;
}
```

You change properties of a link when the link has actually been visited by using a pseudo-selector that looks like `a:visited { propertyName: propertyValue; }`.
```css
a:visited {
  color: grey;
}
```

You change properties of a link when the mouse hovers over them by using a pseudo-selector that looks like `a:hover { propertyName: propertyValue; }`.
```css
a:hover {
  color: brown;
}
```

You change properties of a link when the link is actually being clicked by using a pseudo-selector that looks like `a:active { propertyName: propertyValue; }`.
```css
a:active{
  color: white;
}
```

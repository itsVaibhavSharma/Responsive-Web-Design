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
Remember that the `title` element gives search engines extra information about the page. It also displays the content of that `title` element in two more ways:

- in the title bar when the page is open
- in the browser tab for the page when you hover on it. Even if that tab is not active, once you hover on the tab, the `title` text is displayed.
You can set browser behavior by adding self-closing `meta` elements in the `head`.

```html
<meta attribute="value">
```

Inside the `head` element, nest a `meta` element with an attribute named `charset`. Set to the value to `utf-8` which tells the browser how to encode characters for the page.

Note that `meta` elements are self-closing.

```html
<meta charset="utf-8">
```
To tell browsers how to encode characters on your page, set the `charset` to `utf-8`. `utf-8` is a universal character set that includes almost every character from all human languages.
```html
<meta name = "viewport" content="width=device-width, initial-scale=1.0">
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

/*styling and coloring a div*/
background-color: red;
height: 25px;
width: 200px;
margin: auto;
margin: 10px auto; /*When the shorthand `margin` property has two values, it sets `margin-top` and `margin-bottom` to the first value, and `margin-left` and `margin-right` to the second value.*/
padding: 10px 0px;

background-color: rgb(0,0,0); /*black*/
background-color: rgb(0, 127, 0); /* green equivalent*/
background-color: rgb(255, 255, 255); /*white*/
/*Secondary*/
background-color: rgb(255, 255, 0); /*yellow */
background-color: rgb(0, 255, 255); /*cyan*/
background-color: rgb(255, 0, 255); /*magenta*/
/*Tertiary*/
background-color: rgb(255, 127, 0); /*orange*/
background-color: rgb(0, 255, 127); /*springgreen*/
background-color: rgb(127, 0, 255); /*violet*/
background-color: rgb(127, 255, 0); /*chartreuse green*/
background-color: rgb(0, 127, 255); /*azure*/
background-color: rgb(255, 0, 127); /*rose*/

  

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

#### Multiple classes
To give the markers different colors, you will need to add a unique class to each one. Multiple classes can be added to an element by listing them in the `class` attribute and separating them with a space. For example, the following adds both the `animal` and `dog` classes to a `div` element.

Example Code

```html
<div class="animal dog">
```

If you add multiple classes to an HTML element, the styles of the first classes you list may be overridden by later classes.

#### Coloring 
There are two main color models: the additive RGB (red, green, blue) model used in electronic devices, and the subtractive CMYK (cyan, magenta, yellow, black) model used in print.

In this project, you'll work with the RGB model. This means that colors begin as black, and change as different levels of red, green, and blue are introduced. An easy way to see this is with the CSS `rgb` function.

```css
background-color: rgb(0,0,0);
```
A function is a piece of code that can take an input and perform a specific action. The CSS `rgb` function accepts values, or arguments, for red, green, and blue, and produces a color:

Example Code

```css
rgb(red, green, blue);
```

##### Primary Colors
Each red, green, and blue value is a number from `0` to `255`. `0` means that there's 0% of that color, and is black. `255` means that there's 100% of that color.

```css
rgb(255, 0, 0); //red
rgb(0, 255, 0); //green
rgb(0, 0, 255); //blue

background-color: green; //darker than rgb(0,255,0);

```
While the red and blue markers look the same, the green one is much lighter than it was before. This is because the `green` color keyword is actually a darker shade, and is about halfway between black and the maximum value for green.

##### Secondary Colors
Secondary colors are the colors you get when you combine primary colors.
```css
background-color: rgb(255, 255, 0); /*yellow */
background-color: rgb(0, 255, 255); /*cyan*/
background-color: rgb(255, 0, 255); /*magenta*/
```

##### Tertiary Colors
Now that you're familiar with secondary colors, you'll learn how to create tertiary colors. Tertiary colors are created by combining a primary with a nearby secondary color.

```css
background-color: rgb(255, 127, 0); /*orange*/
background-color: rgb(0, 255, 127); /*springgreen*/
background-color: rgb(127, 0, 255); /*violet*/
background-color: rgb(127, 255, 0); /*chartreuse green*/
background-color: rgb(0, 127, 255); /*azure*/
background-color: rgb(255, 0, 127); /*rose*/
```

##### Color wheel
A color wheel is a circle where similar colors, or hues, are near each other, and different ones are further apart. For example, pure red is between the hues rose and orange.

Two colors that are opposite from each other on the color wheel are called complementary colors. If two complementary colors are combined, they produce gray. But when they are placed side-by-side, these colors produce strong visual contrast and appear brighter.

```css
.one {
  background-color: rgb(255, 0, 0);
}
  
.two {
  background-color: rgb(0, 255, 255);
}
```
Notice that the red and cyan colors are very bright right next to each other. This contrast can be distracting if it's overused on a website, and can make text hard to read if it's placed on a complementary-colored background.

It's better practice to choose one color as the dominant color, and use its complementary color as an accent to bring attention to certain content on the page.

```css
.one {
  background-color: rgb(0, 0, 0);
}
  
.two {
  background-color: rgb(255, 0, 0);
}
  
.three {
  background-color: rgb(0, 0, 0);
}
```
Notice how your eyes are naturally drawn to the red color in the center? When designing a site, you can use this effect to draw attention to important headings, buttons, or links.

##### Hex Values
A very common way to apply color to an element with CSS is with hexadecimal or hex values. While hex values sound complicated, they're really just another form of RGB values.

Hex color values start with a `#` character and take six characters from 0-9 and A-F. The first pair of characters represent red, the second pair represent green, and the third pair represent blue. For example, `#4B5320`.

```css
background-color: #00FF00; /*green */

```
You may already be familiar with decimal, or base 10 values, which go from 0 - 9. Hexadecimal, or base 16 values, go from 0 - 9, then A - F:

Example Code

```js
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F
```

With hex colors, `00` is 0% of that color, and `FF` is 100%. So `#00FF00` translates to 0% red, 100% green, and 0% blue, and is the same as `rgb(0, 255, 0)`.

##### HSL
The HSL color model, or hue, saturation, and lightness, is another way to represent colors.

The CSS hsl function accepts 3 values: a number from 0 to 360 for hue, a percentage from 0 to 100 for saturation, and a percentage from 0 to 100 for lightness.

If you imagine a color wheel, the hue red is at 0 degrees, green is at 120 degrees, and blue is at 240 degrees.

Saturation is the intensity of a color from 0%, or gray, to 100% for pure color. You must add the percent sign `%` to the saturation and lightness values.

Lightness is how bright a color appears, from 0%, or complete black, to 100%, complete white, with 50% being neutral.

```css
background-color: hsl(240, 100%, 50%); /*blue*/
```

##### gradient
You've learned a few ways to set flat colors in CSS, but you can also use a color transition, or gradient, on an element.

A gradient is when one color transitions into another. The CSS `linear-gradient` function lets you control the direction of the transition along a line, and which colors are used.

One thing to remember is that the `linear-gradient` function actually creates an `image` element, and is usually paired with the `background` property which can accept an image as a value.

The `linear-gradient` function is very flexible -- here is the basic syntax you'll use in this tutorial:

Example Code

```css
linear-gradient(gradientDirection, color1, color2, ...);
```

`gradientDirection` is the direction of the line used for the transition. `color1` and `color2` are color arguments, which are the colors that will be used in the transition itself. These can be any type of color, including color keywords, hex, `rgb`, or `hsl`.

```css
background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0));
```
As you can see, the `linear-gradient` function produced a smooth red-green gradient. While the `linear-gradient` function needs a minimum of two color arguments to work, it can accept many color arguments.

```css
background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0), rgb(0, 0, 255));
```
Color-stops allow you to fine-tune where colors are placed along the gradient line. They are a length unit like `px` or percentages that follow a color in the `linear-gradient` function.

For example, in this red-black gradient, the transition from red to black takes place at the 90% point along the gradient line, so red takes up most of the available space:

```css
linear-gradient(90deg, red 90%, black);
```

Even without the color-stops, you might have noticed that the colors for the green marker transition at the same points as the red marker. The first color is at the start (0%), the second is in the middle (50%), and the last is at the end (100%) of the gradient line.

The `linear-gradient` function automatically calculates these values for you, and places colors evenly along the gradient line by default.
```css
background: linear-gradient(180deg, rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
```

Using hsl
```css
background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
```

##### Opacity
Opacity describes how opaque, or non-transparent, something is. For example, a solid wall is opaque, and no light can pass through. But a drinking glass is much more transparent, and you can see through the glass to the other side.

With the CSS `opacity` property, you can control how opaque or transparent an element is. With the value `0`, or 0%, the element will be completely transparent, and at `1.0`, or 100%, the element will be completely opaque like it is by default.
```css
opacity: 0.5;
```

Another way to set the opacity for an element is with the alpha channel. Similar to the `opacity` property, the alpha channel controls how transparent or opaque a color is.

You're already familiar with using the `rgb` function to set colors. To add an alpha channel to an `rgb` color, use the `rgba` function instead.

The `rgba` function works just like the `rgb` function, but takes one more number from `0` to `1.0` for the alpha channel:

Example Code

```css
rgba(redValue, greenValue, blueValue, alphaValue);
```

You can also use an alpha channel with `hsl` and `hex` colors. 
```css
background-color: rgba(255,255,255,50%);
```

##### Styling Borders
All HTML elements have borders, though they're usually set to `none` by default. With CSS, you can control all aspects of an element's border, and set the border on all sides, or just one side at a time. For a border to be visible, you need to set its width and style.
```css
border-left-width: 10px;
border-left-style: solid; //or double
border-left-color: black;
```

The `border-left` shorthand property lets you to set the left border's width, style, and color at the same time.

Here is the syntax:

```css
border-left: width style color;
```

```css
border-left : 10px solid black;
```

##### Shadow
The `box-shadow` property lets you apply one or more shadows around an element. Here is basic syntax:

Example Code

```css
box-shadow: offsetX offsetY color;
```

Here's how the `offsetX` and `offsetY` values work:

- both `offsetX` and `offsetY` accept number values in `px` and other CSS units
- a positive `offsetX` value moves the shadow right and a negative value moves it left
- a positive `offsetY` value moves the shadow down and a negative value moves it up
- if you want a value of zero (`0`) for any or both `offsetX` and `offsetY`, you don't need to add a unit. Every browser understands that zero means no change.

The height and width of the shadow is determined by the height and width of the element it's applied to. You can also use an optional `spreadRadius` value to spread out the reach of the shadow. More on that later.
```css
box-shadow: 5px 5px red;
```

Notice that the edges of the shadow are sharp. This is because there is an optional `blurRadius` value for the `box-shadow` property:

Example Code

```css
box-shadow: offsetX offsetY blurRadius color;
```

If a `blurRadius` value isn't included, it defaults to `0` and produces sharp edges. The higher the value of `blurRadius`, the greater the blurring effect is.
```css
box-shadow: 5px 5px 5px green;
```

You can do that with the optional `spreadRadius` value:

Example Code

```css
box-shadow: offsetX offsetY blurRadius spreadRadius color;
```

Like `blurRadius`, `spreadRadius` defaults to `0` if it isn't included.

```css
box-shadow: 0 0 0 5px blue;
```

```css
box-shadow: 0 0 20px 0 #3B7E20CC; //CC is the alpha
box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8); //0.8 is the alpha
```

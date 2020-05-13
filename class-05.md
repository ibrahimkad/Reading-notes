# HTML Images; CSS Color & Text

## Images

**How to add image to the website**
"_To add an image into the page you need to use an <img> element. This is an empty element (which means there is no closing tag)._"


**Example**
"<img src="images/quokka.jpg" alt="A family of quokka" title="The quokka is an Australian marsupial that is similar in size to the domestic cat." />"

**Where to Place Images in Your Code**

1. before a paragraph The paragraph starts on a new line after the image.
2. inside the start of a paragraph The first row of text aligns with  the bottom of the image.
3. in the middle of a paragraph The image is placed between the words of the paragraph that it appears in.

**Summarizes**
_You must always specify a src attribute to indicate the source of an image_
_You should save images at the size you will be using them on the web page and in the appropriate format._


## Color

**Why color?**
_Color can really bring your pages to life_

**You can specify any color in CSS in one of three ways:**
1. rgb values
 These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90)
2. hex codes
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80
3. color names There are 147 predefined color names that are recognized by browsers. For example: DarkCyan


**Every color on a computer screen is created by mixing amounts of red,green, and blue. To find the color you want, you can use a color picker.**


_It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content)._
_CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA._
_CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA._


## Text

_There are properties to control t XX he choice of font, size, weight, style, and spacing._
_You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented._
_You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or when they have visited a link._
"body {
padding: 20px;}
h1, h2, h3, a {
font-weight: normal;
color: #0088dd;
margin: 0px;}
h1 {
font-family: Georgia, Times, serif;
font-size: 250%;
text-shadow: 2px 2px 3px #666666;
padding-bottom: 10px;}
h2 {
font-family: "Gill Sans", Arial, sans-serif;
font-size: 90%;
text-transform: uppercase;
letter-spacing: 0.2em;}
h3 {
font-size: 150%;}
p {
font-family: Arial, Verdana, sans-serif;
line-height: 1.4em;
color: #665544;}
p.intro:first-line {
font-weight: bold;}
.credits {
font-style: italic;
text-align: right;}
a {
text-decoration: none;}
a:hover {
text-decoration: underline;}"
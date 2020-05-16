# JS Object Literals; The DOM


**WHAT IS AN OBJECT?**

_Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names._

**CREATING· OBJECTS USING LITERAL NOTATION**

"var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var elName = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms .textContent = hotel .checkAvailability();"



**Document Object Model (DOM)**

_The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window._

_The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas:_
1. MAKING A MODEL OF THE HTML PAGE
2. ACCESSING AND CHANGING THE HTML PAGE



**SELECT AN INDIVIDUAL ELEMENT NODE**
_get El ement Byld ()_
_Uses the value of an element's id attribute_


**SELECT MULTIPLEELEMENTS (NODELISTS)**
_getElementsByClassName()_
_Selects all elements that have a specific value for their class attribute._


**TRAVERSING BETWEEN ELEMENT NODES**
_parentNode_
_Selects the parent of the current element node_



**SELECTING ELEMENTS USING CLASS ATTRIBUTES**
_The getElementsByClassName()_
_method allows you to select elements whose class attribute contains a specific value._


**SELECTING ELEMENTS BY TAG NAME**
_The get El ementsByTagName ()_
_method allows you to select elements using their tag name._


**SELECTING ELEMENTS USING CSS SELECTORS**
_querySe 1 ector() returns_
_the first element node that matches the CSS-style selector. querySe 1ectorA11 () returns a Nodelist of all of the matches._


**ACCESS & UPDATE A TEXT NODE WITH NODEVALUE**
"document.getElementByid( 1 one 1 ).firstChild.nextSibling. nodeValue;"
_textContent_
"To collect the text from the <l i> elements (and ignore any markup inside the element) you can use the textContent property on the containing <l i > element."
"document .getElementByid('one') .textContent;"



**ACCESS & UPDATE TEXT & MARKUP WITH INNERHTML**
_When getting HTML from an element, the i nnerHTML property will get the content of an element and return it as one long string including any markup that the element contains._

"var elContent = document.getElementByld('one').innerHTML;"//_collects the content of the list item and adds it to a variable called e 1 Content_




_adds the content of the e 1 Content variable (including any markup) to the f irst list item:_
"document .getElementByld('one').innerHTML = elContent;"


**CROSS-SITE SCRIPTING (XSS) ATTACKS**

_XSS involves an attacker placing malicious code into a site. Websites often feature content created by many different people._

_WHAT CAN THESE ATTACKS DO?_
1. The DOM (including form data) That website's cookies
2. Session tokens: information that identifies you from other users when you log into a site



**DEFENDING AGAINST CROSS-SITE SCRIPTING**

1. Only let visitors input the kind of characters they need to when supplying information. This is known as validation. Do not allow untrusted users to submit HTML markup or JavaScript.
2. Double-check validation on the server before displaying user content/storing it in a database. This is important because users could bypass validation in the browser by turning JavaScript off.
3. The database may safely contain markup and script from trusted sources (e.g., your content management system). This is because it does not try to process the code; it just stores it.



**Never place any user's content in the following places without detailed experience of the issues involved**

Script tags:"<scr ipt>not here</script>"
HTML comments:"<!-- not here -->"
Tag names:"<notHere href=" / test" / >"
Attributes:"<div notHere="norHere" / >"
CSSvalues:"{color: not here}"




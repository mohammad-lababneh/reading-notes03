<!-- Reading
From the Duckett HTML book:

Chapter 4: Ch.4 “Links” (pp.74-93)
Chapter 15: “Layout” (pp.358-404)
Note: This layout chapter is BIG. Focus your attention on understanding the core concepts presented on pp.358-364, and look at the code samples on the website that accompanies the textbook. You will have another reading assignment on this chapter, so do not try to digest it all now.

From the Duckett JS book:

Chapter 3 (first part): “Functions, Methods, and Objects” (pp.86-99 ONLY)
Article: “6 Reasons for Pair Programming” -->
# HTML
## chapter 4 links 

 ##### creating inks between pages
 ##### Linking to other sites 
 ##### Email links 
 
 ### Writing Links
 Links are created using the` <a>` element. Users can click on anything between the opening `<a> `tag and the closing
 ` </a>` tag. You specify which page you want to link to using the href attribute.

  example ` <a href="http://www.imdb.com">IMDB</a>`


### Linking to Other Sites
Links are created using the ` <a> ` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.


### Linking to Other Pages on the Sa me Site
When you are linking to other
pages within the same site,
you do not need to specify the
domain name in the URL. You
can use a shorthand known as a
relative URL.
If all the pages of the site are in
the same folder, then the value
of the href attribute is just the
name of the file.
If you have different pages of a
site in different folders, then you
can use a slightly more complex
syntax to indicate where the
page is in relation to the current
page. You will learn more about
these.


### Email Links
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the ` <a> `
element. However, this time the
value of the href attribute starts
with ` mailto: ` and is followed by
the email address you want the
email to be sent to.

### Opening Links in a New Window  `target`
target
If you want a link to open in a
new window, you can use the
target attribute on the opening
`<a> `tag. The value of this
attribute should be _blank.
One of the most common
reasons a web page author
might want a link to be opened
in a new window is if it points to
another website. In such cases,
they hope the user will return
to the window containing their
site after finishing looking at the
other one.

ex : ` <a href="http://www.imdb.com" target="_blank"> `
` Internet Movie Database</a> (opens in new window) `





### Linking to a Sp ecific


Before you can link to a specific
part of a page, you need to
identify the points in the page
that the link will go to. You do
this using the id attribute (which
can be used on every HTML
element). 
The value of the id attribute
should start with a letter or an
underscore (not a number or
any other character) and, on a
single page, no two id attributes
should have the same value.
To link to an element that uses
an id attribute you use the` <a>`
element again, but the value of
the href attribute starts with
the ` # ` symbol, followed by the
value of the id attribute of the
element you want to link to. In
this example,`  <a href="#top"> `.  



### Linking to a Sp ecific Part of Another Page

If you want to link to a specific
part of a different page (whether
on your own site or a different
website) you can use a similar
technique.
As long as the page you are
linking to has id attributes that
identify specific parts of the
page, you can simply add the
same syntax to the end of the
link for that page.
Therefore, the href attribute
will contain the address for the
page (either an absolute URL or
a relative URL), followed by the
` symbol,` followed by the value
of the id attribute that is used on
the element you are linking to.
For example, to link to the
bottom of the homepage of the
website that accompanies this
book, you would write:
`<a href="http:/www. htmlandcssbookcom/ #bottom">`




## chapter 15 LAYOUT 

#### Controlling the position of elements
#### Creating site layouts
#### Designing for different sized screens

### Key Concepts in Positioning Elements

CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text. You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use
borders, margins, padding, and background colors.

`Block-level elements nstart on a new line`
`Examples include: <h1> <p> <ul> <li>`


`Inline elements flow in between surrounding text`
`Examples include: <img> <b> <i>`



###### Containing Elements
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.


#### Controll ing the Position of El ements

##### Normal flow
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

##### Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

##### Ab solute positioning
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.


##### Fixed Positioning
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
Elements with fixed positioning
do not affect the position of
surrounding elements and they
do not move when the user
scrolls up or down the page.

##### Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box. The floated
element becomes a block-level
element around which other
content can flow.
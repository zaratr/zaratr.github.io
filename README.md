# **Code 201 Reading Notes**
## ~~Reading assignment 1~~
-css styles the html
-html focus on content (markup)
-DNS servers

### Structure
- html structure uses tags to describe bodies of markup
- padding and margin
- closng tags are useful to finish statement
- basic information to get you html or webpage to get started. you can use the html for basic styling if any.

### extra markup
- <!-- --> comments
- attributes: classes, id, etc
- <li> is a list element
  </li>
  - iframe is somewhat useful
  - this goes more in depth on attributes that may help creating some html syntax. Iframe, for example, can be used to show a location in webpage. adding a class allows you to use an attribute
  
### extra html5
- html5 has useful markup
- aside, section, nav, become useful in replacement of div

- this chapter explains what is useful in the new version of html tha twasn't available before. it is more useful now to use these tags and can beautify markup

- javascript portion of the reading describes the usage of object and primitive types. to declare, instanteate , and use keywords to build a stonger code. for example, arrays can be dynamically added onto unless described by coder or client to have alloted memory.

## ***Reading assignment 02***
## HTML Book
### Chapter Two: Text
- Two types of text rules:  Structure Markup (change the whole thing where it looks different) and Semantic Markup (change the words to bold, etc.)
- h1 -> h6 are usable headings. p is a paragraph, br is breaking to new line, hr is breaks the markup and creates horizontal line
- <blockquote> <q> <cite> all have to do with work citation or giving author credit.
- <abbr> helps to have the definition of a abbreviated word.
  - ins, del modify a line under the word or through it. 
### Chapter10:  Intro to css
  - changes appeareance of html.
  - rule book to appearence for markup
  - padding and margin are implicit
  - declaration{property: value;}
  - link href="location/css/file" type=text/css" rel='stylesheet' ----> rel : relationship between html and file , type => type of document always css href => location of file
  - css selectors *, {} => targets all; h1,..,h6 targets specifed chain of elements; #IDselector; parentOf>ThisChild targets everything in parent of that has thisChild selectors
 ### Chapter 2 JavaScrpt
  - conditionals such as if, else if, else ; comments using // and /**/ variables: const, let, var(it is global even when local DONT USE DUMB!)
  -Data Types: Literals(all numbers and concates to preceding. for exp double/floats concat with integers to double/floats operation dependant), strings,  Boolean, array
  -arithmetic operators, string operators, all use same methods in other languages. pay attention to rvalue and lvalues
### Chapter 4 JS
  - using variables and expressions to create statements and sentences. basically combining keywords can initialize a algorithm based on what outcome is wanted. exp 2 + 2 = 4 or obj2 = obj1 (does not deep copy). emphasized points are operators such as logical operators conditionals, switch, loop stopping/starting. while, dowhile, for loops. do not touch on for of or for in.
  
  
  
## Reading assignment 3
  ## HTML /css
  ###Chapter 3
   - <li> list item, <ol> ordered list, <ul> unordered list , <dl> dictionary list, <dt> definition term, <dd> definition(has inline definition)
   - you can chain the li to be a tree with multiple levels of list item by creating ul first within a ul
  
  ### Chapter 13
  - boxes are the surrounding area of element. the margin and padding live here
  - percentages goes by the size of the window
  - em goes by size of the text. so if the text is too large it would measure the window weirdly.
  - the preffered method is using px (pixels)
  - using min-height and max-height avoids clashes in case element contents are too large for the window when shrinking the window
  - overflow usage helps with content being too large
  - hidden hides the content and is useful when the content is too large
  - scroll helps by giving the user the ability to scroll the content f the content is too large.
  - border, margin and padding are all implicit content. padding refers to the property  of how much space should apear between the content of an element and its border. margine is the gap between boxes.
  - you can set their sizes to whatever size.\
  - to modify the style for borders , use border-width: (a Value), border-style:(a Value)
  - text-align: value helps alignment of each box.
  - border-radius: value helps design a circle by narrowing the image edges.
  
  
  ## Java
  ### chapter 2
  - arrays can be declared like : let arr = {x, ..., y} ; let arr[2] ; let el.textcontent = anotherarr[2];
  - arrays are all dynamic
  - expressions can be done onto variables. 
  ### chapter 4
  - switch statements are similar to conditionals as far as flow goes. 
  - truthy and falsy values are useful when being lazy about using boolean. 0 is false but most everthing else evaluates to true.
  - loops can be controlled using parameters and a variable to increment. objects can be incremented by objects and there is a certain method to do so.
  - do while loops just increments first then checks for true or false (false triggers the loop to end).
  
## Reading assignment 4
  - <a> attribute to use for links. href is placed as the attribute link so that html finds the file
  - syntax for entering grandchild or any set of parent folder, we use ..; similar to linux terminal command ..
  - to refer to somewhere in the same page use href to aim where to go to and use html element(tags) attribute id="type here" to show where
### Chapter 15
  - By default the box normal flow is set to static ''' position: static '''. however, it is implicit
  - ''' position: relative; ''' changes the value relative to static position (I think we just use relative to modify the box rather that using static).
### Chapter 3
  - Functions are objects in javascript that carry specialized tasks and rules that the client maneuvers uses. the coder is responsible for making those rules.
  - Declare an array using keyword function followed by variable name and paranthesis for arguments/parameters.
  - calling a function is using the name and parenthesis 
  - you may choose to set a return something and multiple return is possible.
  - functions in js remind me of labda operation which also ties in with functional programming but not quite sure yet (Review later to see if the concepts are the same).
  - avoid using var!!!
### 6 reasons for pair programming
  - I like the idea that we are effiecient but that also ties in with all six reasons (in my opinion)
  - more engagement is possible when working together.
  - students can also have more knowledge of code that I don't
  - becoming more vocal helps me better ask a question and builds skills that will be needed to grab attention or make things more interesting
  - working with other people helps me become more ready for an interview using practice with a teammate.
  - companies already use pair programming and is useful in the field.
## Reading assignment 5
  ### Chapert 5
  - Four steps into adding image: Include image in scope; pic a format; show image with correct size; optimize image for faster render.
  - Important to keep images organized. 
  - they are important to set tone of webpage. 
  -to seetin an image use the tag <img> and to set the style for the image use height and width. these style commands change how big image expands.
  - align:"value here"; command sets the way the things around the image should flow.
  - alight: top; sets the surrounding texts to alight to top right of image. midd sets the surrounding text to start at middle of image. vice-versa for bottom command.
  - Vector images can be really handy! Images lose some of their resolution. some minipulation may be required.
  - animated gifs can add extra characteristics to a webpage that a photo cannot. a video will motion better than image
  - figcaption tag allows for a text caption to follow an image. 
  - Transperency is useful when filtering is needed.                                                                                                                            
                                                                                                                               
  ### Chapter 11
  - colors can be modified either by text or background.
  - css3 unlocks saturation and contrast. opacity is also a good commandin css. hue seems to follow rgb less than cmyk.
  ### Chapter 12
  - serif: strokes to the letters. san-serif: straight ends to letters. monospace: fixed width. weight: refers to boldness. style: italiqu or oblique. Stretch: refers to the text being long for each letter or skinny.
  - respoinding to user with pseudo classes/elements h1:visited is useful for changing the color change if user clicked on it.a:hover is also useful for responding to the mouse.
  - pg 292 has really useful attribute selectors for classes. p[class:"value"] selects class that have a class attribue that is called "value"
  ### JPEG VS PNG VS GIV
  - lossy losses resolution permenantly and irreversible. and lossless is a compression and reconstructable.
  - jpeg will be that can be compressed at a ratio 1:10 without losing its quality.
  - png is lossless in that no data is lost when compressed. looks sharper and ideal for text styling on webpage.
  - gif is lossless image format that uses a LZW compression algorithm. it was used for images but png is superior. now, gif are used for videos.
  - jpeg is does not support transperency but pnng and gif do. png8 can support index transperency wheras png24 can support alpha channel transperency.
  - gif is index transparency supportecd.
## Reading assignment 5
  - it's important to break downt he problem into small solvable steps. also make sure you carefully understand the issue before breaking down for solving.
  - objects have a special place in javascript. the object is treated as a "complex" type. instantiating arrays, functions, classes, or anything with dynamic size or usage of large memory is basically an object. for example, "strings" are objects and a way to check is to use a method. methods are usually tied to collections and all collections(if i'm not mistaken) are objects.
  - objects literals have key and value where : is the assignment operator.
  - object literals have method and properties. field types are properties and the method is still field method.
  - all object properties and methods are dynamic and accessible by client.
  - Pg 189 has really useful cmmands to access elements.
  - first and last child are useful when goin g to grab the last element. you may replace them using getElementsByTagName, then setAttribute('class', 'name'). this can be a bit trick but straight forward. look at pg 211
  - adding to the dom or webbrowser running html/script is possible. usefule commands are document.create Elemtnt() and document.createTextNode()
  - avoid malicious attackers such as xss (cross-site scripting). they can access all information on site.always scrape trusted sources or not at all.
## Reading assignment 6
  - domain modeling reminds me of OOP in that you specify tasks (functions/objects) to carry on tasks. constructors are very useful as they will initialize many objects with same parameters. by using a constructor we also avoid erros.
  - thead, tbody, tfoot, td, tr, are all useful css table creation. 
  - data structure: arrays in objects. it can be extremely useful and better for memory and time complexity compared to object in objects (assuming its the same as java).
  - some global objects are String, Number, Boolean, Date, Math, Regex.
## Reading assignment 8
  - flexbox layout for one dimensional layouts. layout across a single axis, either horizontally or vertically.. it will also align to elements in children. in the inline direction
  - grid multi axis grid. basically it wil make multiple items in a grid and you can manipulated it with grid-row, and grid-column.
  - inlive block flows inline with characteristics of block level element.
   - By default the box normal flow is set to static ''' position: static '''. however, it is implicit
  - ''' position: relative; ''' changes the value relative to static position (I think we just use relative to modify the box rather that using static).
## Reading assignment 9
  ### Chapter 7 "forms"
  - forms can be really useful when used. they addsome functionality and interactions to the client.
  - what makes them useful are adding text into a single line text input. clients can insert their emails or provide some feedback on webpage without leaving the website.
  - A second useful for are radio buttons/ check boxes/ drop down boxes. these are options that someone can have a simple options.
  - the process startes by the client typing in their response - next the client input will then be used by a scripting language passed in (usually servers handle this data and sent to the programmer when needed). then their is a response to the client for typing in the information.
  - inside the scripting language the data is saved into variable passed in.
  - tag name <form action="where from" method="get"> always have -action- within the tag as an attribute.
  - method is used to get values from a server just for data collecting. short forms such as boxes.
  - tag name <input type="text" name="value inserted" size"integer" maxlength="integer that limits client input" receives something from client and gives returns some value somewhere within form to be used later.
  - if we change input type="password" then the attribute in the element will change the text they write to non seeable input.
  - radio buttons have <input type="radio" name="grouping" value="text of radio option" checked="checked">
  - name describes the content grouping and should be in the same group that all radio button options are on.
  - value describes what should be returned from client.
  - checked refers to what should be checked when webpage loads.

  - selected attribute indicates what was selected before.
  - form validation is usefel to user when a password wasnt typed in the form.
  - to do this, create an attribute required="required"
  - for dates use attribute type="date"
  - for search feature on webpage, use attribute type="search" like this <form action="place webpage"><input="search" name="search" placeholder="touser in form"></input></form>
  ### chapter 14
  - controlling appearence on lists, tables and forms provide awesome characteristics.
  - bullet points can be changed to look a bit different using css property list-style-type. we can set this to decimal, decimal-leading-zero, lower-alpha, uppper-alpha, lower-roman, upper-roman.
  - list-style-image property can be used when you have what you want to be the bullet point instead of whats given (insert image).
  - list-style-position property indicaatees marker should appear on the inside or outside of the box containing the points.
  ### chapter 6 java
  - the power of java when client wants to browse is that there are som many possible keywords to use to provide a interactive web page.
  - event trigger has three steps for the client to use. in triggering event handling is used. the three steps are select element, specify event, call code.
  - element node needs to respond. using dom query.
  - next indicate event response aka "binding" to the dom node.
  - finally result from clicking the event.
  
  - programmers can bind three different ways html event, dom event, level 2 event listener (best way to avoid errors).
  - we should stay away from html event handlers and use dom level 2 event listener.
  
  - using event handlers in javascript is like the way we have been doing when writing content onto the dom.
  - element.event = functionName
  - same goes for eventlistener. this is useful when you want interaction with button for example on html
  - element.addeventlistener('enent', functionname, boolean)
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment

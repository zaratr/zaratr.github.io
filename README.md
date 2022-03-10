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
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment
## Reading assignment

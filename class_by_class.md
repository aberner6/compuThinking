# Intro to Programming (p5)

## p5.js

## Structure

### 1 -- Introduction +
- Intro to each other
- Why program?
  - What program?
    - p5 is built from Processing, which began in 2001
    - Casey Reas and Ben Fry: the history of platforms to make programming interactive graphics easier and faster to program rather than heavy lifting to build them in C++ and Java
      - And make programming more accessible for design and art students
      - Inspired by Logo and BASIC and Design By Numbers
    - Evolution to p5 means that Processing is now even more open and accessible - as it is online
      - Still using syntax and conventions of Processing as much as possible
      - But now built with Javascript (and HTML / CSS)
  - Why me?
    - Make a game, animation, interactive interface
    - Visualize data abstractly
    - Sketching with code
      - Write a line, test it out ("press play")
      - What if...
        - A circle disappeared every time I clicked on it
        - A series of bubbles follow my face when I smile
        - Depending on the amount of noise in the room the graphics are bright and busy or dark and calm
  - Me and who else?
    - p5 and Processing are accessible and practical for a wide range of uses and "users"
  - **Diagram:** landscape of languages: which languages and for what?
    - p5 is built in a language called Javascript but has some custom features for interaction and graphics that make it faster and easier to sketch with code
    - Families:
      - Processing, p5, Arduino - sketching with code - artists, interaction designers, scientists! Researchers!
      - C - Processing
      - Java - Processing
      - HTML / CSS - front-end of websites (what you see)
      - JavaScript - front-end action, analysis and tons of amazing libraries
      - Python
      - Ruby
    - Open frameworks - fast processing for interactive installations that take a lot of data in
    - MAX MSP data-flow
    - Grasshopper - architecture + computation
- Fear in a Box
  - Put one in, take one out
- p5 Introduction
  - Darling Dan Shiffman
  - What is it?
  - Who's making it?
    - [p5.js working group mailing list](http://groups.google.com/forum/#!forum/p5xjs-working-group)
  - Getting set up + the editor "environment"
    - A code editor is like a text editor but special for writing code
    - We will use the official p5.js editor
  - p5 and the browser
    - **Diagram:** landscape of the web: how do we see things online?
    - HTML is our backbone, Javascript (and p5.js library) make things interactive, CSS would help us style that page but we won't deal with it this week
    - Let's look at the index.html file - just so you know, it links to our sketch.js file - but we leave that for now
    - We will work in sketch.js
  - p5 - a library - what is a library?
    - 1 word that defines a series of actions / associations (like a dictionary)
    - **Diagram:** how do HTML / CSS / Javascript and its libraries go together?
    - Looking underneath the "hood" - what is a line and how is it defined in the p5 library?
- Computational thinking
  - How do we communicate?
    - Formulate & Represent
    - Speech, Drawing, Writing, Etc.
      - Write left to right and put a space between each word
      - Capitalize names of people and places
      - Use punctuation!
      - ALL CAPS MEANS SOMETHING
    - Communication to another:
      - Speech to Understanding (listening to understand)
      - When have you miscommunicated?
      - How did you clear it up?
    - Definitions:
      - **Exercise:** let's play telephone - draw / write / draw / write
- Code - computational writing
  - Speaking computer: pseudo-code
  - **Exercise:** Write how to make a peanut butter and jelly sandwich?
  - **Exercise:** How to draw a circle
    - Tell it to me
    - Tell it to me as if I am a computer
      - No shortcuts - computers don't understand "how r u"
      - Graph paper / geometry / starting from top left edge (0,0)
      - Setup?
      - Canvas?
      - Draw?
    - Now let's write it in the sketch window in p5
      - A few notes:
        - It's called an ellipse
          - p5 includes a few function to draw basic shapes - thus we have ellipse() - it is a "function" with "parameters"
          - This is also a function: "createCanvas()"
          - And these are parameters (800, 600);
          - They go inside the function - these are the details of your description
        - Some things are turning pink - what do you think that means?
          - Functions / built-in
        - The role of comments - these guys // and these guys /* several lines*/
        - Directions of x, y, radius, radius are inside of parenthesis - parameters
        - Uppercase and lowercase mean different things to the computer
        - Semi colon - means "I'm done here!"
      - Before we press play, close eyes and imagine what we will see
  - Setup and draw:
    - Setup: canvas size, color mode, background - happens ONCE
    - Draw: animation, change over time - ALWAYS RUNNING
  - **Exercise:** Draw a circle _in the center of the canvas_
    - (There is an easier way)
    - Width, height, shapes, color modes, and more - are defined in the library - so they will turn pink - and this means we can reference them directly!
      - A few notes:
        - Watch your Ps, Qs, and...
        - Grammar and programming
          - "Syntax" to watch out for: parenthesis, commas, semi-colons
            - Parameters
            - Functions
            - background (0, 0, 0);
        - Style / formatting: use the conventions. Command t to clean it up
        - Read your debugging console (gear icon top right of sketch - or View -> Developer -> Javascript Console if in Chrome)
          - It's trying to help you!
  - Run / alter / break / enhance / reshape - try tons of Examples!
    - One step at a time - things will be less tangled and you will be able to find the errors more quickly. Write a bit, test, write a bit, test
    - Small successes :)
  - **Exercise:** Draw a circle if your mouse is pressed
    - How do I know about mousePressed? Check the online reference
  - **Exercise:** Draw a rectangle
    - How do I say rectangle to computer? Check the online reference
  - **Exercise:** Draw an arc
    - How do I say degrees / radians and start and stop? Check online reference
  - Variable scope: variable created inside curly braces { } only exists in there. Global variables are above setup. Local variables are inside curlies.
- Programming life:
  - **Diagram:** Think of how you got to school today. Try to note how many times you could have expressed AND/OR experienced computation
    - Order of operations: like reading a novel - this, then that, then that etc.
    - Drawing order: like layers in Illustrator or when you paint a canvas - again - this, then that, then that
- Favorite errors?
  - Mysteries or puzzles
- Wrap up: what did we do today?
  - **Diagram:** what's p5 and how do we work with it? What does computational thinking mean to you?
  - Bowl of concepts (operations, variables, etc.)



### 2 - Debugging, Events (mouse, keys), Shapes (contours, vertices, curves), Text (fonts), Color (RGB, HSB), Blends
- Assignment from yesterday: bowl of concepts
- Debugging: ah, the mysteries :)
  - Order of operations: like reading a novel - this, then that, then that etc.
  - Drawing order: like layers in Illustrator or when you paint a canvas - again - this, then that, then that
  - Variable scope: variable created inside curly braces { } only exists in there. Global variables are above setup. Local variables are inside curlies.
  - One step at a time - things will be less tangled and you will be able to find the errors more quickly. Write a bit, test, write a bit, test
  - Small successes :)
  - "Syntax" to watch out for: parenthesis, commas, semi-colons, capitalization, spacing
  - Did the console help you?
  - Parameters - inside parenthesis
  - Functions - ()
  - Graph paper / geometry / starting from top left edge (0,0)
  - Reading the reference
- Variables
  - Store a value so it can be used later - many times - without you having to state it again
  - If you're typing a number in a lot of times / places, make it a variable
    - Reuse same values
    - Change it locally
    - Name it: var x; //this means new variable
    - Give it a value: x = 12; //references the one above
    - Do it all in one go: var x = 12; //make a new variable and give it 12
      - Careful of the order and scope - who can see what?
    - Built in variables - the parameters from your canvas size - width and height
    - Repetition - for loops - concept for tonight and tomorrow
- Events
  - Continuous input - must run in draw() so we are always listening
  - frameCount
  - mouseX and mouseY
  - background - painting over each frame or not?
  - pmouseX and pmouseY: the most recent position
  - dist()
  - easing
  - mouseIsPressed()
  - if() and else () - conditions
  - Logic - < > <- && || true and false
  - keyIsPressed - this is momentary
    - key - this keeps its value
    - keyCode
  - touchIsDown
    - touchX and touchY
- map()
  - My favorite function :)
  - Values are between 0 and width of screen (mouseX, for example)
  - We "map" them to 0 to 5
- Shapes
  - Vertex... beginShape(); then vertex(); then endShape();
    - endShape(CLOSE);
- Text
- Color
  - Order of operations
  - noFill()
  - noStroke()
  - RGB
  - RGBA (transparency - alpha channel)
- Blends
- Translate / rotate / scale
  - Push / pop



### 3 -- Repetition (Loops, Functions and Helpers), Organizing (Arrays, Objects and OOP), Data +, Structuring (Ideas), Sending (Data)
- Assignment from yesterday: bowl of concepts
- Lovely Loops
  - I'm repeating myself over and over again
  - I want to make this evenly spaced and my fingers and brain are getting tired of writing ellipses forever
    - [Loops to the rescue!](https://www.youtube.com/watch?v=cnRD9o6odjk&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=15)
      - While to your rescue
      - For to your (real) rescue!
        - x = x+50
        - x+=50
        - x++
  - **Exercise:** try making a pattern of repeated shapes. Can you play with the y axis? Color? Shape changing?
- Functions
  - and passing information in different parts of your program
- **Exercise:** make a "you" creature
  - Make an interactive "you"
- Storing data:
  - Arrays
    - Can contain anything! As long as it's organized a bit
    - Brackets mean "at"
    - indexOf('thing') - will tell you where 'thing' is located in the array
    - You can put numbers and letters and strings all in the same array - though it may make your life harder
    - Helper functions - returning the stuff we're looking for!
    - Split 'em up and stitch 'em back together again (array1.slice(1, array1.length-1)), array1.concat(array2))
      - var array2 = array1.slice(1, array1.length-1)
        - Translation: take a slice of array 1 from after the first item until the one before last
      - array2 = array1.concat(array2)
        - Translation: stitch array 2 to array 1 (please)
    - Functions and arrays -
      - Returning the things we are looking for - built in to p5
      - Let's say we only want numbers divisible by 2. How do we write that?
      - We enclose this "functionality" in a function, called "filterFunc"
      - If we run the filterFunc on our array, we will get back only the numbers that fit the special functionality that filterFunc will return to us
        - Translation: When you're scrolling through your Instagram feed and you notice a nice photo. It's tagged with a location. If you tap on that location, you'll see only the photos that were taken and geo-tagged with that same place.
        - Instagram has a functionality that is encapsulated in some locationFunction() that will return just the images you need
      - Arrays and for loops: https://www.youtube.com/watch?v=RXWO3mFuW-I&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=21
    - **Diagram:** what's an array?
  - Things with properties - literal objects
    - I'm a human, defined as a female, brown hair, height, able to walk and talk
    - 2 different ways to define and express the properties of an object.
      - On the fly
      - JSON
        - Especially used in data sets, great to organize, recommend formatting information this way
        - var json = {
          starts: "with curly brackets",
          ends: "with curly brackets",
          inside: "items with colon, then either numbers or letters or words",
          andThen: "a comma after each one"
          whatAboutTheVeryVeryEnd: "put a semi-colon of course!"
        };
        - What's up with this whole low caps high caps thing?
          - Try having spaces instead and you'll see
      - **Diagram:** How would you describe your favorite animal (or if you hate animals, then your favorite food or drink) as a thing with properties?
- Organizing programs:
  - Writing constructor functions...
    - We know how to write the literal object - the collection of "name-value" pairs - the curly brackets, etc.
    - var thisSpecialThing = {
        x:100,
        y:50
      }
      - thisSpecialThing.x = 50
      - Functions in javascript: function blah(){ }
      - function Bubble (capital letter is CONVENTION)
        - bubble = **new** Bubble() <- we see those parenthesis and know it is a function
        - javascript looks for function called Bubble()
      - function Bubble(){ //a template!
          this.x = 100; //attaching x to the object
          this.display() = function(){

          }; //what happens there?
        }
        - IF you made a new object called Bubble, we would give it these special attributes!
    - Creature:
      - Looks like: I'm going to write a function somewhere else that describe what it looks
      - Moves like: Check in the move area!
    - "Playing god":
      - Many many creatures, all the same
      - How would we do this?
  - **Diagram:** A creature and its abilities - based on your favorite animal - but described for the computer to understand
- Figure it out:
  - Google, forums, references, errors
  - **Exercise** recap favorite errors from today?
- Data +
  - Data's everything and eveywhere
  - What is something you are touching that could be described as "data"?
  - Pixels are data
  - Images are composed of Pixels
    - We can access every pixel in an image
    - Let's load one up (we have to tell the computer WHERE to find it - paths in our computers)
    - One tiny square has many many pixels
    - Each pixel is a combination of colors
    - We can get the pixels at any spot in the image
      - And use that color to color in a rectangle
      - Remember to update pixels
  - **Exercise:** Load a picture, loop through the pixels, do something with each color
    - Note:
      - Interaction - in setup vs. in draw loop?
- Structuring ideas
  - Pseudo-code
  - Diagrams
  - Outside help and collaboration
  - # o' times to try before asking for help
- Sending (Data)
  - Web sockets
    - Opening portals to other worlds
    - Connecting
    - Messaging
    - Responding
- **Exercise** recap favorite errors from today?
- Wrap up: what did we do today?
  - Why all the emphasis on organization?
  - **Diagram:** what's your house / apartment building look like and how do you think it was made?
  - **Exercise:** brainstorming controls / communication concept to bring to synths
    - What inputs can you detect?
    - Which ones would you like to play more with?
    - What might they control in terms of audio output?
    - How does "over space" (and time?) change the idea?





















<br>
<br>
<br>
<br>
<br>
_Relevant videos, readings, inspiration:_
### FOR NOW
###### DAY 1:
  * Deeper dive:
    * Drawing with numbers: [video tutorial](https://www.youtube.com/watch?v=D1ELEeIs0j8&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=2)
    * Shape and color functions: [video tutorial](https://www.youtube.com/watch?v=9mucjcrhFcM&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=3)
    * [p5.js reference](http://p5js.org/reference)
  * Readings:
    * [Pick an Eyeo Talk that looks interesting](https://vimeo.com/eyeofestival/)
    * [Introductory p5.js videos](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA)
    * [FORM+CODE: Introduction and What is Code?](http://formandcode.com)
    * [As We May Think](http://www.theatlantic.com/magazine/archive/1945/07/as-we-may-think/303881/), Vannevar Bush
    * [Long Live the Web](http://jblomo.github.io/webarch253/slides/Long_Live_the_Web.pdf), Tim Berners-Lee

###### DAY 3:
* Deeper dive:
  * If you are excited about organizing and controlling arrays, objects, structure of your programming...
    * [What's an array?](https://www.youtube.com/watch?v=VIQoUghHSxU&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=20)
    * [Organizing code a little better through Objects](https://www.youtube.com/watch?v=F3GeM_KrGjI&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=23)
    * An array of objects! [video tutorial 6.3](https://www.youtube.com/watch?v=pGkSHeEZLMU&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=22)
      * [Interactive Stripes](http://alpha.editor.p5js.org/projects/SJRI1mqC)
    * Adding and deleting from an array, `push()` and `splice()` [video tutorial. 6.5](https://www.youtube.com/watch?v=EyG_2AdHlzY&index=24&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA)
      * [MousePressed Adding New Gravity Ball Objects](http://alpha.editor.p5js.org/projects/SJysg7c0)
    * Checking objects intersecting with other objects [video tutorial 6.9](https://www.youtube.com/watch?v=uAfw-ko3kB8&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=28), [video tutorial 6.10](https://www.youtube.com/watch?v=GY-c2HO2liA&list=PLRqwX-V7Uu6Zy51Q-x9tMWIv9cueOFTFA&index=29)
       * [Checking Objects Intersection](http://alpha.editor.p5js.org/projects/BJEYSU90)
* Readings:
    - [Work of Art in the Age of Mechanical Reproduction](http://www.berk-edu.com/VisualStudies/readingList/06b_benjamin-work%20of%20art%20in%20the%20age%20of%20mechanical%20reproduction.pdf), Walter Benjamin




### FOR THE FUTURE:
(Mostly defined by Dan Shiffman and Lauren McCarthy)
##### Data
* [All video tutorials](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6a-SQiI4RtIwuOrLJGnel0r)
- [Tutorial: loading external data with p5.js](https://github.com/processing/p5.js/wiki/Loading-external-files:-AJAX,-XML,-JSON)
- [Tutorial: more about data and APIs](http://shiffman.net/a2z/data-apis/)
- JSON and APIs (and more on callbacks!)
- [Word Counting](http://shiffman.net/a2z/text-analysis/)
- Tabular data
- Additional Reading:
  - [Art and the API](http://blog.blprnt.com/blog/blprnt/art-and-the-api), Jer Thorp
  - [The Anxieties of Big Data](http://thenewinquiry.com/essays/the-anxieties-of-big-data/), Kate Crawford
  - [Sentencing Guideline From Surya](https://www.washingtonpost.com/news/monkey-cage/wp/2016/10/17/can-an-algorithm-be-racist-our-analysis-is-more-cautious-than-propublicas/)

##### Video and Sound
* [Video tutorials on video](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6aKKsDHZdDvN6oCJ2hRY_Ig)
* [Video tutorials on sound](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6aFcVjlDAkkGIixw70s7jpW)
- [p5.sound reference](http://p5js.org/reference/#/libraries/p5.sound)
- [Video/capture: p5.MediaElement reference](http://p5js.org/reference/#/p5.MediaElement)

##### Mobile
- Workflow and process, get a previous sketch running on a device
- Touch interaction
  - [Single Touch](http://alpha.editor.p5js.org/projects/H1a1YWOgl)
  - [Multi Touch](http://alpha.editor.p5js.org/projects/HkDY43yxl)
- Events
  - [Device Moved](http://alpha.editor.p5js.org/projects/BysXo-dgx)
  - [Device Turned](http://alpha.editor.p5js.org/projects/ryMwSnyxx)
  - [Device Shaken 1](http://alpha.editor.p5js.org/projects/rkmqU2Jee)
  - [Device Shaken 2](http://alpha.editor.p5js.org/projects/rJWwujwxg)
- Sensors
  - [Rotation (Gravity)](http://alpha.editor.p5js.org/projects/Hylv2b_xl)
  - [Acceleration (3D)](http://alpha.editor.p5js.org/projects/BJxoCbdxx)
  - [Geolocation 1: lookup lat lon](https://alpha.editor.p5js.org/projects/HkQ8kMdee)
  - [Geolocation 2: track lat lon](https://alpha.editor.p5js.org/projects/SyfolGuex)
- [Hammer.js](http://hammerjs.github.io/)
  - [Swipe events](http://alpha.editor.p5js.org/projects/HyEDRsPel)
  - [Swipe force](http://alpha.editor.p5js.org/projects/rkOj4bueg)
  - [Pinch and rotate](http://alpha.editor.p5js.org/projects/SJpBDW_gg)
- Remote debugging:
  - [Android remote debugging](https://developers.google.com/web/tools/chrome-devtools/remote-debugging/?hl=en)
  - [iOS remote debugging](https://developer.apple.com/library/content/documentation/AppleApplications/Conceptual/Safari_Developer_Guide/GettingStarted/GettingStarted.html)
  - [Generic remote debugging](https://jsconsole.com/)
- [Using the viewport meta tag to control layout on mobile browsers](https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag)

##### Life beyond p5.js
  - Other JS libraries?
    - d3.js
    - WebGL - [tutorial](https://github.com/processing/p5.js/wiki/Getting-started-with-WebGL-in-p5)
  - Wekinator + Arduino + Processing
  - Coding outside the p5 IDE? ([local server tutorial](https://github.com/processing/p5.js/wiki/Local-server)), [video tutorial](https://www.youtube.com/watch?v=UCHzlUiDD10)
  - [More HTML/CSS](https://github.com/processing/p5.js/wiki/Intro-to-HTML-and-CSS)
  - What is server side programming for?
    - [Database a service](http://shiffman.net/a2z/firebase/) controlled by p5.js client.
    - [web sockets for real-time communcation](https://www.youtube.com/playlist?list=PLRqwX-V7Uu6b36TzJidYfIYwTFEq3K5qH)
    - [Basics of node](http://shiffman.net/a2z/server-node/), [making an API in Node](http://shiffman.net/a2z/node-api/)
  - [Processing](http://processing.org)
  - Open source
    - How do artists make and adapt tools for themselves and their communities, like Processing, p5.js, openFrameworks, etc?
  - How do you  get involved with this?

##### Mantras
- "Practice is the best of all instructors." - computation requires practice
- "An agreeable companion on a journey is as good as a carriage." - look to your classmates for help too
- "While we stop to think, we often miss our opportunity." - sometimes you need to take a leap of faith
- "When two do the same thing, it is not the same thing after all." - encourage students with similar ideas
- "The bow too tensely strung is easily broken." - don't get too stressed out
- All of these are from Plubius Syrus.(42 B.C.)

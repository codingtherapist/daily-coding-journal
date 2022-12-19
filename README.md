# My Daily Coding Journal

An informal daily journal with coding activities, research, meetings, musings and more :) <br>


![Photo of author smile with the caption: learnign and buiklding using the MERN STACK Daily coding journal](https://res.cloudinary.com/dtamwfybo/image/upload/v1666889879/Why_I_left_Healthcare_21_vvigwd.png)

<b>Note</b>: This repo will contain excerpts from my personal code journal which I started on January 29th 2022 and started using with more frequency around June of 2022. These excerpts were not originally meant for public consumption and may have grammar errors. I want to preserve the entrees for what they were rather than edit them to perfection.<br><br>

This repo starts on May 28, 2022. If you'd like to read excerpts from earlier check out:

- [ <b>Part 1</b> of this series which details the first 2 months of learning how to code](https://www.africakenyah.com/learning-to-code-part-1/)

- [ <b>Part 2</b> of this series which details the middle 3-4 months](https://www.africakenyah.com/learning-to-code-part-2/)

- [ <b>Part 3</b> of this series which details the next two months](https://www.africakenyah.com/learning-to-code-part-3/)

## Building in Public 

### Nov 14
Coding questions for studying with group:
- What is scope / lexical scope in javascript? 
	- Scope = area visible and accessible to other code
	- Function scope is to access variables from parent scope
	- Place in which item was created
	- Lexical scope is where its defined, children have access to parents 
	- So for example putting a vsariable inside of a function its a lexical scope
	- Anothing outside of function is global scope
	- Lexical scope is wherever you define the variable 
	- Can be in function or be global
- What is polymorphism?
	- The practice of designing objects to share behaviors and takes advantage of inheritance
	- Base, subbasses that inherit from car and then add their own
	- Allows you to extend objects and add different methods
	- Uses protoypal inheritance
	- https://www.javatpoint.com/javascript-oops-polymorphism
- Describe the difference between <script>, <script async> and <script defer>.
	- <script> HTML parsing is blocked, script is fetched and executed immediately. 
	- <script async> script fetched parallel to HTML parsing and executed as soon as possible <script defer> script fetched parallel to HTML parsing and executed only when page is finished parsing 
	- Use: Use async when the script is independent of other scripts on the page Defer is useful when the HTML needs to be fully parsed before executing 
	-Example: <script async> could be used for analytics scripts (independent of other scripts on page) <script defer> must not contain document.write
- Why is it generally a good idea to position CSS <link>s between <head></head> and JS <script>s just before </body>? Do you know any exceptions?
	- Good idea to position CSS between head so it can run load and render before loading page. JS scripts just before body so it runs after the page is rendered
	- CSS rendered before it gets to DOM so thats why
	- Dom rendered from top down do javascript last so it wont render slowly, allows HTML to be parsed first
	- Exceptions = jquery, only executes after document is read

### Nov 10
- 12pm Job interview for technical writing position (offer not extended)
- Coding question studying
- What is recursion and give an example using javascript?
	- A function or algo that calls itself directly or indirectly
	- Corresponding function is called a recursive function
	- A recursive function must have a condition to stop calling itself. Otherwise, the function is called indefinitely.
	- Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write.
	- https://www.javascripttutorial.net/javascript-recursive-function/
- What is an algorithm
	- A set of instructions like a function
- Why is nodeJS single threaded
	- Nodejs is is asynchronous and has an event loop 
	- Eliminates need to create more threads and reduces memory and resource uses
	- Similar to javascript and inspired by the callback mechanism
- Explain callback in Node.js
	- Call when a task is complete and prevents blocking
	- You can have other code run in the meantime
	- Nodes can process a lot of requests without waiting for any function to return



### Nov 9 
Banki morning practice
- What kind of things must you be wary of when design or developing for multilingual sites?
	- You must be wary of design 
	- Globalization, making sure you can serve it and some languages are written from right to left
	- You have to worry about display and format
	- Static graphics or images in a different language buttons
- What are data attributes good for? 
	- To add what kind of data your referencing
	- Like building a calculator, adding more information to specific things in client side javascript
	- Has custom data rather than CSS classes and event listeners for each
	- Adds extra info to html that is more secure
- Describe a float and how they work
	- Floats float the text around the image and the image floats around the top left side corner and allows for text wrapping around image
	- May need to use clear fix to fix the items below so it doesnt break the display of the page of the things that come after it
- Describe the z index and how stacking context is formed
	- Creating depth (think of the hair salon project) having names overlap their pictures
	- Computer screen is flat, CSS gives you margins padding width and height 
	- Z tries to come out the screen at you, with z index, 0 is flat, if you want it to come out you go up from zero so higher the z index, the closer it is to you, the lower the further away it is
	
- Explain why the following doesn't work as an IIFE(Immediately Invoked Function) Expression: function foo(){ }();. What needs to be changed to properly make it an IIFE?
	- Use an IIFE when you want a function to immediately run without being called or needing a click for it to happen
	- Basically you have to wrap the whole function in parentheses
	- Design function known as self executing anonymous function which has two parts
	- Anonymous function enclosed within the grouping operator ()
	- Prevents accessing variable globally
	- (function foo(){})()
- What's the difference between a variable that is: null, undefined or undeclared? How would you go about checking for any of these states?
	- Null: an intentional absence of a value (falsy)
	- Undefined: means it has been declared but not given a value, theres space in memory  (falsy)
	- Undeclared: variable that doesnt exist
	- Console.log it and see what the answer 
	- Conditional boolean check
- What is the difference between classical inheritance and prototypal inheritance?
	- Protoypal inheritance is built it and have objects with proto in them that can be used outside of the object
	- Classical there needs to be some type of connection to inherit it, its more strict and needs to be explicitly
- What are the pros and cons of functional programming vs object-oriented programming?
	- Functional programming is simpler and just requires use of functions
	- Functional programming makes it harder for many ppl to work on bc data is not encapsulated so you may mess it up by adding or changing things
	- Function function, no way to nest things or hide things or protect them, no flexibility or security
	- Mainly used for machine learning or big data in a matrix
	- Object oriented everything is an object and it encapsulares data to make it easier to add to and work with with different people without messing up other parts of the program
	- Oop is more complex and can get out of hand easier bc of so many different components
	- Four pillars of OOP complexity is really important
		- Abstraction
		- Encapsulation
		- Inheritance
		- Polymorphism
- What are the features of nodejs
	- Single threaded
	- Asynchronous
	- Event driven
	- Access to the file system and server
	- Cross platform
	- Run javascript without needing a browser
	- Easily scalable
	- Allows access access to package managers including npm
	- Unopinionated
	- Quick data streaming, minimal buffering
- How do you update NPM to a new version in Node.js?
	- Check version npm -v ,if new update npm update -g
- What are “types” of data
	- Tells computer how to use data
	- Primitive (boolean, string, number, symbols, undefined, null etc)
	- Compound (objects, arrays, lists, hashes, structures, pointers)
- What are data structures
	- Arrays, stacks, queues, linked lists, trees, graphs, heaps


### Nov 8
Study Questions
- What does a doctype do
	- Tells the browser which version of HTML the page is coded in, first line of document
<html doctype=
- How to save a page with multiple languages
	- Putting it under doctype
	- Language attribute lang= en
- What is a CSS selector specificity and how does it work?
 	- Telling us which part of the HTML to apply the rules to
	- Html tag has lowest specificity, classes can be a group of tags, ids have ever higher and can only have 1 !has highest and overrides them all
- Difference between resetting and normalizing CSS
	- Resetting gets rid of all margins and styling , normazlie makes it have a style that is standarzides throughout browsers
- Prototypical inheritance
	- Whatever the parent attributes are goers to the the function within
	- All objects have a proto property, if youre trying to access a property in an object itll keep searching for them until it find it unti it gets to the javascript object
	- Like a dog object with a bark property
	- Dog object with a “bark” method (funtion), golden retriever object like goldenretriever.bark() itll look for the bark method in the other object
	- Above is how you would call the method
- What is is AMD and commonJS
	- AMD is better for the browser because its Asychronous and doesnt just load one huge file
	- CommonJS is sycnronous and used for servers
	- Module loaders are libraries that can handle loading modules 
- Can you name two programming opparadigms important for javascript
	- OOP and functional programming
	- Functional
	- Simple function based programming
	- OOP
	- Prototypal inhereteance object based 
	- Nodejs
	- Its a  javascript runtime that can be used in any IDE and run javascript without using the browser
	- Very fast since its built on chrome and v8 javascript engine
	- Features of nodejs
	- Fast, asynchronous, single threaded but highly scalable


### Oct 31
- Meeting with Mentor
(These notes below are notes I took during out meeting and may not have the best grammer or flow)
- Went over
 	- Method, arrays for loops,
	- Basic data structures
	- Lists, arrays, maps, json objects, map data types
	- Stacks and queues
	- Searching or iterating through a list, string parsing, parse string
	- Binary search is for sorted lists and they can check value in middle and see if the thing youre looking for is greater or less than value
	- Know differente between a list and set and when to use them
- Map
	- A collection of things and values and you look it up by a keys
	- You can look up something with a value
	- In memory theres a pointer to some thing
	- Example
		- Keeping track of certain number of stocks
		- Write a function that takes in name of stock and give you back current price
		- Function that updates the price for stock ticker
		- Need all of it to happen in real time
		- Function updates and reads the price
		- JSON object with two fields, name of stock and price
		- Put it in an array and find price

- Trees and graphs for big tech
- Insertion or sorting algos
- "Do i need to sort this before i do anything or not?"
	- Should know how to do basic things to manipulate array
read/ write array/ splice it/ take thing out of it etc
- Map is a list of pointers
- Looking up a single value itll be better to map it and point it to a value
- Hiring managers are looking at how you approach the problem
	- Dont just start writing
	- Ask questions
- Edge cases
	- Asking clarifying questions
	- Making sure you think about what you want to do before you write code
	- An outline of the code your going to write
	- Asking questions a lot before you write things
	- How you take feedback, throwing something extra in ther and how you deal with it
	- All this is more important, can you solve a problem, can you adapt
	- Not expected to know the most efficient route


### Oct 30
- Tutoring going over API call requests and mongoDB
- Codewars!

### Oct 29
- Created Stretch app JSON objects
- Make a simple API call request 
- Build an independent API using nodejs server


### Oct 28
- Codewars
- Banki with javascript methods 30 mins
- OOP vs functional explanation
- Film weekly update
- Banki 3 questions
- Ideas
	- Walk through of stretch project
	- Byte Sized Coding Lessons
- OOP vs functional programming
-String and array methods to know
	- Map, reduce, etc


### Oct 27
 
- 1 hour daily virtual standup completing 6kyu codewar 
- Frontend Masters Data structures and algos course 1 hour
- Javascript review 1 hour
- Add blog entry on personal blog via vscode
- NodeJS fundamentals review
- Meeting with recruiter 3pm
- 1 hr meeting with a Sr management consultant who works as a full stack developer for a tech company.

Today I did the daily standup of codewars with my study group as usual, but with a little more focus and energy. <br><br>

<b>Coding problem:</b><br>

<i>Parameters</i>:<br>

We worked a on a problem that required us to take in a string (we chose the word "Baddies") and return a string of “(“ or “)” representing the characters that did not repeat [represented by “(“] or did repeat [represented by “(“].
- The string we would be searching for duplicates could be represented by letters (upper case and lower case), numbers, empty spaces or special characters.
<br><br>

<i>Example:</i>

The word "Baddies" should <b>return</b> "(())((("
<br><br>
` console.log(duplicateEncode(Baddies),"(())(((")`<br><br>
<i> Rationale:</i>

- To create a function that could break down the string “Baddies” and put it into an array of letters, we used the <b>slice()</b> method. 
- To make sure all of the letters were lowercase we used the method <b>toLowerCase()</b>. 
- To check whether there were duplicates we used indexOf() to search the beginning of the arrays indexes for characters, and <b>lastIndexOf()</b> to check the end of the array. 
- To place these methods on each letter of the array we created, we used <b>map()</b>.
- We knew if any of the characters came back with different indexes for indexOf() or lastIndexOf(), that must mean the characters were repeating, as if there was only one character type the indexes of both methods would be the same.<br><br>

<b> Solution:</b><br>

`function duplicateEncode(word)` <br>
   `return word` <br>
     `.toLowerCase()` <br> 
     `.split('')` <br>
     `.map( function (a, i, w) {` <br>
       `return w.indexOf(a) == w.lastIndexOf(a) ? '(' : ')'` <br>
     `})` <br>
     `.join('');` <br>
 `}`
### October 26
Yesterday I went to a HackerX Tech conference and met a few software engineers and was able to talk with 6 companies hiring for Software Engineers. Most of the companies wanted engineers who were well versed in React and NodeJS which was good. Three of the companies were looking for engineers with a good amount of experience.  One of the companies I’ve been interested in were there and we were able to exchange information which was nice. Meeting other engineers and talking with them about their experience was great.<br><br>

Today:
- Meeting with one of my mentors 2 hours covering interview questions he asks entry level software engineers. I’ll put a few of the things he says would be good to know below


#### Interview questions
What do you want an entry level person to know well?
- Data structures
 - Array Traversal 
 - Find Nth Item 
 - Removing item
 - Shifting item

- Linked list
	- Iterating through a single list
	- Next pointer
	- Iterating through a doubly linked list
	- Prev and next pointer
		Add, remove, search 
		O(n) 
- Create stacks 
- Create Queues
- O(n) 
- Adding
- Removing
- Searching
- How can you create a stack from a queue and vice versa 

- Stack 
	- Pop
	- Peek
	- Add


### August 25- October 20th
During the past month my journals notes were pretty sporadic. They were mostly filled with references to things regarding data bases, MVC and things I needed to look up for my 100 hour full stack project. It was also and filled with personal information from meeting with different engineers and recruiters I met at virtual tech conferences. <br>
Most of my time was spent finishing up my passion project which is live at https://www.yourstretchbreak.com<br>
 ![screenshot of my stretch break app](https://user-images.githubusercontent.com/96845068/193476091-a9e68a0f-52ae-42dd-a61c-8c35fb0be827.gif)<br>
  - A 5-minute stretch break web application for developers and computer users.   
    -  Built with <b>HMTL, CSS, Javascript, Nodejs and MongoDB</b>.
    - Includes a timer and 40 stretches to try at your desk
    - Ability to upload your own stretches in your profile
    - An API to retrieve yoga poses based on body parts from a mongodb database with photo hosting from Cloudinary will be added to optimize project.<br>
    - [Github Repo](https://github.com/codingtherapist/myStretchApp)
    - [Blog article about project](https://www.africakenyah.com/your-stretch-break/)

I'm pretty proud of my wireframe, and it helped me flesh out this p
roject to working application<br>


![display of homepage in mobile view with html vscode open next to it](https://res.cloudinary.com/dtamwfybo/image/upload/v1665518366/wire1_cmlcju.png)

![display of homepage in mobile view with html vscode open next to it](https://res.cloudinary.com/dtamwfybo/image/upload/v1665518366/wire2_swux3k.png)

### May 28<br>
Note: Entries go in ascending order from this point until August 24<br><br>
Can't believe today was my last day as an occupational therapist providing direct care! I am so excited to start learning full time and commit 100%. This morning I'm finally getting my dev stuff organized with a plan of attack. I will be restarting #100daysofcode on Monday for a fresh commitment to code at least a little every day. This is the first Saturday in actual years I haven't spent my morning catching up on therapy notes.

### May 31<br>
* 2 hours of figuring out how to build my portfolio using Hugo<br>
* 2.5 hours of javascript review<br>
* 1 coffee chat w/ a developer  <Br>
* 1 codewars question 
* 1 reward of vegan pho when done

### Jun 1<br>
* 2 hours #100devs Javascript review and exercises<br>
* 1 hour of trying to figure out Hugo to build a static portfolio site<br>
* 1 codewar question <br>
* 1 hr tutoring help <br>
* 1 hr advice + coding roadmap review from my SWE cousin after he's done working :)


### Jun 2<br>
* 2 hours of the 8-hour #100devs javascript review and exercises before my flight <br>
That's all for today as I am flying back from Atlanta to DC to get to my home office where my streaming gear is waiting for me to play around with yayyyyy

### Jun 5<br>
* JavaScript review covering basic functions and methods - a lot of me shaking my fist at my screen trying to use my terminal correctly while setting up my portfolio 
* A lovely meeting with @ SchipThatCode going over twitch and streamlabs tips


### June 6
* Easy codewars problem, had to google to figure it out but was able to at least write the pseudo codes before looking it up. <br>
* Finally finished editing a YouTube video on repetitive stress injury prevention for computer users

### June 7
* Did 2 hours of tutoring going over using the terminal, pushing to GitHub + Netlify - setup mic, camera + dl programs to figure out streaming for this week<br>
 * Reviewing object-oriented programming concepts

### June 8
Jun 8<br>
* An enlightening and motivating coffee chat w/ @ artsycoder533 
* Practiced pushing code from local to GitHub using terminal 
* Worked a little on my portfolio trying to use Hugo to build it (had a hard time making it work and synch with Netlify )

### June 9
* Long info-packed coffee chat w @ jalonen_lauri (helped me w my frustrations w/ the terminal + Github ) 
* #100devs class on making CRUD apps 
* Setup streamlabs for twitch streaming, created twitch transition + branded backgrounds using canva
* Used ohmyzsh framework to change my terminal to a light theme 
* 1 hr coding tutoring with an awesome dev pushing local files to GitHub + using Hugo framework for portfolio -
* Shot +edited my first tech Youtube video! 
* Attended @ lesbiantech conference + job fair

### June 10
* Finished editing +uploaded 2 vids to YT channel [why I left healthcare for tech](https://www.youtube.com/watch?v=IwyyKlABpTE) + [chair yoga for tech workers](https://www.youtube.com/watch?v=LoYgPYvEZhI&t=126s) 
* Learned a ton about CRUD + pieces needed for full stack apps incl express etc 
* Last #100devs class before our two week summer break (time to catch up!)

### June 11
Jun 13<br>
* Attended last day of @ lesbiantech, got to connect w some really cool indvs in tech as well as recruiters at a few companies I’m super interested in 
* Dug up some training I did earlier this year on using virtual + augmented reality in healthcare

### June 12
 A chill day <br>
* Moved slowly through some OOP material 
* Watched a few videos on using Blender (it seems so complicated w/ a lot of steps to make simple things but I really wanna play w it) 
* Casually watched an AR unity tutorial

### June 13
* Shot a 10min YT video [What Is Assistive Technology](https://www.youtube.com/watch?v=S-npp6P6eMM&t=21s) 
* Started fleshing out a blog post on assistive technology +why developers should be aware of it 
* Put tailwind on my todo list - Hugo + terminal shenanigans

### June 14
* Messed around with making old code cleaner by making objects 
* @ jalonen_lauri was kind enough to hop on discord and show me some stuff code on GitHub w/ real examples of OOP 
* Went to a wedding so didn't code more than a couple of hrs

### June 15
Jun 17<br>
* Finished up my studies w OOP 
* Coffee chat w @ metalandcoffee_ 
* Realized live streaming is prob not in the cards for me right now but reinvigorated my desire to vlog + blog about my projects 
* Worked a little bit on unscrambling old code to make objects again

### June 16
* Coffee chat w @ mrxinu, struck by how kind and cool they are 
* Chat w/ @ ThatAdrienne a former school psych, now a dev, very cathartic + inspiring conversation about therapist burnout and how therapists make excellent developers
* No coding today, hand pain

### Jun 20<br>
* Worked on a short article on why semantic HTML matters and its importance to assistive technology users 
* Did some design work for an ebook - watched more ideas on OOP 
* It was Saturday, I gave myself permission to rest a little


### June 21
* Finished designing ebook 
* Finished a blog post on semantic HTML
* Finally understand the four pillars of OOP and can explain
* Tried and failed to push code to GitHub for a few hours using terminal, will be getting help on this today

### June 22
Today I will<br>
* Finish my portfolio site if it’s the death of me
* Practice pushing local files to GitHub using terminal 
* Finally convert all the video files of my yoga poses to gifs for the stretch break generator I’m building

### June 23
* Today got together with my study group  
* Finally understood what an object constructor was
It is a constructor that takes in multiple objects and gives them all the same properties and methods
<b>Questions</b>
What is a class and how does it help with constructor objects?

<b>Wins</b>
Made a constructor that worked making my own TV shows with show name, genre, cast list, episode number

### Jun 28<br>
summary <br>
* Had really lovely coffee chats w @ metalandcoffee_ @ mrxinu @ ThatAdrienne they gave me so much insight on their experiences as SWE and many good tips 
* Worked every day on learning OOP and asynchronous programming 
*Got way comfier using GitHub

### Jun 28<br>
Summary <br>
* Awesome chat w @ hot_girl_spring, lots of fun hearing about her disdain for JavaScript LOL
* Started studying APIs 
* Worked on my portfolio still struggling using Hugo 
* Fun chat w @ ReedCodes about the wonders of CSS stylesheet templates

### June 29
* Discovered the wonders of a silent virtual study session for working on #100devs API hw + studied for 3+ hrs w my fellow code baddies
* FINALLY USED AN API AND GOT IT TO WORK 

### July 1
* Catching up on hw including a very long build of a simple full-stack app via watching @ mayanwolfe’s 6hr vod, she is so fun to watch!
* Silent study sessions with my code baddies to tackle more API stuff

### July 2 
* 3 hr silent code & study
* Connected MongoDB to my local server and learned a little about databases
* Messed around w terminal and Github using vscode
* Uploaded 2 yoga for computer users videos on YT

### July 3
<b>Journal Entry</b><br>
Today I learned:
* MongoDB is used to store data put into a form into a cloud, very cool, put in quotes and MongoDB will put it in its database
* Git terminal commands, placed notes on my wall for creating a local repo, adding a remote repo, and logging local changes to the remote repo 
* Looking into  building our own data sources that we can build what we want with MongoDB
* Learning how to put data into a database
* We need to do two things to show quotes from MongoDB Atlas to our users.
- Get quotes from MongoDB Atlas.
- Rendering the quotes in HTML with a template engine

<b>Wins:</b>
* Used EJS to generate HTML markup with plain JavaScript, got it to work by troubleshooting returned error message
* Figured out error message stopping local server from working (express.js not installed in the correct area, needed to be at the root of file)

<b>Struggles:</b>
Felt like I spent a lot of time on simple things and troubleshooting to figure out where to place files, but felt good I was able to figure out how to do most of the steps up to the point I stopped today, which is right before making the objects for the quotes.

<b>Notes:</b> Via B during silent study sesh chat-> ” video on installing Heroku CLI. I'd suggest watching it because that was my stumbling block yesterday and Monday.”
https://www.twitch.tv/videos/1315269230
 
<b>Random Web app ideas:</b>
* Making this prettier in a nicer format web app with automated dates and generated areas of concern
* Tarot card web app: make flip of card happen on the server side instead of a coin flip

### July 16th
- met with a software engineer at  NVIDIA 
- Met with engineer at Audible to work on javascript timer.
- got timer to work then at the end broke it, only goes one second on click
- need to figure out how to make click events not toggle off on click and instead bring up the next random picture in the array on the next click of button

### July 18th
- worked o CRUD app, unsuccessful. Netfily deploying old version of hugo blog site

### July 19th
- working on portfolio
- making containers using flexbox grid maker https://grid.layoutit.com/
- need to make a submodule for git clone

### July 20th
- Meetings:  1030-240ish working on CRUD, making card flip for tarot flip happen server side
- Worked on building a server using express, then putting card flip up through node and on local server
- Worked on github merges, pulls, working with another person on github
- Learned how to force kill a server using command lsof -i tcp:, to find the number key and kill -9 to kill server

### July 21st
- Worked on portfolio and blog
- Figured out portfolio tag on blog site, it is its own page that i am adding in my sites
- Need to finish projects (simplify stretch app and just add working timer, on back end you can add how many stretch breaks you took maybe as a daily counter!
- Meetings: mail chimp engineer 430pm
- Good idea to focus only on backend and API stuff to showcase that i know it and do minimal front end stuff
- Work on making yoga pose API, need to host pictures somewhere and make a database then figure out functions

### July 22nd
<b>Wins:</b>
- Figured out the hugo site build, i needed to deploy the site first LOL

- finished personal portfolio site
- learned about jekyll configurations for netlify, need to put in a gemfile and configure in terminal due to jekyll not being able to be uploaded without configurations
- build command jekyll build publish directory _site
<b>App ideas:</b>
- anonymous silent disorder and tips site
- Coding Therapy typing room
- Fine motor therapy room with typing area, fine motor exercises, stretches

### July 25
- finalized blog and portfolio, completely done essentially and live
-  attempted codesignal assessment, completely bombed and gave up after one question

### July 26
- Las olas sobe vegan studying
- Fixed my timer! I had to use setInterval in the function and set it to 1000 so that it could interval and run every second

### July 30
- researched open source accessibility project, NVDA has 2k open issues
- Researched open source projects accessiblity
https://www.digitala11y.com/open-source-accessibility-tools/
https://en.wikipedia.org/wiki/List_of_open-source_health_software


- Got help with timer, i put a div around all my ids instead of isolating the div with the name of the id 


### August 2
- Finished client linktree and simple site. 
- Spoke on a twitter space about networking

### August 5
- heroku issues
- folder within repo all info was in vs a folder in the repo itself. It likes everytign in the root folder
- cli and github version

### August 6
- finished hugo site, added readme to github projects
- shared finished work
- stopping timer
- clearinterval
- cleartimeout
https://stackoverflow.com/questions/9913719/are-cleartimeout-and-clearinterval-the-same
- why is clearinterval being passed in as a variable?
-https://www.youtube.com/watch?v=rBpRtu7GgpQ
- database
- s3 aws storage
- google photos is not secure, dont do it on person google account, create a dummy google account
- use better service to make it secure
- use this:
https://azure.microsoft.com/en-us/services/cloud-services/

- Multer npm package to upload files (may not need this)
- Npm website look at library and packages
- Configure vscode with prettier so you can see elements
- format with parents and etc,
- format parent and children format
 

### August 9
- Went over canonical tags, head files which are in themes lovit partial for graph tags for twitter
- Worked on part 2 blog of 1st six months of coding
- Worked on onboarding therapy clients and updated holisticaimtherapy website

### August 10
-mes build and webpack setting up bill system
- testing things out in production so if you break something you break
- provisioning
 - Servers
 - Bash scripts
 - Set procedure for what you execute
- docker for shell scripts

Databases
- how do we get data from point a to b
- How to get a list of yoga poses, queries that get executed, how do you optimize your database?

Servers:
- Backend operations unique to a specific company
-  a backend process is handling that, knowing how to set that p, creating an email server, configuring a server to handle those responses

Backend
- Focus more on optimizing server
- Think about whats needed to present data and optimize server for presentation of the data
- Doing more reads than write, more reads optimize server so there are more reads
- Tasks that are ran
- How are you going to set up flags? Etc
- Testing data using a node server to make sure end points are making sense
- Understanding how to interact with server with node, how to properly store dsdata and paradigms around that
- Launching servers and execute this application, make sure certain ports are available


### Auguts 11
- Worked on responsiveness for nasa api and stretch break app, added meta data 
- Added percentages for max-width: 50%; instead of hardcoding it by px. 
- Added in the calendar for NASAA API and increased accessibility with alt text, heading etc
- Still need to fix contrast etc

### Auguts 15
- Recorded simple video on MVC
- Started article on human-centered technical documentation

### August 17
- 1030 study sesh
Firebase 
- Not as easy to use as mongodb
- Using for straight up saving data mongo better
- Good for holding cards
- Fetch cloud pictures
- Using api to fetch clouds
- Try making api that fetches pictures of yoga poses
- Mvc
Cloudinary
- Have to hook it up to mongo db 
- Each image would have an id in cloudinary, but id in url then send url to database
- rascal 2 stream with soft delete
- Deletes in the dom but doesnt delete the database
- Or do it with local storage local to the user
- Or maybe they can delete just what they put
- Need a login
- Lecture on model view controller
- Why you would want to build your site with a different kind of architecture


### August 18
- Virtual coffee 12pm
- Uploaded video on human-centered 
Commits
- How many how often?
- Git kraken
- Conventional comments
https://github.com/commitizen/cz-cli
https://conventionalcomments.org/
https://www.conventionalcommits.org/en/v1.0.0/
https://learngitbranching.js.org/
https://ohshitgit.com/
https://github.com/Cerchie/git-cherry-pick-tutorial
- Do PR’s even for personal projects

### August 24
- Created a server for my stretch break!
- ran into issues with cors and dotenv, just needed to reinstall the dependencies with npm
- Created the google cloud storage of my gifs, need to put the path into a JSON object to be called by click, and add all the click events to make it work
- Need to upplaod on heroku instead of netlify since there is a backend
- Need to look into opensea maybe this is what ill sue tfor this? We will see.

Digital ocean vs heroku
- PAAS vs IAAS
freelance
- Swapping pictures out, doing menu, adding packages and prices to packages
Homework 
- look up strings methods


## To be continued 
Interested in seeing further than August? Click the links at the begining of this repo. Parts 1-3 are avaiable to read via blog articles documenting my first 6 months of learning to code.

	(This journal lives on a google document that I add to daily, I will be uploading the daily posts little by little as I have time :) )






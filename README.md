# My Daily Coding Journal

An informal daily journal with coding activities, research, meetings, musings and more :) <br>
<b>Part 1</b> of this series which details my first 2 months of learning how to code can be found [here](https://codingtherapy.hashnode.dev/what-i-learned-learning-how-to-code)

<b>Part 2</b> of this series which details the middle 3-4 months can be found [here](https://codingtherapy.hashnode.dev/my-first-6-months-of-learning-web-development-part-2)

![Photo of author smile with the caption: learnign and buiklding using the MERN STACK Daily coding journal](https://res.cloudinary.com/dtamwfybo/image/upload/v1666889879/Why_I_left_Healthcare_21_vvigwd.png)

<b>Note</b>: This blog post will also contain excerpts from my personal code journal which I started using with more frequency around June of 2022. These excerpts were not originally meant for public consumption and may have grammar errors. I want to preserve the entrees for what they were rather than edit them to perfection.


## Building in Public 
### Oct 27
 
- 1 hour daily virtual standup completing 6kyu codewar Frontend Masters Data structures and algos course 1 hour
- Javascript review 1 hour
- Eloquent Javascript read 5 pages
- Add blog entry on personal blog via vscode
- NodeJS fundamentals review
- Meeting with recruiter 3pm

Today I did the daily standup of codewars with my study group as usual, but with a little more focus and energy. <br><br>

<b>Coding problem:</b><br>

<i>Parameters</i>:<br>

We worked a on a problem that required us to take in a string (we chose the word "Baddie") and return a string of “(“ or “)” representing the characters that did not repeat [represented by “(“] or did repeat [represented by “(“].
- The string we would be searching for duplicates could be represented by letters (upper case and lower case), numbers or special characters.
<br><br>

<i>Example:</i>

The word "Baddie" should <b>return</b> "(())(("
<br>
` console.log(duplicateEncode(Baddies),"(())(((")`<br><br>
<i> Rationale:</i>

- To create a function that could break down the string “Baddie” and turn it into an array or letters, we used the <b>slice()</b> method. 
- To make sure all of the letters were lowercase we used the method <b>toLowerCase()</b>. 
- To check whether there were duplicates we used indexOf() to search the beginning of the arrays indexes for characters, and <b>lastIndexOf()</b> to check the end of the array. 
- To place these methods on each letter of the array we created, we used <b>map()</b>.
- We knew if any of the characters came back with different indexes for indexOf() or lastIndexOf(), that must mean the characters were repeating, as if there was only one character type the indexes of both methods would be the same.<br><br>

<b> Solution:</b><br>

`function duplicateEncode(word){<br>
   return word<bR>
     .toLowerCase()<br>
     .split('')<br>
     .map( function (a, i, w) {<br>
       return w.indexOf(a) == w.lastIndexOf(a) ? '(' : ')'<br>
     })<br>
     .join('');<br>
 }
`
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
(this journal lives on a google document that I add to daily, I will be uploading the daily posts little by little as I have time :) )
- Africa 10/26/22





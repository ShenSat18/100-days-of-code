
# 100 Days Of Code - Log

-------------------------------
### Day X: October X, 2017

**Today's Progress**: 

**Thoughts:**

**Learnings:**

**Link to work:**

**Tomorrow:**

------------ Example -------------------
### Day 1: August 1, 2017 

**Today's Progress**: Wrote a script that extracts the content of a webpage in HTML format.

**Thoughts:** This was the hardest day of coding by far, ironically. I just couldn't find the relevant gem to extract data from a webpage - it's taken me like 4 hours! I eventually came across Nokogiri gem which does the job. Also used github for the first time. Not sure how I'm going to store scripts and projects here as I progress, but I'm sure it'll become clear!

**Learnings:**
- use The [Ruby Toolbox](https://www.ruby-toolbox.com/) for finding relevant gems (they are ranked!)
- there isn't always a simple, easy-to-understand gem to get what you want. Sometimes you'll just need to copy & paste (eg to get the Nokogiri gem to work (and download a webpage's html) I had to use [this solution](https://gist.github.com/fnichol/867550))

**Link to work:** [extract webpage script](https://github.com/shen-sat/100-days-of-code/blob/master/scripts/extract_webpage)

-------------------------------
### Day 2: August 2, 2017 

**Today's Progress**: Wrote a script that sends tweets.

**Thoughts:** A lot of messing with Gems again, but this time I just copied and pasted rather than dive into the abyss. I can now interact with the Twitter API which is amazing. I've been copying and pasting snippets of code and simply running them a bit aimlessly; they work fine, but I'll need to actually understand how the snippets work so I can start calling up data that I want.

**Learnings:**
- Using gems doesn't hand me what I want on a platter. I still need to understand the commands in order to manipulate it and get what i want
- without a specific task (eg retrieving a specific tweet), I tend to be a bit aimless in my learning.

-------------------------------
### Day 3: August 3, 2017 

**Today's Progress**: Systematically worked out how to access data within tweets.

**Thoughts:** I kind of stumbled across the answer yesterday, but today I spent time working it out. It seemed like data was stored in hashes within hashes. But the the section where picture data is stored seems to be an array, which I didn't understand for a while. However, layter in the day I realised that this may be because you can have more than one media (eg picture, gif etc) within a tweet - therefore you need to build an array to store data on each media. I'm going to test this theory out tomorrow!

**Learnings:**
- I'm decent at working things out, even though it takes a bit of time, I'll get to a solution eventually. 
- I may need to set aside a time limit because I'm still spending too much time everey time I hit a 'bump' - from now on, if I can't work something out within a couple of hours I will leave it. I can save the problem as a script and bring it up at a future meetup, possibly.

-------------------------------
### Day 4: August 4, 2017 

**Today's Progress**: Definitively worked out how to access multiple pics' urls in a tweet. It's all about arrays!

**Thoughts:** This didn't take much time, compared to yesterday. I want to show people what I've built now, so Ive started looking at places to 'host' the app I end up buidling - I had no idea how to do this andresearching tis has actually taken up the most time today. I have a couple of solutions now that I'll try tomorrow (Google Cloud and Heroku). Once, I've tried them, I'll go back to writing code that searches for pixelart tweets and returns images with a specified fave count.

**Learnings:**
- Media in tweets are stored in arrays. Once you access the relevant image in the array, then you can access it's url, id etc
- I need to 'deploy' my app to a web server so that other people can use it

-------------------------------
### Day 5: August 5, 2017 

**Today's Progress**: Played around with the search function in Twitter's API

**Thoughts:** Search returns arrays, and I know how to use these now ;) I haven't made great progress today but that's probably because I have been coffee-shop hopping. I also reached out to some #100DaysOfCode peeps for help in learning to deploy my app - they both responded which is awesome.

**Learnings:**
- Twitter API search returns an array
- Reaching out to#100DaysOfCode people is awesome

**Tomorrow:**
- write code that can take in two search terms (hastag and a username - when you tried to look for Kratos' last tweet, it didn't work)
- write code that can return top #pixelart tweets according to fave count
- look into the responses you got for deployment

-------------------------------
### Day 6: August 6, 2017 

**Today's Progress**: Played nore with the search function in Twitter's API. I found out how to use the filter function

**Thoughts:** Not everything has to be done with complex code! I found out that inserting things like "filter:media" can actually be typed into the normal Twitter search AND into code to retriev relevant results.

**Learnings:**
- there are a [bunch of normal Twitter search functions](https://dev.twitter.com/rest/public/search) that can be used in code

**Tomorrow:**
- write code that uses the above normal twitter search funstions to retrieve #pixelart tweets from @pixel_dailies timeline
- start reading about Git

-------------------------------
### Day 7: August 7, 2017 

**Today's Progress**: I can now retrieve only posts from pixel_dailes that contain images. Came up against Twitter's API request limits.

**Thoughts:** I'm not sure what counts as a request, but I di know that when I cast my net wide for searches, I am now coming up against limits set by twitter relating to number of requests per period of time. I need to find out why this occurs, so that I can set limits on my searches accordingly.

**Learnings:**
- searches for #pixelart in a day may exceed the Twitter API request limit and return an error

**Tomorrow:**
- learn how search requests are restricted

-------------------------------
### Day 8: August 8, 2017 

**Today's Progress**: Found code that'll let me know how many requests I have per search.

**Thoughts:** As above really. Not really sure how this will affect the user though.

**Learnings:**
- new code

**Tomorrow:**
- so unfocused - gonna make a plan for the app tomorrow

-------------------------------
### Day 9: August 9, 2017 

**Today's Progress**: Made a plan for the app. I can sort through #pixelart tweets for those that have media.

**Thoughts:** Having a plan is better, but I still feel like I'm working a bit slow. This is probably because I'm working from home. Need to get out!

**Learnings:**
- Twitter outputs time in UTC
- can sort by using if [statement]?

**Tomorrow:**
- I can sort by media, but what happens if a tweet has a gif? I need to rule gifs out somehow
- properly incorporate time limits (eg tweets only from 24 before search initiated)

-------------------------------
### Day 10: August 10, 2017 

**Today's Progress**: Pushed my first git commit

**Thoughts:** Just video tutorials today then some very brief coding. I feel very positive about using git in future for my scripts. From what I've seen and read, git is also a useful tool to learn for future jobs.

**Learnings:**
- Git is version control and a collaboration tool
- Git can be used with github to store work

**Tomorrow:**
- Put current script to git/github

-------------------------------
### Day 11: August 11, 2017 

**Today's Progress**: Script now pulls pixelart tweet in last 24hours with most likes

**Thoughts:** Feel super happy with result so far. Using Twitter search operators has allowed me to limit my search calls. I've pretty much finished back end, now to move on to front end.

**Learnings:**
- I've found d out that some objects within a tweet eg the 'type' hash within a tweet, don't have methods that other objects do and have to be accessed hash by hash.
- Twitter search operators are so much more powerful than I thought initially. Eg I can search for tweets with media rather than filter tweets with media out of an array

**Tomorrow:**
- Github and Heroku and front end

-------------------------------
### Day 12: August 12, 2017 

**Today's Progress**: Uploaded my script to Github using git

**Thoughts:** Slow progress today, but only because I'm on my friend's stag!

**Learnings:**
- Everytime I make a change to my local files, I should push commit and push the change. Otherwise version control can get a bit messy.

**Tomorrow:**
- Finish Heroku tutorials

-------------------------------
### Day 13: August 13, 2017

**Today's Progress**: Read some of Hartl's Rails tutorial.

**Thoughts:** Started on DevTips's Rails/Heroku tutorial but it feels to complicated. Hartl's book seems a lot more beginner friendly and it aims to get user to make a simple web application first

**Learnings:** 
- Rails web apps as a default come pre-packaged with an app 'structure' as soon as you create one.
- Bitbucket, unlike Github, allows you to create private repos for free

**Tomorrow:** Go through first chapter and create and deploy my first Rails app

-------------------------------
### Day 14: August 14, 2017

**Today's Progress**: Started creating my first web app

**Thoughts:** Slow progress today, because I didn't prioritise coding. I need to do coding first thing in morning, or first thing after gym.

**Learnings:**
- You can set the default page for the web app by defining an action in the application controller script, and then referring to that controller action in the routes script

**Tomorrow:** Finish app and deploy to Heroku

-------------------------------
### Day 15: August 15, 2017

**Today's Progress**: deployed a hello app to Heroku

**Thoughts:** this was tricky because of git - the Hartl's tutorial required me to set up a repo via the command line rather than simply cloning one from github. I messed up and had to do it again, because Hartl's instructions weren't quite right. Luckily there is a [youtube video](https://www.youtube.com/watch?v=T9h8Yl5bhJE&index=2&t=194s&list=PLunaYManlK3shgk_9iz_RQTa8J0kpeR-h) that has accurate step by step instructions. 

**Learnings:** once I have given github my public SSH key, I can set up a repo locally and send it to github

**Tomorrow:** find out how (eg tutorial) to put my app online.

-------------------------------
### Day 16: August 16, 2017

**Today's Progress**: Manipulated my rails hello_app_v2 to redirect to urls defined by me

**Thoughts:** Using the controller script in a rails app, I can state which url the app should go to. This bodes well for my pixelart twitter app, but making whole rails app for a static app seems like overkill. Could there be another, simple way to build an app from the ground up?

**Learnings:**
- I can put secret data (like private keys) directly into Heroku and acces them from script using ENV['YOUR_KEY']
- I can put script within a controller method (that a route points to) that will automatically be run on launching the app

**Tomorrow:** see if I can run scripts via Heroku without having to use rails

-------------------------------
### Day 17: August 17, 2017

**Today's Progress**: learnt about the Sinatra gem

**Thoughts:** Didn't do my full hour. Annoyed as I had all day!

**Learnings:** Sinatra gem takes a request to go to the root url and does an action that you specify. Super handy for my app!

**Tomorrow:** Try out Sinatra gem

-------------------------------
### Day 18: August 18, 2017

**Today's Progress**: used the Sinatra gem to display twitter images from my app

**Thoughts:** Didn't work again as hard as I woul've liked. Plain bad organisation. I really need to do my hour of coding as early as possible.

**Learnings:** Sinatra gem is great, but I'm only redirecting to the pixelart image url at the mo - I can't put in any extra text.

**Tomorrow:** Find out how to simply insert pixelart image as an html image rather than directing user to the image url.

-------------------------------
### Day 19: August 19, 2017

**Today's Progress**: learnt about the erb gem

**Thoughts:** I found out about this gem using this amazing site, [ruby monstas](http://webapps-for-beginners.rubymonstas.org/erb.html). More amazing free content. I should look into this site a bit deeper, it's written perfectly: it breaks down code line by line with explanations. My twitter code also didn't work for a bit which meant I had to re-learn the Twitter API - I need to make reference notes to come back to.

**Learnings:** 
- You can embed Ruby code (for example, a variable that stores the url for a pixelart image) into html code.
- I need to make ref notes for key learnings

**Tomorrow:** Combine Sinatra and erb gems to realise twitter app

-------------------------------
### Day 20: August 20, 2017

**Today's Progress**: rendered a page in html that displays the most popular pixelart image in last 24 hours

**Thoughts:** Great progress (decided to work in a coffee shop, sooo much more productive than working at home). I tested basic bits of code before combining them for my app: great for making sure there are no bugs. I should do this more often.

**Learnings:**
- testing tiny bits of code seperately and methodically saves lots of headache later on

**Tomorrow:**
- start making ref notes
- display other info (like fave count) alongside pixelart image
- use heroku tutorial to create gem files, procfiles etc to run app locally (using command 'heroku local')

-------------------------------
### Day 21-22: August 21-22, 2017

**Progress**: I've pretty much finished the app! 

**Thoughts:** I've completed the html code and ruby code and combined it so that my app works fine locally. When I upload it to Heroku however, it seems like it does,'t return an up-to-date fave count. Quite annoyed about this -- I can see why devs go on about bugs so much!

**Learnings:**
- [Heroku's tutorial to deploy a ruby app](https://devcenter.heroku.com/articles/getting-started-with-ruby-o#write-your-app) involves uploading code to their own github (and not my github)
- to run an app on Heroku, you need to change port from a number (eg 5000) to $PORT
- code doesn't seem to be run everytime from app launch (hence why fave count does not change)

**Tomorrow:**
- fix the bug--why isn't fave count refreshing as it should?

-------------------------------
### Day 23: August 23, 2017

**Today's Progress**: Fixed the bug!

**Thoughts:** Had to go back through the code line-by-line. Putting in 'puts' statements was really useful! Helped me identify which parts of my code were being run only once.

**Learnings:**
- I can't really use methods in Ruby on their own. They have to be attached to an object -- so a class of that object has to be made. Once I've made a class (eg Xmen), and then make the method (eg def claws) withn the class. I can then make an instance of that class (an object eg wolvie = Xmen.new) and I can then access an variables within the method by calling it by using object.method (eg wolvie.claws)
- only the last line of a method will be returned, so if you want a method to return a certain variable, list it at the end
- sinatra will run a page and then "listens" for a refresh. So if you want to run code on refresh, you have to call it within the sinatra piece of code 

**Tomorrow:**
- I need to re-learn methods, classes and variables so go back and do relevant codecademy chapter
- deploy to heroku local, then heroku final


-------------------------------
### Day 24: August 24, 2017

**Today's Progress**: Tidied up code, re-learnt classes and different types of methods and variables

**Thoughts:** My code works, so I'm happy not to re-factor it for now. But re-learning about classes, methods and variables means I could make the code cleaner. At the moment the code is one long chunk, but it could be split up into different methods. I think this would be useful if I had a more complex app that needed multiple instances (objects) that needed to be treated differently. As it stands,I only need to create on object for my app, so one long chunk of code is enough.

**Learnings:**
- creating objects are a way to run code in ruby. Once you have set up the class and its methods containing the code you want to run, then simply create an object and call the method to run the code.

**Tomorrow:**
- Deploy to Heroku finally
- Flash cards

-------------------------------
### Day 25-27: August 25-27, 2017

**Progress**: Deployed to Heroku! Learnt about coding games in Ruby

**Thoughts:** Finally finished my app! Feels really good, BUT I'm so hungry for my next challenge. I want to do something that I'm personally going to sue (like my Twitter app). I need to decide quickly so I can get on with it. The last two days have involved very sparse work - I've been in the countryside for a friend's bday, and I've learnt that I'm not comfortable asking for 1 hour to do my coding with people I don't know that well. I need to line up good reading materialfor situations like this. 

**Learnings:**
- I can't take my laptop on holidays with friends I don't know well
- Any class I create in RPG maker will inherit from classes that come pre-defined with the program. i learnt this from a [tutorial](https://forums.rpgmakerweb.com/index.php?threads/slip-into-ruby-an-introductory-guide-to-rgss-for-beginners.38900/) I found

**Link to work:** [My final twitter app](https://twitter-app-final.herokuapp.com/)

**Tomorrow:**
- flash cards
- Ruby book for when I'm on the move/on holiday
- next project

# 100 Days Of Code - Log

-------------------------------
### Day 28: August 28, 2017

**Today's Progress**: decided RPG maker is no good, read about Gosu gem

**Thoughts:** RPG Maker is not tinkerer-friendly. Gosu on the other hand looks promising, if tough - games are built purely from scratch. There could be a way to contribute code to the Gosu gem because it is so new.

**Learnings:** Gosu is agem for making games from scratch

**Tomorrow:** Build a simple game using Gosu

-------------------------------
### Day 29-30: August 29-30, 2017

**Progress**: Created a scene and movable character

**Thoughts:** The Gosu tutorial has helped me a lot. Especially the code for animation (Gosu.milliseconds / seconds_per_frame_needed % @animate_sheet.size). It took me ages to get my head around how it works, but once I realised Ruby does integer division, it all started to make sense.

**Learnings:** (Gosu.milliseconds / seconds_per_frame_needed % @animate_sheet.size) is a great way to animate from an array

**Link to work:** ![Alt text](https://media.giphy.com/media/l378gQP1EFNRzOufC/giphy.gif)

**Tomorrow:**
- put (Gosu.milliseconds / seconds_per_frame_needed % @animate_sheet.size) into Google Keep
- make player jump

-------------------------------
### Day 31-32: August 31-1, 2017

**Progress**: Made player jump

**Thoughts:** This involved a lot of maths, but I'm having lots of fun doing it because it relates to video games. Thinking in video game terms is so much fun.

**Learnings:** If you create a method that accepts an argument, eg def example(n), then you can't call that method without putting in an argument. (See Google Keep for an explanation).

**Tomorrow:**
- Mmke  a Google Keep note for the above learning
- add jump animation

-------------------------------
### Day 33-34: September 2-3, 2017

**Progress**: I can edit and import tilesets into my game using the map editor Tiled

**Thoughts:** It didn't work at first and for the first time the error code pointed to the gem I was using (gosu_tiled) instead of my own code. Using a bit of logic and trial & error, I was able to locate the problem and create maps in a way that satisfied gosu_tiled. I think I would like amend the gosu_tiled documentation at somepoint to reflect what I've learnt.

**Learnings:**
- images need to be imported as 'tilesets' and embedded in Tiled in order for gosu_tiled to recognise them
- images can be put into onbject or tileset layers and gosu_tiled will pick them up

**Tomorrow:**
- create a level using tilesets and run it
- work out how to import colliders
- write a rough draft for submitting to gosu_tiled's README for what you learnt today

-------------------------------
### Day 35-42: September 4-11, 2017

Progress**: Made the beginnings of a platformer

**Thoughts:** I spent waaaaay too much time on this! It was great at first and I've learnt tonnes, especially around using arrays and hases and classes, mthods and variables. But by the end, I was dipping into too much maths and not enough code. If it gets like this in future, I don't need to quit, but I need to scale down my idea.

**Learnings:**
- classes, methods and variables are great ways of organising code
- arrays and hashes are great ways of extracting information at for a given program state/moment in time
- if I spend more than 3 days on a problem, time to scale down! 

**Tomorrow:**
- work on idea for new game
- draw a rough map first and move a square around within boundaries

-------------------------------
### Day 43: September 12, 2017

**Today's Progress**: made a orthograpghi-game mockup

**Thoughts:** Seting up is quite simple because this is my third time. I'm also learning to take a break when it gets intense!

**Learnings:**
- Gosu.distance is another way to work out colliding states

**Tomorrow:**
- look through Gosu methods to see if there is anything that can help work out collision
- bound character by colliders
- look up FCC

-------------------------------
### Day 44: September 13, 2017

**Today's Progress**: Accessed new data within json Tiled file using hashes, arrays and loops 

**Thoughts:** I can't figure out an intuitive way to use rectangle colliders, so I'm figuring out how to use and import line colliders. This means using lots of arrays and hashes which is welcome practice. 

**Learnings:** .each_with_index |object, index| allows you to access an object in an array and its index number

**Tomorrow:**
- finish colliders
- look at FCC

-------------------------------
### Days 45-48: September 14-17, 2017

**Progress**: Colliders are now working

**Thoughts:** Colliders involve a lot of logic work, but even though it can be frustrating, it's also a lot of fun. I'm excited to build the next feature of the game.

**Learnings:** In an OR statement, if the first part is satisfied, the second part is not considered. For eg: in the statement 'if x = 3 || x = 4', if x equals 3, then the 'x = 4' part of the statement will not be run. To check for both parts, you'd have to use two seperate 'if' statements, one for each. 

**Link to work:** ![Alt text](https://media.giphy.com/media/3ohhwhpioio4kAoF9K/giphy.gif)

**Tomorrow:**
- level design
- FCC

-------------------------------
### Day 49: September 18, 2017

**Today's Progress**: created characters (mages) to interact with

**Thoughts:** This game is starting to look really cool! For the mage characters, I first had them sit within the Player class and it worked fine. But then thinking about it, it made sense to seprate these, so that the code would be easier to read. I therefore made a separate Mages class which works just as well.

**Learnings:** attr_reader is a great way for classes to talk to each other. The Mage class needs to know where the player is at all times, so I made the player's coordinates accessible to Game_Window class (via attr_reader) which then passes them to the Mage class 

**Link to work:**

**Tomorrow:**
- enemies!
- ask at Ruby Hacknight for FCC equivalent for Ruby

-------------------------------
### Day 50: September 19, 2017

**Today's Progress**: re-factored some code, started on enemy code. Also made a branch on Github.

**Thoughts:** I went to my first ruby hacknight! Mixed emotions: some devs don't know how to teach and are not that friendly, where as others have lots of potential to be great teachers/ruby-homies. I've started making changes to my game based on learnings from meetup, but boundaries arent working anymore.

**Learnings:**
- My code can be split into separate files and called from the main file using require_relative 'filename'
- I can make branches to make changes and pull them into main branch when I'm happy
- Ctrl X to cut (LOL)

**Tomorrow:**
- move code for detecting colliders into 'world' code as suggested by Pedro
- finish enemy code

-------------------------------
### Day 51: September 20, 2017

**Today's Progress**: fixed collider code, but had to stop to figure out Github

**Thoughts:** Github is quite confusing when starting to branch. I wasn't sure how to push to a remote branch for a while, but now I think I can get it.

**Learnings:**
- to change the upstream remote branch of your local branch, first use 'git fetch' then use: 'git branch --set-upstream-to origin/cyclops' (cyclops here is the remote branch name)
- if your local branch name does not match the remote branch name then git will warn you and give you instructions on what the avilable options are

**Tomorrow:**
- sort out github so I have the master branch and then the hacknight branch
-enemy code

-------------------------------
### Day 52-65: September 21 - October 4, 2017

**Progress**: I've finished my game! I've also started reading about object-oriented design (OOD). I've also reached out to a couple of coders for potential collabs.

**Thoughts:** It's taken me much, much longer than I expected, but the learnings have been worth it. I want to share what I've learnt, but not sure how. I'll reach out to see if any sharing possibilities are out there. I also feel confident I can use OOD in future to organise the messy but functional code I've written.

**Learnings:**
- I can scale my projects back a lot more
- seperating code into different files helps when navigating code and organising its structure
- hashes and arrays can be used to break into other programs and extract and organise info
- it's best to have local folders match remote counterparts for git control

**Link to work:** ![Alt text](https://media.giphy.com/media/3o7aD0A6aPBt3IQZva/giphy.gif)

**Tomorrow:**
- initiate opportunities to share learnings
- reach out to collabs, initiate collabs

-------------------------------
### Days 66-68: October 5-7, 2017

**Today's Progress**: Arranged code into OO classes. Made contact with my collaborators.

**Thoughts:** I have forgotten some things about the Twitter API. Using arrays is not as intuitive as I remembered!

**Learnings:**
- Twitter::SearchResults (ie the result I get when I call 'client.search') is not an array. I think it's an enumerable. I can convert it to an array by calling .to_a on it. 

**Tomorrow:**
- post game to any gosu forums
- work on options hash
- put above learning into a ref card

-------------------------------
### Days 69-71: October 8-10, 2017

**Today's Progress**: Worked out bug in partner's code. Researched sharing access Rwitter tokens/keys 

**Thoughts:** Slow day today. Felt like I haven't made much progress.

**Learnings:** There is no way to share tokens with partners in code and hide it from them at the same time. To work with a coder, they will either see and use your tokens, or they need to create their own.

**Tomorrow:** Same as previous post

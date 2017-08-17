
# 100 Days Of Code - Log

-------------------------------
### Day X: August X, 2017

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

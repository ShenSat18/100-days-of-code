
# 100 Days Of Code - Log

------------ Example -------------------
### Day 0: February 30, 2016 (Example 1)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts:** I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link to work:** [Calculator App](http://www.example.com)

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


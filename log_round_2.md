# 100 Days Of Code - Log

-------------------------------
### Day X: December X, 2017

**Today's Progress**: 

**Thoughts:**

**Learnings:**

**Link to work:**

**Tomorrow:**
-------------------------------
### Day 1: November 21, 2017

**Today's Progress**:write first tests for a game called fizzbuzz

**Thoughts:** Fisrt day kicked off with a bang. Admitted by ignorance around TDD (test driven development) and asked for help. Got paired with Lewis - he might not be more experienced than me (he is only a few weeks into Makers Academy) but he knew more about me re: TDD. I followed him stepby-small-step to write tests and write fizzbuzz 

**Learnings:**
- save beginner concepts for Meetups
- break the tests down as small as possible. Each test should relate to one tiny bit of functionality

**Tomorrow:** continue writing tests for fizzbuzz
-------------------------------
### Day 2: November 22, 2017

**Today's Progress**: finished fizzbuzz functionality

**Thoughts:** writing tests led me to write the code for the program in a way I wouldn't have otherwise, because of the order/structure of my tests. It's not very read-able but it does work!

**Learnings:**
- tests can get you to make a functional program, but refactoring is required after to make code elegant. And because you've written tests for everything, if you make a mistake whilst refactoring, tests will let you know! 
- learnt about require and require_relative (made a note on Google Keep)

**Tomorrow:**
- look at [Makers academy blog](https://blog.makersacademy.com/an-introduction-to-tdd-in-ruby-72f0a8536509) and:
  - refactor your code according to the red-green-refactor principle
  - do the last challenge at the end
  
  -------------------------------
### Day 3: November 23, 2017

**Today's Progress**: solved some of the game engine maths for Algebra Jungle 

**Thoughts:** Didn't get get nearly as much coding as I wanted to get done. Mostly maths logic for 'balance' in game. Frustrating, but even Steven couldn't solve the problem at the heart of the balance mechanic.

**Learnings:** Not much learning unfortunately, except take more breaks when thinking about a problem.

**Tomorrow:** see Day 2 entry.

-------------------------------
### Day 4-5: November 24-25, 2017

**Progress**: Completed Makers challenge on TDD. Read about Chrome extensions

**Thoughts:** The Makers academy challenge was surprisingly straight forward. It was fun messing around with Ruby's built-in classes. Chrome extensions on the other hand are a bit more complicated. I feel like I need more basic HTML/CSS/JS knowledge before jumping into the chrome extension, because at the moment, I can't read the examples given by [Google Developers' guides](https://youtu.be/e3McMaHvlBY?list=PLCA101D6A85FE9D4B). Freecodecamp might be a way through this, ie to develop my front-end knowledge

**Learnings:**
- Stating an in-built class in Ruby and then defining a new method inside it will mena you can call that method on any object of that class.
- Chrom extensions use a mixture of HTML/CSS/JS

**Tomorrow:** work through Freecodecamp

-------------------------------
### Day 12: December 2, 2017

**Today's Progress**: Learnt more about HTML and CSS

**Thoughts:** Doing Freecodecamp is really nice, but I still feel like I need a project. Maybe at the end I should aim for some sort of portfolio page?

**Learnings:** HTML has two layout concepts called element, margin and padding. Element is a chunk of content - each will have its own border. Margin is the space between different elements (eg if a box (element) sits within another box (another element), the margin is the space bewteen the former's border and the latter's border). Padding is the space between the element and its own border (eg a text box with lots of padding will have a lot of space between its text (element) and its box border). 

**Tomorrow:** 
- Do some more Freecodecamp - work out a project
- Look at user input for TDD

-------------------------------
### Day 13: December 3, 2017

**Today's Progress**: Learnt about Bootstrap

**Thoughts:** Finally understand what people mean by Bootstrp. I'm a bit ill today, so only did around 45-50 mins rather than full hour.

**Learnings:**
- Bootsrap is a like a library of premade CSS classes that you can add to elements
- some of Bootsrap classes have to be added to div sections that house each element you want to apply Bootsrap to. For eg, if you want adjust relative size of an button by using the 'col-xs-4' class, the button needs to be within a div section, and the class 'col-xs-4' is applied to the div. Otherwise, othert classes like 'btn-primary' can be applied to the <button> element itself  

**Tomorrow:**
- carry on with Freecodecamp
- look at user input for TDD

-------------------------------
### Day 14-16: December 4-6, 2017

Progress**: Worked out that I definitely need help thinking about TDD and user input. Also read a solution to the Mars Rover challenge

**Thoughts:** It's nice knowing I can reach out to someone to help me code. Its especially nice knowing I have tried my best to solve it myself but recognise I need help.

**Learnings:**
- a ||= b is another way of say a = a || a = b. Eg '@variable ||= nil' is another way of saying if the @variable has been assigned a value then it equals itself, otherwise it is equal to nil
- % number is a great way to cycle through the indices of an array. Eg: if you have 3 objects in an array, then using something like '(index + 1) % 3' will cycle through them (first it will be 1 % 3 which equals 1, then 2 % 3 = 2, then 3 % 3 = 0, then 4 % 3 = 1 again. So you can cycle through the indices 1, 2, 0 forever. 

**Tomorrow:**
- work on a new project

-------------------------------
### Day 17: December 7, 2017

**Today's Progress**: made a chrome extension

**Thoughts:** making my first (tutorial) chrome extension was quite easy, but manipulating it further was quite difficult. 

**Learnings:**
- Looking at the elements that make up a Google homepage, I was able to change the background image image by adding this "style" to the body part of the HTML code:
style="background: rgb(0, 255, 255); background-image: url(https://assets.pokemon.com/assets//cms2/img/video-games/_tiles/pgl/johto-x-alola/pgl-johto-x-alola-strategy-169-en.jpg);" ETC

**Tomorrow:**
- see if I can make a [content script](https://developer.chrome.com/extensions/content_scripts#pi) that changes background image

-------------------------------
### Day 18-20: December 8-10, 2017

**Progress**: Learnt a bit about Builder pattern and exception handling in Ruby

**Thoughts:** I don't have a project to apply Builder pattern to, so it still feels abstract. However, I can apply exception handling to Mars Rover tomorrow, so should hopefully have a good grasp of it soon!

**Learnings:**
- Builder patterns are used to seperate the construction of an object from the actual object itself. For example, if I create Computer.new, I don't want to have to specify in it's inititialization to include a CPU, a mouse etc. I want the code in the Computer class to only contain code for it's behaviour, not what components it has. Therefore, I use a ComputerBuilder class to specify componenets, and then I can use the Compueter class to define behaviour.
- Exception handling: 'begin' holds the code to run. If the code produces an error,it will usually terminate the script. But 'rescue' contains code to handle the error; eg it can puts an error message, and rerun the script. 'Else' executes if there is no error, and 'ensure' runs code regardless of if there is an error or not. Exception handling is used for a part of the code that is likely to have a varied input (and therefore likely to raise an error) eg user input fields.

**Tomorrow:** Use error handling to create user input part of mars rover app. [Use bastards book of ruby](http://ruby.bastardsbook.com/chapters/exception-handling/), it's a good well-explained guide.

-------------------------------
### Day 21: December 11, 2017

**Today's Progress**: Wrote the beginnings of my user interface for mars rover tech test

**Thoughts:** Getting the 'flow' down for user input is quite simple.

**Learnings:** attr_accessor can be used without having to initialize/state any instance variables. A class with only 'attr_accessor :foo' will work, meaningyou can read and write the variable foo. 

**Tomorrow:** write error handling for user input

-------------------------------
### Day 22-24: December 12-14, 2017

Progress**: learnt about Regex and Modules

**Thoughts:** Regex is the ugliest (aesthetically speaking) part of coding ever, but it is easy-ish to pick up. I kind of understand Moules, but I have a feeling I'll only start using them/understanding them fully once I build a big application.

**Learnings:**
- Regex are great way to validate user input: you use a whole library of symbols to looks for 'patterns' in the input, which, importantly, has to be a string. An amazing resource to test out Regex code is here: https://regexr.com
- Modules are like libraries that contain methods or variables you want to use across classes. Again, this will be more pertinent for large applications. A good explanantion is [here using the instruction 'include'](http://ruby-for-beginners.rubymonstas.org/advanced/modules.html)
- if you use a module, make sure you require it (if it is a different file) or state it above the classes you want to use it in (if it is in the same file)!
- '..' refers to the parent directory of you are in, whereas '.' refers to the directory you are in. So typing ../.. refers to the parent dir of the parent dir of the dir you are in :)

-------------------------------
### Day 25: December 15, 2017

**Today's Progress**: started using TDD with Regex

**Thoughts:** I love TDD

**Learnings:** no new learnings actually. More practice of what I've just learnt (symbols in Regex, let statements in TDD)

**Tomorrow:** Finish UI for tech test using TDD/Regex

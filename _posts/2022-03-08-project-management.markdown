---
layout: post
title:  Project Management
date:   2022-03-08
image:  /coding-cat-get-back-to-work-you-piece-of-fur-there-is-no-money-from-blogging.jpeg
tags:   First Post
---



__Defining Goals & Setting up a website.__ First week at Waag and trying to figure out how to work with *<span style="color:DarkMagenta">github</span>, <span style="color:GoldenRod">jekyll</span>, <span style="color:LightSeaGreen">terminal</span> and getting familirized with some basic coding!* The goal was to create a website in order to document my journey at Fablab. I looked into what the fablab academy students are up to and followed their steps!

## Goals for this week

* Make a website and describe how you did it
* Introduce yourself

---

### Documentation Process


I started off with opening the fablab academy’s blog posts and seeing what others are up to and what steps they took so far. With the help of the other inter, we managed to look into a few things. First step was choosing a static site generator, as there are way too many options. I chose Jekyll since, according to this youtube video <https://www.youtube.com/watch?v=c9g4UkHkzLs>, it has been around for quiet sometime and has gained a lot of popularity, which thanks to the big community established, it makes it easier to find tutorials and answers quickly. Most importantly, it’s a default static generator that runs github websites and uses ruby.

I had to also familiarized myself with a lot of new terminology since I had no prior experience to jekyll, what ruby or homebrew meant, following this tutorial <https://www.youtube.com/watch?v=UKB9ylw0G4U> it helped me gain some basic idea and enabled me to accomplish the first part of the assiment - installing jekyll.

---

#### Jekyll Installation


1. Make sure your Macbook is up to date, M1, macOS Monterey or higher

- Side note: When updating, sometimes it takes too long when its 1 minute remaining, if it is the case, make sure that no external devices are connected. i.e. hard drive or a USB device. Also, make sure you have enough space on your computer. other than that just be patient and it will work!

2. On the top, press Go — Utilities — Open terminal.

3. Right click on the icon of terminal and press options — keep in dock since you will be using it a lot.



![]({{ site.baseurl }}/images/week_1.png)
*Visual Studios*

#### HomeBrew Installation

5. Go to <https://brew.sh/> and click on the icon next to the code to copy it

6. Go back to terminal and paste, enter to install

7. After installing 2 command lines should appear under the test that reads: the Next Steps. (yet in my case they did not), I nevertheless wrote the lines and entered :

![]({{ site.baseurl }}/images/code-1.png)

8. press enter, if everything is working properly you won’t get any error messages. 

9. second line: 

![]({{ site.baseurl }}/images/code_2.png)

#### Install Ruby

12.   Type code 

![]({{ site.baseurl }}/images/code_3.png)

*Side note: SDK stands for Software Development Kit*
The command is used to make sure that any jekyll component that use ruby do not fail
macOS comes with a pre-installed version of Ruby

(very important, that the Xcode command will be installed)
*what is Xcode? tools needed to create an app… project management tools + solve problems
IDE - integrated development environment *

13. Type code 

![]({{ site.baseurl }}/images/code_4.png)

14. Copy 

![]({{ site.baseurl }}/images/code_5.png)

*why do we do that? so that when we run jekyll, it will first look for what is in its path and its going to look for the first one which in default mode is the macOS one yet we want it to find the ruby 3.0*

15. Seeing no error is a good sign, type clear and enter

16. Type

![]({{ site.baseurl }}/images/code_6.png) 

17. quit terminal and come back in and check that ruby 3.0 is now the version running!

#### Install Bundler & Jekyll

#### Hosting on Github Pages

Some intro on what git is
<https://www.youtube.com/watch?v=USjZcfj8yxE>

I followed this tutorial 
<https://www.youtube.com/watch?v=fqFjuX4VZmU>









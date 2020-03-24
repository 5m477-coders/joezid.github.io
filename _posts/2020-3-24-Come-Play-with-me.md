---
layout: post
title: Come Play with me
categories: [CTF-Writeups]
tags: [Reverse Engineering,Competitions,CyberTalents]
description: Writeup for Come Play with me challenge from CyberTalents.
---
# Challenge name
Come Play with me
# Category
Malware Reverse Engineering
# Level
Hard
# Points
200
# Description
This strange game can give you the flag, will you play ?
# Solution

![Image](https://raw.githubusercontent.com/joezid/joezid.github.io/master/Images/comeplaywithme/1.png)

As we can see we are given x64 elf file ,so let's run the executable and see what it does.

![Image](https://raw.githubusercontent.com/joezid/joezid.github.io/master/Images/comeplaywithme/2.png)

As we can see there is an error due to wrong key legnth ,so it's clear now that we are working with a frozen python executable.
Our goal now is to retrive the source code of the executable first thing we have to do is installing the pyinstaller library.

{% highlight yaml %}
pip3 install pyinstaller
{% endhighlight %}




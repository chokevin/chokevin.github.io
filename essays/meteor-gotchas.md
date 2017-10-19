---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-10-19
labels:
  - Software Engineering
  - Meteor
---

<img class="ui small right floated spaced image" src="../images/meteor.jpg">


Frameworks can be the worst. Every framework comes with heaps of praise and hundreds of webpages full of documentation, yet the simple beginner user struggles to load content with the tutorial. Programmers for the past decades have looked to find newer ways to get up to speed quicker. How to get things done quicker without sacrificing the flexibility and feature-richness of more "complicated" frameworks.

As I browsed Reddit, I came across a very suitable question for software engineering as a whole. The user said that in an interview the following question was asked:

<blockquote> "Is programming an art or a science?" </blockquote>

The response the user said received high praise which I also agree with.

<blockquote>"Programming is a craft." </blockquote>

A craft where the programmer spends countless amounts of hours refining. The types of programs start out tutorial-like and basic, yet over time become beautiful masterpieces. Much like a sculptor achieving his "David".

Such is Meteor. Over the past few days I had encountered numerous problems that made me question the existence of the Meteor framework. One of those problems I outline below.

<h3> Unable to load add-content, edit-content, and homepage simultaneously </h3>

<img class="ui small floated spaced image" src="https://imgs.xkcd.com/comics/fixing_problems.png">

Many users may not have encountered this problem if they blindly followed the tutorial. I certainly am not that type of person. As such when the tutorial mentioned to delete certain javascript files attached to my add-content page I readily ignored it. Why would javascript attached to my file cause any issues with loading pages? Especially if it's javascript that pertained to the template file. I was completely wrong. I spent the whole afternoon trying to find pieces of code that may have potentially been causing the error. Changing syntax, moving lines of code around, deleting lines of code, until I finally decided to delete the syntax in the javascript file.

<h3> BOOM. Everything Loaded </h3>

What a struggle of an afternoon. Except now I have faced one struggle that I shouldn't face again. Except that was not the end of my problems.

<h3> Initializing IntellijIDEA and new Meteor Applications </h3>

I understand that for most users they may only build one Meteor application every few months. To the average user they would begin one meteor application and develop on it for multiple hours until achieving a nice web application. Except in my case I have been building new meteor applications for tutorials for the past few weeks. Each time I start up an instance of meteor and load the files into Intellij takes about five minutes. When dealing with time sensitive trials, such as the ones I deal with in my software engineering class, I found myself doing edits in vim and finishing the code before my Intellij finished indexing my files. I have yet to solve this issue, but I find myself wondering if it is worth fixing this issue. It will be soon that I dedicate the last few weeks of school to implementing a large-scale Meteor application where it will only need one initialization. For now I will struggle on.

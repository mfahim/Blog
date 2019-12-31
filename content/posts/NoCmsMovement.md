+++
date = "2015-01-26"
Title = "No CMS Movement"
Description = "No CMS Movement, the return of static site generators."
Keywords = ["Development", "Hugo", "Personal"]
Section = "post"
Slug = "No CMS Movement"
Tags = ["Go", "Hugo", "No CMS", "Static Blogging Engine", "GitHub", "Windows"]

+++

#### Welcome to my first post! ####

Yeah! This post is a static HTML page, No dynamic partial fragments, no connection to database, no charges from any CMS website or 3rd party. Unbelievable, isn't it? 

It's a page written in MarkDown and deployed on GitHub.
Internet and its evolving nature pushed us one more time to a correct direction. 
Obviously, all static pages are faster, less expensive and more straightforward to maintain.<!--more-->   


Personally, after some years of developing server-side page applications, I was intrigued by the concept of static blogging engine. Technically, most of the well-known ones turn a pile of templates, content, and resources (like CSS and images) into a neat stack of plain HTML. You run it on your local computer, and it generates a directory of web files that you can upload to your web server, or serve directly.

Basic Concept
------------------------------------
The idea is that you don't need a big server-side engine like IIS, PHP, etc. to generate every page, every visit, for every visitor. You can generate the entire site once ahead of time, and only regenerate things when something has changed, e.g. with a post-commit hook on a Git repository containing your content or layout.


One of the clear benefits of this approach is caching without any complex mechanism. Web servers are built to quickly cache static content. All images, styles, javascript libraries could be cached on browsers as well.

How the new wave has been started?
------------------------------------
  
I believe, It's around the key question of whether we really need real-time contents. Many bloggers/publishers have ultimately admitted that not everything needs to be “real time,” and that most users, in most scenarios, don’t experience a noticeable difference between real time and near real time.

Big players in the market
-------------------------

Actually, there are many. Every technology/programming languages build a blogging platform for its users.
  
 1. [Jekyll](http://jekyllrb.com/): probably the most popular one. It's a Ruby based engine and features tight integration with GitHub.
    
 
  * [OctoPress](http://octopress.org/) is based on Jekyll and makes it easier to get started by adding default templates and various other tweaks.

 1. [Pelican](http://docs.getpelican.com): a python based blogging engine and has most of the features you'd expect. It uses Dropbox as uploading system.
  
 2. [Ghost](https://ghost.org/): The brainchild of one the heads of WordPress team that focuses on writing and publishing. Simply a Node.js app built upon the Express framework.
 3. [Scriptogr.am](http://scriptogr.am/): A tool for generating simple, elegant, static weblogs by reading Markdown files stored in your Dropbox folder.
 
 4. [Dropplets](http://dropplets.com/) : is a minimalist Markdown blogging platform focused on delivering based on PHP.
    
 4. [Hugo](http://gohugo.io/): A fast and flexible blogging engine that works in many formats. It's written in Go language.     
  

In my next posts, I'll elaborate on the new wave of content management via static pages via Hugo.

Happy Static Blogging!
 
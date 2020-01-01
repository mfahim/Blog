+++
title = "About Visual Studio 2015"
date = "2015-07-01"
description = "About Visual Studio 2015."
keywords = ["Development", "Visual Studio", "Asp.net"] 
section = "post"
slug = "About Visual Studio 2015"
tags = ["Visual Studio 2015", "Asp.net"]
+++

 
I don't know how long you've been on the Visual Studio train, but my personal experience started when Visual C++ 6.0 was the only game in the town. MFC and ATL were the major solid libraries that most developers relied on. However, my primary focus of this post is more about the evolution of Visual Studio.Net since 2002. <!--more-->So, scanning my mind quickly, here's the list of things that I can outline:
   
  - VS 2002 - .Net 1.0 - WebFoms/WebService
  - VS 2003 - .Net 1.1 - Bug fixing/Compact Frameworks
  - VS 2005 - .Net 2.0 - Asp.net 2.0/ Local IIS
  - VS 2008 - .Net 3.5 - Linq/MVC/Some Testing tools/ TFS
  - VS 2010 - .Net 4.0 - MVC 3/ Test Manager
  - VS 2012 - .Net 4.5 - MVC4 / Nuget/ Metro UI/ WebEssentials/
  - VS 2013 - .Net 4.5.1 - MVC5 / WebAPI/ Git Support/TypeScript/Bootstrap/Code Map/Browser Link 
  
Looking back on it, we'll see more of these changes towards better team management and quality of production code and more Agile-friendly in one word.
However, Visual Studio 2015 is supposed to be a different environment for all MS developers. Specially on the web application front, many changes have been made to persue them into new generations of web apps.


Visual Studio 2015 has some tentacles, I'll write about them in brief.

1. VS 2015 online(Monaco): is the online editing tool for Azure websites. It's great for cross-platform development, CI (builds & integrations) and hook to other online services. e.g. Github, Jenkins, Trello, Bamboo,..!
 
2. VS 2015: The most important one is all menu items are not in caps anymore! The new changes cover some areas that I put them under these categories: 
	 
  1. Compiler (Roslyn)

  2. Portable Class Libraries (Native & Hybrid apps)

  3. Asp.net VNext

  4. Owin
	 

    **Compiler (Roslyn):**

    In short Roslyn is compiler as services via api. One of the good things about Roslyn is Out of the box Parser & Lexer. It allows you to do code-fixes, even you can see what’s going to compile by Roslyn Syntax visualizer. However, HTML & typescript are not not supported in the current version.

    So, in visual studio the impact is lead into a great one which is by saving a file the whole project built. (Dynamic Compilation)
    The sad point about that is the Resharper. They have developed their own parsers and based on the news, they're not going to change it to adapt with Roslyn. You can do refactoring either by Roslyn or Resharper.
    Roslyn Refrences:   

     - Matt Warren Roslyn performance lessons: 
	  - [Roslyn code-base performance lessons-1](http://mattwarren.org/2014/06/05/roslyn-code-base-performance-lessons-part-1/) 
  	  - [Roslyn code-base performance lessons-2](http://mattwarren.org/2014/06/10/roslyn-code-base-performance-lessons-part-2/) 
	
     - Roslyn official website: [Some samples and wlakthroughs](https://github.com/dotnet/roslyn/wiki/Samples-and-Walkthroughs) 

    **Portable Class Libraries:**

    This is the one that makes everybody excited about Visual studio being cross-platform. By that we can create cross-platform apps and libraries.
    The obvious benefit is writting native applications for mobile and share 75% of your code. 

    The whole ideas is reuse your code as much as you can and put them under 'Shared' project(PCL) and having different projects for different platforms. VS 2015 provides some options to design your form based on different size and also Xamarin Forms could be another candidate. Debugging and Testing on emulators are some plus features for devs.

    On the other side, VS provides good tooling with Hybrid mindset. 'Apache Cordova' is included into product and with support for native device capabilities (e.g. camera, accelerometer, contact), offline scenarios and popular JavaScript frameworks (e.g. Angular, React and Backbone), the Tools for Apache Cordova contain everything web developers need for building cross-platform mobile apps using Visual Studio.Don't worry about the challenges from Cordova UI: 'Ionic' and 'Onsen UI' are helpful libraries to come over some known issues from different devices.

    **Asp.net VNext**

    Finally, npm, bower, and grunt/gulp an dbower inetrgate nicely in VS 2015. So, client-side compilation can be done on the client by the client tools. All package management and bundling, minification and... by js files. To be short here's the list of changes:   

    no more web.config, .csproj. (project.json(nuget), config.json(web.config), package.json(npm), bower.json(front-end package mngr), gruntfile.json(process your js/css files)
    - wwwroot for static file (content)
    - WebApi & Controllers are in one.
    - Angularjs templates
 

    **Owin**

    To my undesrtanding, Owin is making asp.net mvc to be launched on Linux, Osx. Owin in VS 2015 has addressed one the biggest problems of Asp.net. Which is being slow. All of the Asp.net competitors like PHP load time are a lot faster and that was because in Asp.net all modules including the resudant ones need to be loaded in the first place. 

    The real beauty of OWIN is that it gives you direct access to the ASP.NET pipeline in a relatively friction-free way. This is a great place to deal with cross-cutting concerns such as logging and authentication. Dependency injection is now also an integral part of OWIN and can be used to inject services into your middleware.

    By using appbuilder (single interface) to register any middleware component that handle the web request ( SignalR, webapi, asp.net identity) 
    Overally, your Http pipeline is optimised in what you need. 

 
- Startup.cs -> define what services needs to be added (EF, MVC, routes, features, auth)
- Owin means asp.net mvc running on Linux, Osx
- Owin :  

- Asp.net KRE, KVM, KPM -> cmd -> (install K)K Runtime env, K version mngr(install KRE), K Package mngr(run app)


- Microsoft Built-in dependency injection. So, no Autofac, Structremap, Ninject, You can use dependency injection in Razor page, too!

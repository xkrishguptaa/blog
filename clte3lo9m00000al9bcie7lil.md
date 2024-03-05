---
title: "3 Actually "Unique" Project Ideas + Execution That Will Get You the Job"
datePublished: Tue Mar 05 2024 08:18:30 GMT+0000 (Coordinated Universal Time)
cuid: clte3lo9m00000al9bcie7lil
slug: 3-actually-unique-project-ideas-execution-that-will-get-you-the-job
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1709626575446/f0d89628-6a9c-462a-a294-0208e599a408.jpeg
tags: programming-blogs, development, projects, webdev, developer

---

## Introduction

So you're James, walking into an interview with 12 different full-stack projects. You built a to-do app, a chat app, and a movie rating app. Most people have built those sorts of things 🤷🏻‍♂️. If you have a lot of product clones, like an Amazon clone or a Netflix clone, several people have already built them.

The worst part is the interviewer probably already knows what a to-do app or an Amazon clone is. That doesn't strike quite the conversation. Unique "project ideas" can be showcased in an interview much better.

Here are 20 problems I face in real life that do not have any solutions yet (trust me, I scoured all of Reddit.).

## 1\. IRC Client

The most popular IRC client, HexChat, looks like this:

![hexchat screenshot](https://hexchat.github.io/img/thumb.png align="center")

I get that the IRC nerds would love it. However, this creates a barrier for those who might wanna chat with people but don't want an app that looks like it was made for Windows XP.

On top of that, this app, which is supposedly the "best" one, isn't even available on Macs. 🤡

After many sleepless nights, I found Halloy, an IRC application written in Rust. This solves the problem to a minuscule extent, as this is also designed for the IRC gurus. The only GUI it has is looking at the chat and sending messages. To configure it, you add all the options in a configuration file. So, it is still not user-friendly for those who aren't good with IRC.

![halloy](https://github.com/squidowl/halloy/raw/main/assets/animation.gif align="left")

I think you might have caught on till now. The idea is to build an IRC client.

* If you're a web developer, Choose either [Electron](https://www.electronjs.org) or [Tauri](https://tauri.app). They allow you to build desktop applications using web technologies like HTML, CSS, or JavaScript.
    
* If you're not a web developer, build it in any programming language that can output desktop applications.
    
* You can read the source code of [Halloy](https://github.com/squidowl/halloy) to figure out how to process IRC streams.
    
* Use a UI library if you're not that good with design. Otherwise, design and build a UI to work with the IRC.
    

## 2\. Email To-do

I know that to-do apps are LAME, but hear me out. A lot of people use email as a to-do application. CEOs and CXOs generally do that, basically busy rich people.

Busy rich people are probably the best customers for any product. After looking through ProductHunt, I found Spark Mail. It is what I described. Now, why do I not use it? Because It doesn't support anything other than Gmail. I use iCloud Mail, so I can't use it, and that sucks.

![Smart. Focused. Email.](https://cdn-rdstaticassets.readdle.com/spark/img/spark3/index/banner-device.png?1661256907 align="left")

I tried using Apple Mail and the archive folder. Wherein I would archive emails after I'm done, but threads in Apple Mail and absolute dogshit.

Now, how do I make this?

* Figure out SMTP and other email protocols (I'm sure there is good documentation on these)
    
* Build a UI for a decent Email Application.
    
* Finally, add a "done" button to emails that put them in the archive.
    
* Bonus: You could experiment and add stuff like Kanban boards or things that to-do apps have!
    

## 3\. Manga-Reader

A lot of people read the manga. Manga is comics but for Anime instead of superheroes. There is this really cool website, called MangaDex which allows you to read manga.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1709624882679/a0797fb7-e860-4da6-8249-881d94431eea.png align="center")

However, they do not have an offline app, so you need internet to access this library of manga. When people are travelling or do not have internet, they generally like to read stuff or watching downloaded videos. If there was an offline app to download and read mangas, it would be awesome!

Building it:

* Choose a tech stack. Recommended: Native Language for the platform.
    
* Mangadex has a very slick API, that you can use to download mangas: [https://api.mangadex.org/docs/](https://api.mangadex.org/docs/)
    
* Have a way to store the manga on the system, put the location and the manga details in a local database and voila! You have it!
    

## Tips

* Build In Public. This small project of yours could turn into a startup with several users. (in case it does, I don't want 5% of equity, your soul will suffice my hunger 😜). This was the case with SuperHuman (an email app).
    
* Document your journey, write a journal or something like that, trust me it's helpful because you will forget stuff later on.
    
* Launch on Product Hunt! It brings great traffic to your project and feel free to even ping me about it, I would love to support your launch on Product Hunt.
    

Feel free to follow me on [Twitter](https://twitter.com/xkrishguptaa) and until the next time 🚀  
  
Edit: the soul was delicious, thank you 😋

![I'm different...like everyone else | I'M NOT LIKE THE OTHERS...I'M UNIQUE: | image tagged in class of females,class,unique,different,memes | made w/ Imgflip meme maker](https://i.imgflip.com/5uob45.jpg align="left")
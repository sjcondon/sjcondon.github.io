---
layout: post
title:      "Rails Project- Coding Journey"
date:       2020-06-17 16:05:16 +0000
permalink:  rails_project-_coding_journey
---


My coding journey for this project was a rough ride. I knew that I wanted to create a *todo project* since I tend to create a lot of check lists for myself but when a project is created from scratch it is tough to know where to start. 

I watched about 8 different videos that Avi created to get my project up and running but the biggest mistake was that I wanted to challenge myself and used *scaffold* (I didn't fully read the directions saying **DO NOT USE SCAFFOLDING**) Yes, I am **now** aware that it was not good practice and it created the front end and back end needed for CRUD. This was my first mistake since it made my project hard to manage and I was not *scrappy*. This was a learning experience and now I know why you should not use scaffold. I feel like I set myself up to fail right away.

Rails generate was a neat tool that I used for my controller and models. For my project I made the names a bit confusing, *todo list* and *todo items*. I learned that I need to simplify and maybe just have* list* and *items*. In my mind, I always had to remember what each did. "Were the list in items or the items in the list". Then I had to think about my own check list. I have a list of many items. This is where the models were helpful *has_many* and *belongs_to*. The confusing part was where do I put *has_many :through*. I had to be creative with where I put this and after talking to a few other instructors, I was able to figure it out. It was a requirement to put it in two places but I could only think of one. Once I created a *belongs_to :creator*, I was able to have another 'has_many :through". 

Validator - I understood what needed to be done because I did this in Sinatra, but in Rails it was a bit different. Rails, I used render :new  to help assist the validations and another new thing was *flash[:{blank}]*. From Avi's videos, I had a high level uderstanding of what needed to be done, but didn't fully understand how it should be done. Everytime I tried to implement this, I would get an error and once I got help, it was and easy fix which was extremely frustrating. 

Scope Method- I only used this once and I used it in my models *todo list*. This scope method allows the list to be ordered alphabetically and the *todo list controller* index allows the logic to happen and have the todo list to be orderd by the title. 

I think the **easist** part of the project was creating a *login*, *logout*, *signup* and *password* creation. For the emails,  I created validations which allows each email to be *unique* and no duplicates. A new thing  was to use *user.password = SecureRandom.hex* this allowed the password to be secure. SecureRandom is a number generator interface which fill generate session keys in HTTP cookies so that a random hacker cannot get your actual password. I think that is **super** neat. 

Login in via github - This was something that I learned through Avi's video, but I wasn't able to do it exactly what he did. I was super proud of myself once this was created. It was tough and a bit confusing. 

Nested routes - I nested my todo items into my todo list. I did this through my routes (*line 4 allows this to happen*). When I did my project I knew that I created a nested route in my project because I could see it on my server, but it was hard for me to wrap my head around it. I do have a better understanding of it today, but it is still somewhat tough. 

**DRY**- This is something that I always had to be aware of and I did  the best I could do. 


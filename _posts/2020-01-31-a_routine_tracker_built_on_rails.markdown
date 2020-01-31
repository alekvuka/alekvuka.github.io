---
layout: post
title:      "a routine tracker built on rails!"
date:       2020-01-31 17:00:21 +0000
permalink:  a_routine_tracker_built_on_rails
---


I must confess, I sometimes struggle to remember all the routines I’ve set for myself. Usually these routines contain multiple tasks and are usually grouped by time of day — morning, evening, etc.

So, for my first Rails project, I thought it would be awesome to create a custom web app that enables me and my friends to create and share routines!

First, I thought about how the models for such an app would be structured. I decided that the app can do with five models — user, routine, task, task_routine and user_routine.

A user has_many user_routines and has_many tasks, through user_routines. Likewise a routine has_many user_routines and has_many task_routines and thus has_many tasks through task_routines and has_many users through user_routines.

After setting up the models I started thinking about controllers and views. My sessions controller takes care of sign-in and logging out the user. I also created a controller for users, routines and tasks. In my views, I created corresponding files that would show the individual instance as well as enable the user to edit it and see other instances within that model.

My previous project was built using Sinatra, and working with Rails was definitely a joy. I really really really like Rails and recommend it to anyone looking to create their own web app. Rails smartly uses standardization to save you a lot of work. ActiveRecord is indispensable, in particular if you are quarrying the database. Using Active Record Query Interface instead of SQL is like trying to walk vs drive to a destination. With Rails you will get there quicker and be a lot less tired.

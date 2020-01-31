---
layout: post
title:      "Building JS"
date:       2020-01-31 17:05:38 +0000
permalink:  building_js
---


A few months ago, I built a routine tracker app entirely in Rails! I love working with Rails but its rendering of views and use or erb can be quite limiting. So as a challenge, I wanted to build a front end entirely in JavaScript and just use the Rails app as a back end API.

I first changed the routing and controller methods in the Rails app so that information for a user and/or a routine can accessed through an API in a JSON format. Next, the only two views which will load are login/signup page and (after signup/login) and user show page. The user show page has three <div>s, which I used to construct the page via Javascript.

Next I created the relevant js files in my javascripts assets folder. One file, routine.js, was responsible for the code that would create a view of all the user’s routines. Another file, user.js, was responsible for building the elements and content necessary to display information about the user.

Thus, the user could create a routine, see all of their routines, delete a routine and see their current and upcoming routines all without ever reloading a page!

---
layout: post
title:      "another look at sinatra "
date:       2020-01-31 17:30:40 +0000
permalink:  another_look_at_sinatra
---

My neighborhood has an impromptu book sharing program - many public and private places contain bookshelves where people put books which they would like to share with the community! People then choose which book from the shared collection they would like to take and read.

Its a very cool cool community resource and I though that a process which would keep track of who has read which books and which books belong to whom would enhance our community book share. I though that such tool would be best if it was web based and easily accessible to all, thus I decided to use this project as an opportunity to learn and build a Sinatra application.

As I built this application, I really got to appreciate a few tools and functionalities. First, rack and shotgun where indispensable. I used rack for my database migrations which included setting up :has_many and :belongs_to and :has_many_through relationships between the models.

Shotgun was incredibly useful as well, in particular for debugging. In many cases, the bug was an obscure syntax error that would be extremely painful to find without shotgun.

The models I created for this application where User, Book and Neighborhood. A User :belongs_to a Neighborhood and a Neighborhood :has_many Users. A book :belongs_to a user and :belongs_to a neighborhood through Users.
The application has a few cool features, including the ability to contact the book’s owner and for the owner to note what the book was about and jot down their impression of the book. The community can also rate the book.

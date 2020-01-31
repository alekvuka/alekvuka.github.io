---
layout: post
title:      "Cameras and Traffic in NYC"
date:       2020-01-31 17:27:32 +0000
permalink:  cameras_and_traffic_in_nyc
---

I live in NYC and, yes, I drive in NYC. I drive a lot actually. I logged~60,000 miles in the last 3 years just within the 5 boroughs. And I can tell you: google maps and waze are terrible at predicting traffic in the city. For a while I wondered if there was a way to better to determine traffic conditions and it finally struck me that there are an enormous number of camera in NYC. At least some could be used for predicting traffic!

In fact, NYC’s Department of Transportation maintains and broadcasts feeds from a ton of cameras. Which was super exciting! What was not exciting is the user interface on their site. It was difficult to select cameras and view them in a user friendly manner. So I decided to build a more user friendly interface using react as a front end and rails as a back end.

Components are a big part of what makes React awesome, and this project lent itself well to presentational/container components. I created two containers: Header and Camera. The header container deploys the presentational containers for creating buttons and nav links. The buttons and nav links are determined by the Rails back end.
The camera container is responsible for rendering camera presentational components. This includes the rendering the image and the description of that particular camera.

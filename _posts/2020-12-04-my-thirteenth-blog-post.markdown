---
layout: default
title: Blog 12
date: '2020-12-04 11:30:00 -0700'
categories: blog update
published: true
---
<h1>Creating a CSUN Map Quiz</h1>
<p>For my CIT 384 class, Web Development and Hosting, we were assigned to code a CSUN Map quiz which consists of the user being presented with a map of campus (using Google Maps) and a set of locations. The user then has to click on the map where they think the location is. A requirement for this assignemnt was that if the user clicked on the correct location, a green rectangle would be drawn on that spot, and if they were wrong a red rectangle would be drawn on the correct spot.</p>

<p>The first step was to go the Google Developers website so I could get access to the Google Maps API. The process was pretty simple; once on the right page you just select which product you want to use, in my case its Google Maps Javascript, then you set up a billing account because this is a paid service if you plan on using it commercially, finally you are given an API key which can be used in Javascript to import a working Google Map. One issue I had though, the billing account I setup was not associated with my API key I was given, so everytime I tried to import the map, I was given an error. The error luckily gives you a link to go to so you can fix the issue. Once I had successfully imported a working Google Map, I had to now start working on the quiz itself.</p>

<p>Making the layout and design of the page was easy enough using HTML and CSS since I had to do this for multiple other projects in this class, so what I really had to focus on was the Javascript code to create the logic for the quiz. The first thing I had to do was the get the coordinates for every location I needed. Google Maps Javascript has a command where, if given a north, south, east, and west point, can draw a rectangle on that spot. I made a function that whenever it's ran, will check if whether or not the user pointed at the location being asked about, and if yes then will draw the green rectangle, or if not the red rectangle. The function can also tell when the game is over and pop a goodbye message that says "Thanks for playing!". The user can now refresh the page to play again if they want. With this all of the requirements for the assignmnent were met.</p>
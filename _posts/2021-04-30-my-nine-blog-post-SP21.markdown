---
layout: default
title: Blog 9 SP21
date: '2021-04-30 16:30:00 -0700'
categories: blog update
published: true
---
<h1>General Methods of Speeding up a PC</h1>
<p>A relative of mine visited me a few days ago and asked if me if I could take a look at his PC. He built it himself less than a year ago but it apparently was already feeling sluggish whether he was playing games or just browsing the internet. After some benchmarking and stress test software, I didn't see any issues hardware wise like crashing or overheating, but I did notice the tests would stutter and drop frames.</p>

<p>Over the years of dealing with PCs and all of their issues, I've gotten used to what could be causing those issues and checking for them. If you've ever had similar issues such as sluggishness or slowdowns these would be the steps I would recommend taking. He had an NVIDIA graphics card so the first thing I did is update the graphics card drivers using the NVIDA GeForce Experience software. An out of date driver could be the culprit but after some further testing it turned out not to be the case. Next is updating the BIOS of your motherboard. This is something that is often overlooked by casual PC users, but even after updating it there was no change.</p>

<p>By default on Windows 10, there is a feature called "Windows Game Mode" that is on by default on a fresh installation. This does more harm than good for gaming performance so I made sure to disable that as well. Similar to that feature, NVIDIA graphics cards are able to have your gameplay recorded on its own and create highlights for you automatically using the GeForce Experience software. Disabling this could also bump up performance for gaming. When these steps didn't work I decided to check his Windows Power Plan. The different power plans enable or disable certain performance enhancement settings, where balanced is usually the default. When I checked his power plan it was set to power saver, making it so that his CPU and GPU were being throttled to save energy. Once I set the power plan back to balanced the slowdowns were completely gone.</p>
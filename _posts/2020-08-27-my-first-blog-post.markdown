---
layout: default
title: Blog 0
date: '2020-09-04 11:38:00 -0700'
categories: blog update
published: true
---
<h1>Jekyll on Windows</h1>
<p>When I reserched Jekyll I saw that it was only <i>really</i> supported by macOS and Linux. Because I have a Windows 10 PC I saw that my options were to use RubyInstaller to install Ruby along with a DevKit, or enabling Linux Bash on Windows. I thought using Linux on windows was a more interesting route so I went with that.</p>

<p>Thankfully with recent updates to Windows 10 you can actually enable a couple features to use Linux, those features being &quot;Virtual Machine Platform&quot; and &quot;Windows Subsystem for Linux&quot;. After those were enabled I was able to install Ubuntu terminal from the Windows Store. From there I was able to install Ruby, and from there install Jekyll.Once I confirmed Jekyll was correctly installed on my Ubuntu system, I followed a very straightforward video tutorial series on getting a blog up and running on GitHub with no issues.</p>

<p>I ended creating an issue when I decided to change the theme of my blog using the GitHub Pages built-in theme changer. The issue I had was my blog was now a blank screen. Through research I ended up finding out that the theme I chose had a different scheme for the layout, so I had to make a new layout folder and combine the layout files of the new theme, and the original minima theme. Once that was the done my blog was up and running with a new theme.</p>
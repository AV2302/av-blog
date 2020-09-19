---
layout: default
title: Blog 2
date: '2020-09-18 19:30:00 -0700'
categories: blog update
published: true
---
<h1>Kali Linux and the endless issues</h1>
<p>For my CIT 425 lab assignment I wrote about in my last blog, I had the displeasure of using Kali Linux to complete the tasks. The first issue I ran into was whenever I tried to use the web browser, Kali would freeze and then log me out, closing any open application in the process. This kept happening repeatedly so I tried installing a different browser hoping it was just Firefox being the issue.</p>

<p>I attempted to install Chromium but when I ran the command the response I got back was “unable to locate package”. This happened whenever I tried to install any application. After some research I found out that the sources list in Kali is empty. After manually adding the official Kali repository link in the sources file I fixed the issue of the package not being found but then then the console was saying that the repository I added was not signed so installing the repository couldn’t be done. </p>

<p>After some more research it turns out something called a gpg key needed to be added from a keyserver and only then was I able to install new applications. Unfortunately using a new browser did not fix the issue so I uninstalled the version of Kali I was using, which came from an ISO file, and installed a new version that was made specifically for VirtualBox. This was different than an ISO file because I didn’t have to run an installer to setup Kali, the VirtualBox image file came preconfigured and worked immediately when I ran the VM. Once I was on the new version, I was then able to use the web browser without Kali signing me out every couple minutes and finally move on to work on the rest of the lab.</p>
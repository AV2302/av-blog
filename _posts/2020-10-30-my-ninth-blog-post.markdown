---
layout: default
title: Blog 8
date: '2020-10-30 14:30:00 -0700'
categories: blog update
published: true
---
<h1>Installing Security Onion</h1>
<p>For this week's assignment in my CIT 425 class, I was assigned to install a virtual machine of Security Onion, which is a special Linux distribution that is specialized in intrusion detection. I created a virtual machine for it in Virtual Box using the recommended settings. When it boots up, it goes straight to the desktop because Linux distros based on Ubuntu are live, meaning it is usable without having to install anything. But there is an executable file on the desktop to install the full version.</p>

<p>My first task for the homework assignmnet was to run that installer, but unfortunately I ran into numerous errors. One of them was that Security Onion was constantly freezing. I had to restart the entire virtual machine a number of times. Another error occuring was freezes happening, but when it unfroze I would get sent back to the login screen. This was an issue because I did not have a login for Security Onion, as it was set to login automatically when launching so I had no way of logging back in.</p>

<p>Just as I thought I was going to be able to successfully finish running the installer, I received a fatal error that would send me back to the desktop. Upon further research I found out that Ubuntu on Virtual Box has issues running when hyper-v, which is Microsoft's hardware virtualization software. This software is needed for my other virtual machines such as Docker so I wanted to leave that enabled. I then installed a free version of VMWare's virtual machine software which has better compatibility with hyper-v. Once I ran Security Onion on VMWare I was able to successfully run the installer and download all of the updates.</p>
---
layout: default
title: Blog 11
date: '2020-11-20 11:30:00 -0700'
categories: blog update
published: true
---
<h1>Testing the network utility Netcat</h1>
<p>This week in my CIT 425 class, we were assigned to run two Ubuntu virtual machines and use Netcat to have them interact. I used VirtualBox to make both machines with one user named Alice and the other named Bob. After finishing the installation of both machines I made sure to update my package manager so I can install netcat.</p>

<p>I used to the command <code>apt-get install netcat</code> but doing it this way installs the default version of Netcat which is missing some commands I need for this assignment. Using the command <code>sudo update-alternatives --config nc</code> I was able to change Netcat to use traditional settings, which includes the -e and -c switches that are required for the assignmnet.</p>

<p>To make sure both machines were visible to each other, I changed the network adapter on VirtualBox to host-only adapter. I made a file on Alice's machine named payload.txt and then ran the command <code>nc –nlvp 4444 > fromAlice.txt</code> on Bob's machine. This is a Netcat command to make Bob's machine listen on port 4444 and await a file that will be named Alice.txt. On Alice's machine I ran the command <code>nc -nv ip.addr.of.bob 4444 < payload.txt</code> which makes Alice's machine connect to a machine listening on port 4444 and send the file payload.txt. After running this the file fromAlice.txt is created on Bob's machine and contains the contents of payload.txt.
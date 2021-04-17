---
layout: default
title: Blog 7 SP21
date: '2021-04-16 16:30:00 -0700'
categories: blog update
published: true
---
<h1>CPU Bottleneck</h1>
<p>This week I had a friend bring me his PC to help troubleshoot it. He explained that whenever he was playing games the FPS (frames per second) would drop dramatically. This was strange because he recently upgraded his graphics card and it was significantly better than his old one. I never asked which CPU he had so when I opened task manager to find out, I saw that it was an AMD FX-8350, which is a CPU released in 2012. He tried to pair a 9 year old CPU with a newly released Nvidia RTX 3070 which caused a bottleneck.</p>

<p>A bottleneck, in particular a CPU bottleneck, is when there is an imbalance between the CPU and graphics card, where the CPU is unable to send enough data for the graphics card to process. To an average person, a graphics card is seemingly entirely what determines if a game runs smoothly enough, but the CPU and even RAM are what the generates and prepares frames (or data) for the graphics card to process. A weak CPU that can't prepare a high number of frames paired with a powerful graphics card that can potentially process hundreds of frames is where the bottleneck happens.</p>

<p>I referred to my friend to a website called www.wepc.com and on that website there is a tool that can help you check if a CPU is a potential bottleneck for a graphics card. <img src="https://i.imgur.com/egFF48S.png" width="650" height="300"> <br> This image shows the tool comparing the AMD FX-8350 with an Nvidia RTX 3070. Even on 1080p resolution, which is the resolution most gamers use, there is almost a 53% bottleneck happening. This tool is also useful because it suggests what CPU upgrade you should make, or what graphics card downgrade you should make if you want to keep your current CPU.</p>
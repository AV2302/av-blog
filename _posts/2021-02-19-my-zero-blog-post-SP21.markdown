---
layout: default
title: Blog 0 SP21
date: '2021-02-19 16:30:00 -0700'
categories: blog update
published: true
---
<h1>Solid State Drive Troubleshooting</h1>
<p>A few years ago I purchased a 1 Terabyte SATA III SSD, mainly for storing my video games because SSD's greatly improve load times compared to a conventional spinning disk drive. Just a few days ago I noticed a strange issue with the SSD where, according to task manager, had 100% usage even though there were seemingly no reads or writes happening. With the SSD being hogged by some invisible process, I wasn't able to open the drive in file explorer or launch any of the games installed on that drive.</p>

<p>What's also strange is that the drive would go back to normal after about 5 minutes, every time I turned on my PC. After some research into fixing the problem, I found out that this particular issue could be caused by a LARGE number of settings, faults, or services. The first fixes I tried were disabling Superfetch and search indexing on the drive. These Windows services are meant to speed up basic use of the PC but those features were almost useless for a drive meant for only games. But disabling those services did not fix my issue. There were also other recommendations such as editing the Registry to disable a possibly bugged SATA Controller driver, running Disk Check on the Command Prompt, and running a TRIM on the drive.</p>

<p>None of the fixes I tried fixed the drive so I started to believe that there was a hardware issue rather than a software one. What finally made me give up on the drive was when my entire Operating System would basically freeze for moments at a time while the SSD was at 100% usage, even though it wasn't a system drive, or had any applications installed on it besides games. I ended up purchasing a 2 Terabyte NVME M.2 SSD which is much faster than the SATA III drive I had. But when I went to unplug the old SSD, I decided to try plugging it into a different SATA port and turned on my PC. After doing this the issue was completely gone and the SSD was running just fine. Always try the easiest fix when troubleshooting PC issues, I learned that the hard way.</p>
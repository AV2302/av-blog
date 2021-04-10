---
layout: default
title: Blog 6 SP21
date: '2021-04-09 16:30:00 -0700'
categories: blog update
published: true
---
<h1>Switching from a Normal SSD to an NVME Drive</h1>
<p>A few days ago I decided to upgrade my computer from a basic Solid State Drive to an NVME drive. Not only is an NVME drive four to five times faster than an SSD, but it also is a smaller form factor that doesn't need any cables. The motherboard on my PC has always supported an NVME drive but when I first built the PC I found it more cost effective to use a basic SSD as the boot drive that has Windows on it. With NVME drives becoming more mainstream and supply outgrowing demand, the prices have become similar to an SSD despite the large speed difference.</p>

<p>I bought a 1TB NVME drive to replace my 120GB SSD, but I didn't want to go through the process of reinstalling Windows and backing up all of my applications and files. Instead I opted to research on finding a good and free software to copy the contents of my SSD to my NVME drive. I settled on using Macrium Reflect Free edition which was both well reviewed and in my price range. The software was simple to use, all it took was selecting your drive in the list of drives connected to your PC, clicking "Clone this disk...", select the disk you want to clone to, then keep clicking continue until it starts the cloning process.</p>

<p>Once the disk was cloned I double checked the contents of the NVME drive and compared it to the SSD, both being an exact match. There was an issue I ran into upon further inspection of the NVME drive. When I viewed it in File Explorer, it only showed the drive having a capacity of 120GB, even though it was a 1TB drive. After doing some research I found out that this happens when using cloning software to clone a smaller capacity drive to a larger capacity drive. The fix was simple. Navigate to Disk Management by typing it into the Windows search bar and find the drive that needs fixing. Right-click the drive and select the option "Extend Volume". Select the default disk space allocation for the drive and click Finish. Once that's done the new drive is all set and ready for normal use.</p>
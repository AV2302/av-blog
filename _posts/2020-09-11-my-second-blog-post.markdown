---
layout: default
title: Blog 1
date: '2020-09-11 11:00:00 -0700'
categories: blog update
published: true
---
<h1>Working with Metasploitable and Kali Linux</h1>
<p>For my class CIT 425, we were assigned a lab where we have to get Metasploitable and Kali Linux up and running on a virtual machine software. Metasploitable is a virtual Linux machine that is intentionally vulnerable to exploits. It is made by Metasploit Project for the purpose of penetration and security vulnerability testing. I installed it on Virtual Box using the recommended system requirements and was able to run it with no issues. Kali Linux is also a security focused Linux system made by Offensive Security. I did end up having an issue trying to install Kali on Virtual Box.</p>

<p>Even though I allocated the required system resources that Kali needed, whenever I tried to run the installer, I kept running into an issue that would force me to restart the installation. I tried researching the issue and tried various fixes such as allocating more storage and RAM to Kali or turning on some Virtual Box options, but none of those worked. I found out that I had a pretty old installation version of Virtual Box and I ended up updating it and restarting my PC. When I tried the installer again it finished with no error.</p>

<p>Now that I had both running the next step of the lab was to make sure they could communicate. I stopped both systems and changed their network adapter settings so that they wouldn’t connect to the internet but instead be assigned a host-only IP address so that only I could connect to them, and they can’t access the outside world. The reason for this being that these two systems are going to have malicious traffic running to each other and I don’t want to risk that traffic reaching other devices or another network. Once I did that, I restarted both systems and ran the ifconfig command to get their inet addresses, which is the IP address assigned by the host-only adapter DHCP, and I was able to ping each other’s address.</p>
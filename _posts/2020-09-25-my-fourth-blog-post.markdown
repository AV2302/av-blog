---
layout: default
title: Blog 3
date: '2020-09-25 21:30:00 -0700'
categories: blog update
published: true
---
<h1>CIT 425 Lab 0: The Conclusion</h1>
<p>In my previous couple blogs, I detailed my trials and tribulations I went through while using Metasploitable and Kali Linux to finish lab 0. I was finally able to get Kali to run normally without crashing and I could move on to the final steps of the lab assignment. I had to use Metasploitable to replace the default site that was being served by apache with an original website I design myself. I chose to make a simple restaurant website with the location, menu, and prices on the homepage.</p>

<p>Apache uses the /var/www/html as the default directory to host websites from, so I navigated to that folder and renamed the index.php file so that it wouldn’t be served by apache until I rename it back.  Web servers will by default serve up a file named index to use as the homepage. I created a new file named index.html and used both HTML and CSS languages to design the website. When that was finished, I used the web browser on Kali to make sure I could connect to the site Metasploitable was hosting.</p>

<p>When I confirmed that it could connect, I could move on to the final step of the lab which was to deface the website I made using Kali to gain unauthorized access to a root shell on Metasploitable. To do this, I used the application called Armitage which is a cyber attack tool made by the creators of Metasploitable. Armitage is able to scan a network and display the machines it found. It can then give you a list of attacks it can perform on a targeted machine to give you access to a root shell. In the list of attacks, I ended up choosing an exploit that used a backdoor that was left in a fraudulent version of an IRC client, that just happened to be installed and running on Metasploitable. The exploit was successful and I used the root shell I now had access to, to edit the index.html file so the website now displayed messages saying the website was hacked. </p>
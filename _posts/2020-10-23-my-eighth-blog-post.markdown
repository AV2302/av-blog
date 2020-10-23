---
layout: default
title: Blog 7
date: '2020-10-23 14:30:00 -0700'
categories: blog update
published: true
---
<h1>Password Cracking Lab for CIT 425</h1>
<p>In my CIT 425 class, we were assigned a lab where we would be given an &#47;etc&#47;shadow file and a textfile of 100,000 passwords. We would use the 100,000 passwords to attempt to crack the passwords of the users on the &#47;etc&#47;shadow file. An &#47;etc&#47;shadow file is where all users on a Linux system have their encrypted passwords saved.</p>

<p>When a Linux user creates a password, that password is encrypted into something called a hash. Because Linux passwords are one-way hashed, meaning they can't be decrypted, the goal of the lab was to use a hashing command from a programming language to test the hash of all 100,000 passwords and see if they match the hash of the user on the &#47;etc&#47;shadow file. If they matched then that meant the correct password was found. I chose to use Python to make the script so I could use the crypt module.</p>

<p>The crypt module allows you to enter a plaintext password and a salt, with the output being a hashed version of the password. The salt is just random data that is combined with the hashing algorithm to make a more complex hashed password. The first thing I did was create seperate files for each user that each contained their hashed password. Then I coded a loop that would iterate through all 100,000 passwords, hash them using the crypt command, and compare that hash to the user's hash that I'm attempting to crack. By doing this I was able to find the password for every user in the &#47;etc&#47;shadow file.</p>
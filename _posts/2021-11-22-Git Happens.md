---
layout: post
title: Git Happens
---

tryhackme.com room

Alright, another tryhackme room that only has a single input. I wasn't 100% sure where to start, but when in doubt, nmap. A quick scan showed me that only port 80 was open, so either this was a colossal red herring, or the right path. I tried to log into the page, but none of the regular defaults worked. Tinkering some with nmap modes, I found a git repository. Well, since that's in the name of the room, I assumed I was on the right path. After some searching, I found some tools to pulling git repositories, and then translating them into something human readable. After that, it was a slow process of scanning each folder for the .html files, and seeing which one had the plaintext password. Since the room mentioned a version control, which I took to assume each later version was more secure, I started at the top, and worked my way down. In the file that started with 2-*, I found 
Th1s_1s_4_L0ng_4nd_S3cur3_P4ssw0rd! - which turned out to be correct. 

I stumbled at a few points, but overall this was a pretty fun room. The title was a decent hint, and helped me along some. 
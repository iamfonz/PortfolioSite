---
title: The Riddims Website
description: The Riddims band website built with ASP.net core.
date: "2017-11-05T19:47:09+02:00"
jobDate: 2017-2020
work: [full-stack web development,  cloud server]
techs: [ASP.NET Core, Bootstrap, CSS, DigitalOcean, GIMP]
designs: [ ]
thumbnail: /riddims-site/theRiddims.jpg
projectUrl: https://theriddims.com
draft: false

---


After graduating from [CNM](https://www.cnm.edu), I wanted to start building stuff. Some friends from high school needed a website for their band. I found it to be the perfect opportunity to help each other out. I could build them a website in exchange for free admission to their concerts and something to add to my portfolio.

I actually built this website two times. The first build I used ASP.Net with Entity Framework for the back end. I included a database so that they can update the website with upcoming shows. It also allowed them to showcase past shows to any potential promoters. I also used Bootstrap with some custom CSS for the front end. 

I hosted the website on [Microsoft Azure](https://azure.microsoft.com/en-us/). However, over time it proved to be too expensive to host considering the extent of the website. There weren't users and a bunch of dynamic data to be served. The site is mainly static pages with concerts to be updated from time to time. It was hosted on Azure for about a year. Then I decided to make a change to bring down the cost.

.Net Core was really gaining traction at the time. I loved the fact that it's cross-platform. That alone sold me on using it to start building with it. My quest to redo their website in .net Core began.

A lot of it stayed the same. The most major changes were on the front end and removal of the database. The band members began using [SongKick](https://www.songkick.com/?utm_medium=referral&utm_source=widget&utm_campaign=8600399) to promote their concerts. SongKick has an upcoming shows widget that easily embeds on to websites. They preferred to do this rather than have to update their database. This made building it a lot easier and faster.

The second version of the site is now hosted on [DigitalOcean](https://m.do.co/c/d2a53e8b19fa). I used a Ubuntu server with Nginx as a reverse proxy. This cut down costs considerably. Not to mention, it's made it easier for me to administer the site as I'm quite comfortable in Linux.  This solution proved to be the best for me.

I still currently adminster the site for them. I simply SSH into the server whenever I need to make some updates. I own the repo on Github, though it is private. I'd be happy to share it upon request to showcase my work and skills to potential employers. 

##### Disclaimer
The DigitalOcean link above is a referral link. Per DigitalOcean "Everyone you refer gets $100 in credit over 60 days. Once they’ve spent $25 with us, you'll get $25. There is no limit to the amount of credit you can earn through referrals."
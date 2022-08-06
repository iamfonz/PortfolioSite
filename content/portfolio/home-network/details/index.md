---
title: Details - Home Network Project
description: Details of my home netowrk project
date: "2022-05-02T19:47:09+02:00"
jobDate: 2022
work: [network, DIY]
techs: [Networking, OpnSense, CAT6, RG6]
designs: [ ]
thumbnail: home-network/images/rackAlmostComplete.JPG
#projectUrl: https://github.com/iamfonz/MetalOMatic
draft: true

---

# Intro
If you made it here you either want to nerd out, or learn about networking a home. Either way, you've landed where I detail my project of setting up a custom home network.

Most people setup a moderm/router combo with their ISP (internet service provider), setup a Wi-Fi network, and call it a day. But not me. I wanted to have much more control of my home network. I specifically wanted to have the abiltiy to setup VLANs and Firewall rules for Cyber Security purposes, as well as have the ability to hardwire many devices to the network. While I won't share my entire configuration, I'll outline what I did and why.

# CAT6 Runs
The absolute beginning of everything was running CAT6 cabling throughout my home.

 I started out by buying 1500 ft of CAT6 cabling in bulk. I initially had the idea of running one cable at a a time. However, once I was in the attic (cooking my insides) I realized it'd be more efficient to do two cables at once. That prompted me to buy another box of 500 ft s I could run two cables at once.

 ## Challenges of Running CAT6 in My Home
I had a special case where my house has "two" roofs. At one point in time, my house had a flat roof. Then at some point, the previous owner added a pitched roof on top of the flat roof. This presented an extra challenge in that I had to be meticulous as to where I drilled holes from inside the roof to pentetrate the interiors of the walls where I wanted connections. 

I overcame this challenge by using an eigth-inch X 18-inch drill bit to penetrate through the drywall of the ceiling into the attic, and then inserting a white 12-gauge wire into the hole. That allowed me to see the wire in the attic and thus giving me an idea of where I needed to drill to penetrate both roofs, and top-plates of the walls to get inside them and run my wire. Once the whole was made, I used a fishing wire to push through the whole where I had a helper use a strong magnet to catch the fishing wire and pull it through the hole where the connection plate would be. The helper then taped the CAT6 and RG6 cable to the fishing wire and I slowly pulled on it inside the attic. We communicated through cell phones to coordinate releasing more wire from the bulk box as I pulled it through the attic to the drop location. Once I made it to the drop location, my helper terminated the cable and wound it up at the drop location.

![First drop example](/portfolio/home-network/images/twoRuns.JPG)
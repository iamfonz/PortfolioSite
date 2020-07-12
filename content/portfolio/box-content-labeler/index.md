---
title: Box Content Labeler
description: A program that generates a barcode label that contains the contents of a box in a formatted string per Amazon's spec.
date: "2017-10-02T16:30:16+02:00"
jobDate: 2017-2019
work: [desktop, e-commerce, amazon, thermal printers]
techs: [.Net, Entity Framework, WPF, ZPL, PDF17]
designs: [ ]
thumbnail: 
projectUrl: 
draft: true

---

My previous employer, Shoe Box, is an online shoe retailer. One of my responsibities was to ship product to Amazon warehouses where orders would be fulfilled by Amazon on our behalf. In 2017, Amazon started requiring shippers to provide box content information for all of the boxes in a shipment. They would eventually start charging procesing fees for each item in a box that did not contain box content information. We calculated that these were going to add up quickly for us. Especially considering we ship thousands of shoes a month. 

I had two semester's worth of .Net under my belt from [CNM](https://www.cnm.edu), that I felt confident in tackling this problem. In 2014, I implemented using iPods as scanners around the warehouse to collect inventory data. We naturally adopted them to also collect the box content data. The first iteration was designed to handle the output of the iPod scanners, which was a collection of text files, each representing a box. The Box Content Program v1.0 opened all of them at once, parsed through to collect data, created a formatted string to Amazon's spec to be printed on a thermal label with a PDF417 barcode. 
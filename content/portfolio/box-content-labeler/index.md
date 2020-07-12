---
title: Box Content Labeler
description: A program that generates a barcode label that contains the contents of a box in a formatted string per Amazon's spec.
date: "2017-8-02T16:30:16+02:00"
jobDate: 2017-2019
work: [desktop, e-commerce, amazon, thermal printers]
techs: [.Net, Entity Framework, WPF, ZPL, PDF417, EPPlus]
designs: [ ]
thumbnail: 
projectUrl: 
draft: true

---

My previous employer, Shoe Box, is an online shoe retailer. One of my responisbilities was to ship product to Amazon warehouses where orders would be fulfilled by Amazon on our behalf. In 2017, Amazon started requiring shippers to provide box content information for all of the boxes in a shipment. They would eventually start charging procesing fees for each item in a box that did not contain box content information. We calculated that these were going to add up quickly for us. Especially considering we ship thousands of shoes a month. 

I had two semester's worth of .Net under my belt from [CNM](https://www.cnm.edu), that I felt confident in tackling this problem. In 2014, I implemented using iPods as scanners around the warehouse to collect inventory data. We naturally adopted them to also collect the box content data. The first iteration was designed to handle the output of the iPod scanners, which was a collection of text files, each representing a box. The Box Content Program v1.0 opened all of them at once, parsed through to collect data, created a formatted string to Amazon's spec to either be printed on a thermal label with a PDF417 barcode, or saved as a PDF to print from a regular ink printer.

One of the first updates I added was the ability to accept Microsoft Excel files using [EPPlus](https://github.com/JanKallman/EPPlus). One day I found an old USB barcode scanner in a closet that we started using with a laptop. This little upgrade allowed us to process shipments faster by being able to scan each box into a Worksheet inside an Excel Workbook file. I was able to implement the ability to accept an Excel workbook as well as the text files from the first iteration. It allowed flexibility in that if one team was using the laptop and scanner, another team can still continue to process shipments with the iPods. Eventually we received a big tech upgrade in 2018 and received two laptops and three industrial Honeywell barcode scanners.

![Major Update](/assets/images/philly-magic-gardens.jpg "Major Update")

After that small update, I did a pretty major update to add more functionality and areas to explore in the interface. 
- First, I added a database to hold all of the shipments data. In the first iteration, all shipment and label data were saved in files to a specified directory in a configuration file. I implented a database using Entity Framework. 
- With the a database addition, I wanted to add the ability to see shipment history and re-print any label(s). This enormously came in handy when we needed to do some inventory reconciliation.
- I added a settings view to the interface to quickly make changes without having to mess with any configuration files. It made it more user-friendly overall which the warehouse team really appreciated.
- I also added an Amazon Warehouses view to perform any CRUD functionality for warehouses in the database.
- Lastly, I added a Help view that is ultimately the user guide to the program. It documents how to use the program and the various features.

The program was written mostly at work with a few hours where possible on evenings and weekends. It was a great opportunity to grow and learn a lot. I came across many challenges from learning about PDF417 barcodes, to  learning Zebra Programming Language (ZPL) to create the thermal labels. It also allowed me to improve interpersonal skills by constantly seeking and gaining feedback from colleagues who were using the program as well as myself. Overall I feel fortunate to have been given the opportunity to write this as well as the trust and confidence my supervisors at Shoe Box had in me.
---
title: "Utilities"
date: 2021-07-13T14:47:40+03:00
draft: false
layout : "projects"

description: "Track cost and consumption of utilities. Obrain insights from the data."
about: ["Track cost and consumption of utilities. Obrain insights from the data."
        ,"The application keeps log of invoice data and also invoices could be stored on the cloud (like an azure storage account). Uses statistics to find trends, outrliers, recommend actions based on histoirical data and predict future expences. Also reminds for upcomming activities based on flexible business logic. Maintenance requires approval prior to archiving."]
motivation: 
        ["Automating the operation allows the usage of repetitive processes, good practices, and the collection of data that can be used for business inteligence or data mining."
        ,"The application started as a Google sheets file. In this incarnation, it allows the management of multiple vehicles, provide statistical information, and visualizations."
        ,"As the interest in the product increased, I realized that the shortcomings in the platform limit the usability. Each new customer had to have its own version of the application and aggregating the information from multiple files results in an overhead. Although google sheets are available in a mobile version as well, the experience is very different compared with the desktop version."]
challenges: ["The first challenge was to build a data layer that could be used for statistical analysis of data."
            ,"The second challenge was to be able to apply statistical analysis on the whole dataset while retaining each user's data private."
            ,"The third challenge was to allow secure usage from multiple users on desktops and mobile devices."
            ,"The fourth challenge was to use architecture and design that allow changes."]
approach: ["Considering the nature of the application - a database one, I decided to use the Oracle 11g XE that comes with a preinstalled APEX and a web server, that unfortunately requires a license to use SSL."
            ,"To use SSL I deployed an Apache running on Ubuntu server 16.04, that acts as a reverse proxy and SSL offloader. The certificate was obtained from Let's Encrypt."
            ,"Power BI report is available and could be updated from a reporting server, while the later is feed from the application database.",]
services: true
---


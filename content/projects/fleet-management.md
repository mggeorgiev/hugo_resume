---
title: "FLEET MANAGEMENT"
date: 2021-01-21T23:47:48+03:00
draft: false
description: "Manage effectively and efficiently vehicle fleets."
about: ["Manage a vehicle is something that most owners experience (except if they have hired someone to do it on their behalf). Some even enjoy it, despite that most tasks are mundane. Adding cars to form a fleet comes with an overhead."
        ,"The application keeps log of both refueling and maintenance. Uses statistics to find trends, outrliers, recommend actions based on histoirical data and predict future expences. Also reminds for upcomming activities based on flexible business logic. Maintenance requires approval prior to archiving."]
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
---



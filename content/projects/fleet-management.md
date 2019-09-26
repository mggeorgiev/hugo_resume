---
title: "FLEET MANAGEMENT"
date: 2019-09-21T23:47:48+03:00
draft: false
description: "Intelligent management and process automation for condominia in the republic of Bulgaria."
about: "The application keeps log of income and outcome cost. Automates budgeting. Post and distribute messages accros different roles within homeonewners assossiation. Facilitates trhe management of the homeowners book and decisions log. The analytical module provides prediction based on historical data."
motivation: "Automating the operation allows the usage of repetitive processes, good practices, and the collection of data that can be used for business inteligence or data mining."
challenges: ["The first challenge was to build a data layer that could be used for statistical analysis of data."
            ,"The second challenge was to be able to apply statistical analysis on the whole dataset while retaining each user's data private."
            ,"The third challenge was to allow secure usage from multiple users on desktops and mobile devices."
            ,"The fourth challenge was to use architecture and design that allow changes."]
approach: ["Considering the nature of the application - a database one, I decided to use the Oracle 11g XE that comes with a preinstalled APEX and a web server, that unfortunately requires a license to use SSL."
            ,"To use SSL I deployed an Apache running on Ubuntu server 16.04, that acts as a reverse proxy and SSL offloader. The certificate was obtained from Let's Encrypt."
            ,"Power BI report is available and could be updated from a reporting server, while the later is feed from the application database."]
---


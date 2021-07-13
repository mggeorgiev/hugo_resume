---
title: "martingeorgiev.info"
date: 2021-07-13T14:47:40+03:00
draft: false
layout : "projects"

files: "https://www.martingeorgiev.info"
graphs: "#graphs"
predictions: "#predictions"

description: "A static web site generated with HUGO. Hosted on the cloud."
about: ["CV like one page site that is generated with HUGO and then automatically deployed on an Azure storage account. The site is delivered via Azure CDN. It has a certificate from Azure."]
motivation: 
        ["After a newtwork issue that cut off the version that was hosted on premise I decided to replace it with one that is hosted on the cloud. the requirements are that the updates are automated, including the certificate renewal."]
challenges: ["The first challenge was to automate the deployment of the required resources (storage account and cdn) on Azure."
            ,"The second challenge was to deploy the site on the storage account"
            ,"The third challenge was link the CDN with the storage account"
            ,"The fourth challenge was to create a GitHub action to automatically deploy the site once a commit is made and to update the CDN"
            ,"The fifth challenge was how to renew the Let's Encrypt certificate as the existing automation scripts will not work on Azure."]
approach: ["The infrastructure was created using terraform together will all the necessary configurations
. Examples are available at https://github.com/mggeorgiev/azure."
            ,"Deploying manually was not a problem but I found a way to combine uploading the content with a purge of the cdn into a Github action."
            ,"All details are available in Github."]
---


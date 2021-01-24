---
title: "API"
date: 2021-01-24T21:47:55+03:00
draft: false
description: "How to use the exposed APIs"
about: ["The site exposes the following APIs:"]
api:
    - name: healthcheck
      url: "/healthcheck"
      description: "Healthcheck mechanism"
      schema:
            - title
            - home_page_url
            - status
            - message
    - name: jsonfeed
      description: "JSON feed"
      url: "/jsonfeed"
      schema: ""
    - name: api
      url: "/api"
      description: "Exports education and certificatiion in a json format"
      schema: ""
layout : "api"
---
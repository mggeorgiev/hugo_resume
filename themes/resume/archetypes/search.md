
---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
#featured: true
description: "Text used in summary on main page"
tags: ["techtags","used","in","website"]
image: ""
link: "URL linked from project details page"
fact: "Interesting little tidbit shown below image on summary and detail page"
weight: 500
sitemap:
  priority : 0.8
---

{{ define "main" }}
{{ partial "about.html" .}} {{ if .Site.Params.showExperience }} {{ partial "experience.html" . }} {{ end }} {{ if .Site.Params.showEducation }} {{ partial "education.html" . }} {{ end }} {{ if .Site.Params.showSkills }} {{ partial "skills.html" . }} {{ end }} {{ if .Site.Params.showProjects }} {{ partial "projects.html" . }} {{ end }} {{ if .Site.Params.showCertificates }} {{ partial "certificates.html" . }} {{ end }} {{ if .Site.Params.showOpenSource }} {{ with .Site.GetPage "section" "projects/contributions" }} {{ .Scratch.Set "sectionId" "open" }} {{ partial "sectionSummary" . }} {{ end }} {{ end }} {{ if .Site.Params.showPublications }} {{ with .Site.GetPage "section" "publications" }} {{ .Scratch.Set "sectionId" "publications" }} {{ partial "sectionSummary" . }} {{ end }} {{ end }} {{ if .Site.Params.showBlog }} {{ with .Site.GetPage "section" "blog" }} {{ .Scratch.Set "sectionId" "blog" }} {{ partial "sectionSummary" . }} {{ end }}
{{ end }} {{ end }}


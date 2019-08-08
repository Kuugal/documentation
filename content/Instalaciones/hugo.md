---
title: "Hugo"
date: 2019-08-05T10:21:50-05:00
draft: false
tags: ["hugo", "CMS"]
menuTitle : "Hugo CMS"
---
<img src="/img/hugo-logo.svg" width="720">
### ¿Qué es hugo?
___
Hugo is a fast and modern static site generator written in Go, and designed to make website creation fun again.
Hugo is a general-purpose website framework. Technically speaking, Hugo is a static site generator. Unlike systems that dynamically build a page with each visitor request, Hugo builds pages when you create or update your content. Since websites are viewed far more often than they are edited, Hugo is designed to provide an optimal viewing experience for your website’s end users and an ideal writing experience for website authors.

Websites built with Hugo are extremely fast and secure. Hugo sites can be hosted anywhere, including Netlify, Heroku, GoDaddy, DreamHost, GitHub Pages, GitLab Pages, Surge, Aerobatic, Firebase, Google Cloud Storage, Amazon S3, Rackspace, Azure, and CloudFront and work well with CDNs. Hugo sites run without the need for a database or dependencies on expensive runtimes like Ruby, Python, or PHP.

We think of Hugo as the ideal website creation tool with nearly instant build times, able to rebuild whenever a change is made.

### Windows
___
1. Download the latest zipped Hugo executable from [Hugo Releases](https://github.com/gohugoio/hugo/releases)

2. Create a subfolder in the Hugo folder: C:\Hugo\bin

3. Extract all contents to your ..\Hugo\bin folder

4. Agrega la variable de entorno C:\Hugo\bin a PATH 
    * Right click on the Start button
    * Click on System
    * Click on Advanced System Settings on the left
    * Click on the Environment Variables… button on the bottom
    * In the User variables section, find the row that starts with PATH (PATH will be all caps)
    * Double-click on PATH
    * Click the New… button
    * Type in the folder where hugo.exe was extracted, which is C:\Hugo\bin
    * Click OK at every window to exit

Comprueba la instalación con:

    hugo version

{{% notice note %}}
Usa **hugo help** para ver la lista de comandos disponibles
{{% /notice %}}



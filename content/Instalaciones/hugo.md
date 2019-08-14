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

{{% notice tip %}}
Download the latest zipped Hugo executable from [Hugo Releases](https://github.com/gohugoio/hugo/releases)
{{% /notice %}}

### Windows
___

1. Create a subfolder in the Hugo folder: C:\Hugo\bin

2. Extract all contents to your ..\Hugo\bin folder

3. Agrega la variable de entorno C:\Hugo\bin a PATH 
    * Right click on the Start button
    * Click on System
    * Click on Advanced System Settings on the left
    * Click on the Environment Variables… button on the bottom
    * In the User variables section, find the row that starts with PATH (PATH will be all caps)
    * Double-click on PATH
    * Click the New… button
    * Type in the folder where hugo.exe was extracted, which is C:\Hugo\bin
    * Click OK at every window to exit

### Linux
___


#### Debian-like 

1. Instala el paquete *.deb*

#### Tarball
##### Decide the location

When installing from the tarball, you have to decide if you’re going to install the binary in /usr/local/bin or in your home directory. There are three camps on this:

1. Install it in /usr/local/bin so that all the users on your system have access to it. This is a good idea because it’s a fairly standard place for executables. The downside is that you may need elevated privileges to put software into that location. Also, if there are multiple users on your system, they will all run the same version. Sometimes this can be an issue if you want to try out a new release.

2. Install it in ~/bin so that only you can execute it. This is a good idea because it’s easy to do, easy to maintain, and doesn’t require elevated privileges. The downside is that only you can run Hugo. If there are other users on your site, they have to maintain their own copies. That can lead to people running different versions. Of course, this does make it easier for you to experiment with different releases.

3. Install it in your Sites directory. This is not a bad idea if you have only one site that you’re building. It keeps every thing in a single place. If you want to try out new releases, you can make a copy of the entire site and update the Hugo executable.

##### Install into your *bin* directory

    # create the directory if needed
    mkdir -p ~/bin

    # make it the working directory
    cd ~/bin

    # extract the tarball
    tar -xvzf ~/Downloads/hugo_X.Y_osx-64bit.tgz
    Archive:  hugo_X.Y_osx-64bit.tgz
    x ./
    x ./hugo
    x ./LICENSE.md
    x ./README.md

    # verify that it runs
    ./hugo version
    Hugo Static Site Generator v0.13 BuildDate: 2015-02-22T04:02:30-06:00

You may need to add your bin directory to your PATH variable. The `which hugo` command will check for us.
If it can find hugo, it will print the full path to it. Otherwise, it will not print anything.
```
# check if hugo is in the path
which hugo
/Users/USERNAME/bin/hugo
```

If hugo is not in your PATH, add it by updating your ~/.bash_profile file. First, start up an editor.
```
nano ~/.bash_profile
```

Add a line to update your PATH variable.
```
export PATH=$PATH:$HOME/bin
```
Close the terminal and open a new terminal to pick up the changes to your profile. Verify your success by running the `which hugo` command again.

You’ve successfully installed Hugo.
___

Comprueba la instalación con:

    hugo version

{{% notice note %}}
Usa **hugo help** para ver la lista de comandos disponibles
{{% /notice %}}



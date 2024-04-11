---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Developing On Fedora Kinoit
title: "How to Develop on Fedora Kionit Using VSCodium"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: Linux
# multiple tag entries are possible
tags: [Linux, Developing]
# thumbnail image for post
img: ":FedoraKinoite.jpg"
# disable comments on this page
comments_disable: false

# publish date
date: 2024-04-11 21:55:00 +0900

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-01-01 10:04:30 +0900
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
published: true
---

<h1><b>I'm user Fedora Kionit and sometimes I use **VSCodium** for writing programming.</b></h1>
For developing, I have two options.
Firstly, I must create a virtual machine and start developing.
Second solution: we can create a container and start developing.

For the second solution, we can create a container using distrobox and export it to the desktop and use it.
However, I don't like installing **VSCodium** directly into distrobox for privacy reasons. I prefer to install all software using **Flatpak**, which is very **restricted**.

<h2>Create a Container Fedora</h2>
Okay, let's go ahead and create a container using distrobox:

`distrobox create namecontainer --image registry.fedoraproject.org/fedora-toolbox:39`

After pulling it, we can run it using this command:

`distrobox enter namecontainer`

<h2>Configure Fedora For SSH</h2>

After that, we must configure the Fedora environment created using distrobox. Let's proceed.

Firstly, install software on the container:

`sudo dnf install policycoreutils-python-utils cracklib-dicts cracklib`

After that, we must **turn off SELinux**:
`sudo setenforce 0`

Next, we need to configure sshd. Firstly, uncomment the **port** and **PermitRootLogin** lines. For example:

`port 9050`
`PermitRootLogin yes`

Then, to start sshd:

`sudo /usr/sbin/sshd`

For **debugging**, you can run:

`sudo /usr/sbin/sshd -d`

Next, we need to **configure root**. Use this command:

`sudo passwd`

<h2>ssh</h2>

To connect, use ssh:

`ssh root@localhost -p 9050`

<h2>Install Extension VSCodium</h2>

<a href="https://open-vsx.org/vscode/item?itemName=jeanp413.open-remote-ssh">Open remote ssh</a>

<h2>Connect With Extension</h2>

then you can use the shortcut **ctrl+Shif+p** and select **remote ssh connect** to host and write ssh to the container.

Enjoy life!

<i>Thank you for reading this post. I wish you to have a nice day and a great time.</i>

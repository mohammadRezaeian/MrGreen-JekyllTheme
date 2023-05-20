---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Change Frequency CPU 
title: "Change Frequency CPU Such Wow!"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: Linux
# multiple tag entries are possible
tags: [Linux, CPU]
# thumbnail image for post
img: ":Cpu.jpg"
# disable comments on this page
comments_disable: false

# publish date
date: 2023-05-20 11:45:30 +0900

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



<h1><b>Hi
I writing this document because I think some times we need use maximum frequency CPU or GPU alternative let's set it ourselves instead of leaving it to the kernel </b> </h1>

<b>After that what's happen ?</b> <br>
be carefully this work causes the power will increase and its temperature will also increase

<h3>ok now let's go </h3>

wee need install this package:

<b>in fedora</b>
<br>
`sudo dnf install cpufrequtils -y`
<br>
in debian:
<br>
`sudo apt install cpufrequtils -y`
<h4> Now we wan't increase frequency cpu

it's very easy really😃 you just need  use this command:
<br>
`sudo cpufreq-set -g  performance`
<br>
<h3> Now maybe asking how to make sure that it has increased</h3>
it's very easy just write this command:
<br>
`cpufreq-info`
<br>
if your output line <b>current policy: the governor  was "performance" it's increased</b>.

<i>thank you for reading this post
I wish you to have a nice day
have a great time.</i>

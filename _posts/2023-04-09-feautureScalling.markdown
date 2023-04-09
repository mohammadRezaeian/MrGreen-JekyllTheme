---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Feauture Scalling
title: "how to rescalling a point to another scale!"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: Math
# multiple tag entries are possible
tags: [Math]
# thumbnail image for post
img: ":FeautureScalling.jpg"
# disable comments on this page
comments_disable: false

# publish date
date: 2023-04-09 15:41:30 +0900

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



<h1><b>
how to  rescalling a point to another scale</b> </h1>

<b>maybe you ask why i write this?</b> <br>
I was trying write a generator number with cpp and i wanted send it to client and create a sine wave use with the points
you can see it one my github <a href="https://github.com/mohammadRezaeian/serverTCPCPPSTL">Server TCP Use API Kernel</a>

<br>

<h3>ok now let's go </h3>
<br>
<h3>how to change scalling :</h3>
<br>
it's very easy really😃 you just need 
to know these
<li>What's your Point</li>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;\acute{y}"/>
<br>
<br>
<li>What's your Range Maximum Number Input</li>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;InputRangeMax"/>
<br>
<br>
<li>What's your Range Minimum Number Input</li>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;InputRangeMin"/>
<br>
<br>

<li>What's your Range Maximum Scalling (width or height)</li>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;FinalScaleMax"/>
<br>
<br>
<li>What's your Range Minimum Scalling (width or height)</li>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;FinalScaleMin"/>
<br>
<br>
<h3> <b>And Formullar is</b><h3>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;\frac{y}{InputRangeMax-InputRangeMin}&space;=&space;\frac{y\rq}{FinalScaleMax-FinalScaleMin}&space;"/>
<br>
<br>
Imagine Number is number 30
ok let's go:<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;y=30"/>
<br>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;InputRangeMax=60"/>
<br>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;InputRangeMin=0"/>
<br>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;FinalScaleMax=540"/>
<br>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;FinalScaleMin=0"/>
<br>
<br>
<img src="https://latex.codecogs.com/svg.image?\Large&space;\frac{30}{60-0}&space;\div&space;\frac{y\rq}{540-0}&space;&space;=&space;\frac{30\times540}{60}&space;=&space;{y\rq}&space;is:&space;270"/>
<br>
<br>
<i> <a href="https://en.wikipedia.org/wiki/Feature_scaling"> for more information read wikipedia</a><br>
have a good time
---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Separated QML Components  Directories
title: "How To Create Separated Components Directories And Access With Versions"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: QML
# multiple tag entries are possible
tags: [Linux, Qt, QML]
# thumbnail image for post
img: ":QML.jpg"
# disable comments on this page
comments_disable: false

# publish date
date: 2023-07-08 10:25:30 +0900

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
I writing this document because  in the past i wanted to create many components without use C++, And setting up version for up them  </b> </h1>


<b>maybe you ask why?</b> <br>
Just see your projects <br>
You trying create many custom components for your projects first of everything it's fine because they are not very much<br>
Nut after months or week you seeing oh they are very much and It's very confused, <br>

Until this everything  it's ok <br>
you again try for continue but again you trying create new components with many new feature<br>
Maybe you saying it's ok <br>
Maybe you saying it's ok i must just create new directory <br>
Or i must just use  git <br>
But they aren't best way  you need  create version for access  them. <br>

<h3>ok now let's go </h3>

<b>How to create QMLDir file</b>

1. create a directory for your components (it's not matter you use Qt creator or terminal linux or....) after that going into directory:
  * `create file qmldir (example i use terminal in Gnu\Linux)`
  * `touch qmldir`

2. open it and
   * `example i use directory with name DesingControls`
   * `module DesingControls (name attention you must Observe the big or small letters )`

3. open now open .pro file (because i use qmake alternative cmake)
   * `QML_IMPORT_PATH += $$PWD/src/Ui (example i create a directory src  and into i create directory Ui  for qml files)`
  
4. adding path components directory into main.cpp
   * `engine.addImportPath("qrc:/src/Ui"); (engin is a object of QQmlApplicationEngine)`

5. now thinking you must add version for specific custom components 
   * `CustomButton  1.0     CustomButton.qml`

<br>
and now oh how can must use it<br>
imaging it's so hard 😂

let's go to file qml and just add this <br>

example:
* `import DesingControls 1.0 `

<i>in feature i trying write a example project for it </i><br>

<i>thank you for reading this post<br>
I wish you have great time </i>

---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: What's Gstreamer
title: "introduction Gstreamer"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: C++
# multiple tag entries are possible
tags: [CrossPlatform, Camera , Process Multimedia , CXX , C , Linux ,Qt]
# thumbnail image for post
img: ":Gstreamer.svg"
# disable comments on this page
comments_disable: false

# publish date
date: 2023-01-06 23:33:10 +0900

published: true
---

<h1></h1>

<h3>what's Gstreamer</h3> 
<b>First of Let me  Ask do you know what's FFmpeg ?</b>
<br>
<b>if your answer is yes</b>
<br/>
Now you know what's Gstreamer; because of many works is like FFmpeg
but when you need to work with Qt to show Output Video in QML we must use Gstreamer and use plugin qmlgsink

<br/>
<b>if your answer is No</b>
<br/>
Gstreamer is a software Cross Platform with many plugins for working with multimedia like sound or video to convert or do many works.

<br/>
<h3> why we must use Gstreamer</h3>
I saying Gstreamer has many plugins
because of those, we must do much work like can use Hardware to convert a video format to another format using GPU 
because GPU is very faster than CPU and resource is very low.
<br><br>

<h3> ok now let's go to know better than Gstreamer</h3>

<h4>Gstreamer Collections</h4>
<br/>
<b>Gstreamer plugins convert into Four Collections:</b>
<br></br>


<a href="#gst-plugins-base">gst-plugins-base </a><br/>
<a href="#gst-plugins-good">gst-plugins-good </a><br/>
<a href="#gst-plugins-bad">gst-plugins-bad </a><br/>
<a href="#gst-plugins-ugly">gst-plugins-ugly </a><br/>

<br/>
<h5 id="gst-plugins-base"><b>gst-plugins-base</b></h5>

a small and fixed set of plug-ins, covering a wide range of possible types of elements; these are continuously kept up-to-date with any core changes during the development series.

<br/>
<h5 id="gst-plugins-good"><b>gst-plugins-good</b></h5>

a set of plug-ins that we consider to have good quality code, correct functionality, and our preferred license (LGPL for the plug-in code, LGPL or LGPL-compatible for the supporting library).

<br/>

<h5 id="gst-plugins-ugly"><b>gst-plugins-ugly</b></h5>
a set of plug-ins that have good quality and correct functionality, but distributing them might pose problems. The license on either the plug-ins or the supporting libraries might not be how we'd like. The code might be widely known to present patent problems.

<br/>

<h5 id="gst-plugins-bad"><b>gst-plugins-bad</b></h5>
a set of plug-ins that aren't up to par compared to the rest. They might be close to being good quality, but they're missing something - be it a good code review, some documentation, a set of tests, a real live maintainer, or some actual wide use. If the blanks are filled in they might be upgraded to become part of either gst-plugins-good or gst-plugins-ugly, depending on the other factors.

<br/>
<a href="https://gstreamer.freedesktop.org/">for more information</a>

<i>it's was just an introduction I trying to show examples of code and show better examples for work with Gstreamer in Qt or just terminal.
thank you for reading this post<br>
have a good time.</i>
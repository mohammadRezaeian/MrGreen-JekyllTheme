---
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: Why We must need to know what's state Machine 
title: "Why we need to know what's State Machine and why we need it"

# post specific
# if not specified, .name will be used from _data/owner/[language].yml
author: Mohammad
# multiple category is not supported
category: C++
# multiple tag entries are possible
tags: [Linux, Network, C++]
# thumbnail image for post
img: ":stateMachine.jpg"
# disable comments on this page
comments_disable: false

# publish date
date: 2023-08-13 14:05:30 +0900

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
I writing this document because I think  all Developer needing to know what's state machine and use it. </b> </h1>

<b>maybe you ask why?</b> <br>
let me i telling a example for you <br>

in my projects i must handle too many data and all of them coming from a server <br>
maybe now you asking it's not problem we can read it very easy like use of just function readAll in library QTcpSocket or i don't know it's\depended your language using or your library but it's really easy because you don't want use of sysCall kernels <br>

all of theme until this is ok but a mistake happen and too many moving data  to you <br>
and you reading all of theme but now what's must happen ? <br>
thinking to it <br>
it's has many answers <br>
maybe your program crashed or you lost many data or your parser and your algorithm can't handle because you can't decide which data is for use of your function <br>
ok now you told me what's the best way for solving this problem maybe you have many answers but The most basic way to use is use of state machine  <br>

<h2><b>Explain why must to know state machine </b> </h2>

let me i explain it whit an example <br>

when you are riding a machine and using it you don't want to know anything about it  <br>
and you just need to know when time must use pedal  <br>
because all operation are happen other class and you just need to know how you must work with pedal <br>
yes just this  <br>

but when you start write a class for handle pedal you must need to know many things \
like write a class for know when time our class must upper speed machine  or when time must down speed machine <br>
and it's so easy you just must write a function for input data and handle it and if to many data coming for you  <br>
you will not have much problems <br>

<h2><b>What's state machine</b> </h2>
it's a category of states of happen in your program <br>

like example problem  network i told you  <br>
let me i explain better than problem network  <br>
in your server when data must send to you  <br>
it's use a character in header for set this is start of message and it's start from here  <br>
and using a ending character for set this is end of message <br>
when can use a state machine for handle it very easy <br>
because you can parse it and be make sure your data is right  <br>
and maybe you using a switch case in your function and handle it with a enum and whit it you have very beautiful code  <br>
and can reading it very easy <br>

<h3><b>Example Code</b></h3>

```
while (DATA_STATUS == DATASTATUS::PHASE_1 && _byteArray.size() >= PACKET_DATA_HEADER)  {
        if (_byteArray[0] == 'H' && _byteArray[1] == 'i') {
            DATA_STATUS = DATASTATUS::PHASE_2;
            _byteArray.remove(0, PACKET_DATA_HEADER);
        }
        else {
            _byteArray.remove(0, PACKET_DATA_HEADER);
        }
    }

    if (DATA_STATUS == DATASTATUS::PHASE_2 && _byteArray.size() >= PACKET_DATA_SIZE) {
        memcpy(_dataRecive, _byteArray.constData(), PACKET_DATA_SIZE);
        _byteArray.remove(0, PACKET_DATA_SIZE);
        DATA_STATUS = DATASTATUS::PHASE_1;

        double* _dataConverted = reinterpret_cast<double*>(_dataRecive);
        m_list.append(*_dataConverted);
        m_pastList.append(*_dataConverted);

        sendNumbers();
    } 
``` 

<h3><b>Explain it </b></h3>

i use a while for check all message coming and ensure it's bigger bigger than or equal my header file  <br>
because i must check header start message for find new messages  <br>

`while (DATA_STATUS == DATASTATUS::PHASE_1 && _byteArray.size() >= PACKET_DATA_HEADER)`

in an example server send me two character for start message:  <br>
i reading all message coming until find header and ensure new message start it  <br>

`if (_byteArray[0] == 'H' && _byteArray[1] == 'i')`  

<br>
example i found new message and i set state machine two another phase for other works  <br>

`DATA_STATUS = DATASTATUS::PHASE_2;` 

<br>
i remove header because i found new message  <br>

`_byteArray.remove(0, PACKET_DATA_HEADER);`  

<br>
and if i can't find it <br>
i must just remove as much as the size of the start message and back two while for iterate again for find start message <br>
and in phase two i parse message and again going back two while for find other new message for parsing<br>


<h5><b>summary</b></h5>
state machine is just a collection of deciding for working. <br>

<i>thank you for reading this post
I wish you to have a nice day
, have a great time.</i>

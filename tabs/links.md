---
layout: links
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_links

# publish date (used for seo)
# if not specified, site.time will be used.
#date: 2022-03-03 12:32:00 +0000

# for override items in _data/lang/[language].yml
#title: My title
#button_name: "My button"
# for override side_and_top_nav_buttons in _data/conf/main.yml
#icon: "fa fa-bath"

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:00 +0000
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
#published: false


# you can always move this content to _data/content/ folder
# just create new file at _data/content/links/[language].yml and move content below.
###########################################################
#                Links Page Data
###########################################################
page_data:
  main:
    header: "Resume"
    info: " "

  # To change order of the Categories, simply change order. (you don't need to change list order.)
  category:
    - title: "Educations"
      type: id_educations
      color: "gray"

    - title: "Experience"
      type: id_experience
      color: "#F4A273"

    - title: "Skills"
      type: id_Skills
      color: "#62b462"

    - title: "Favorites"
      type: id_Favorites
      color: "gray"

    - title: "Projects"
      type: id_projects
      color: "#F4A273"
      
  list:
    # id_educations
    - type: id_educations
      title: "B.S"
      url: "https://garmsar.iau.ir"
      info:  "Computer Science <b>B.S</b> IAU Garmsar Branch &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;<b>2016-2018</b>"

    - type: id_educations
      title: "A.S"
      url: "https://garmsar.iau.ir"
      info:  "Computer Science <b>A.S</b> IAU Garmsar Branch &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;<b>2016-2018</b>"

    # Experience
    - type: id_experience
      title: "<a href=https://Unalink.net>Unalink</a>"
      info:  "<b>C/C++ Programmer And SysAdmin</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;<b>2021-2022</b><br></br>My Responsibilities  included writing programs under in Linux for Embedded  C like ESP32( with IDF) Or work with Protocols <b>GPS103</b> Or <b>MQTT</b> , our mainly used Technologies C++."

    - type: id_experience
      title: "<a href=https://dkap.ir/>DKApadana</a>"
      info:  "<b>C/C++ Programmer</b> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<b>2021-2021</b><br></br>My Responsibilities  included writing programs under in Linux for Android , our mainly used technologies: <b>C++11</b> with Framework <b>Felgo</b>."

    - type: id_experience
      title: "<a href=https://hanasystemsco.com/>HANA</a>"
      info:  "<b>C/C++ Programmer And DB Designer,SysAdmin</b>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&emsp;&emsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<b>2019-2021</b><br><br/>My responsibilities included writing programs under Linux And Windows For Management UAV(Drone) , our mainly used technologies: <b>C++11</b> with <b>Qt</b> and write UI wih <b>QML</b> and work with various <b>Databases</b>."

    - type: id_Skills
      title: "C/C++"
      info:  "<i>Proficient in:</i> Standard <b>C++11 , Qt , Felgo  </b> Framework and use <b>QML</b> for write UI Programs and use <b>IDF</b> write programs for ESP32 Hardware.<br></br><i>Familiar with:</i> <b>Multi-threading</b> under <b> C++11 </b>thread library.<br> </br>"

    - type: id_Skills
      title: "DB"
      info:  "<i>Experienced with:</i> <b>Designing </b> database with <b>hand-written queries.</b>"

    - type: id_Skills
      title: "Gnu/Linux SysAdmin"
      info:  "<i>Experienced with:</i> IPtables , DNS , Docker, Podman , Hardening Linux"

    #Favorites    
    
    - type: id_Favorites
      title: "Embedded Linux"
      info: "I love Work with Embedded Linux Device. "

    - type: id_Favorites
      title: "IDF"
      info: "I love doing things that few people do , Like use IDF For Develop ESP32"

    - type: id_Favorites
      title: "C++"
      info: "I love working with C/C++ in any situation"

    - type: id_Favorites
      title: "Gnu\Linux"
      info: "I love working with GNU/Linux in any situation"

    - type: id_Favorites
      title: "Reading Book"
      info: "I like read a book about it before doing anything"
      

    - type: id_Favorites
      title: "Developing"
      info: "I'm very interested in spending some of the time to reading before start Develop"
    
# id_projects
    - type: id_projects
      title: "<b>DK Apadana</b>"
      info: "Khoshe android application"

    - type: id_projects
      title: "<b>HANA</b>"
      info: "<b>System Automation</b> and create other project For <b>Management UAV(Drone)</b> and write <b>Messenger</b>   for local network into company."

    - type: id_projects
      title: "<b>Personal(Qt)</b>"
      info: "First Mirror Finder For Project Fedora (is Distribution Gnu/Linux)"

    - type: id_projects
      title: "<b>Personal(Qt)</b>"
      info: "Music player"

    - type: id_projects
      title: "<b>Personal(BASH)</b>"
      info: "Music player"

    - type: id_projects
      title: "<b>Personal(BASH)</b>"
      info: "Script Music Finder for Distribution Gnu\Linux"

    - type: id_projects
      title: "<b>Personal(Fedora)</b>"
      info: "Script For Install Package and Many configuration for Fedora"

---

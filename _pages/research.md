---
title: "Research Projects"
permalink: /research/
layout: splash
author_profile: false          # Splash 通常不放侧栏
classes: wide                  # 全宽更好看
excerpt: "Selected and ongoing projects"

header:
  overlay_image: Project_Prosocial.png
  overlay_filter: 0.25
  #caption: "Photo: Your credit"
  #actions:
    #- label: "Get in touch"
      #url: "mailto:jingshu@u.nus.edu"
    #- label: "Google Scholar"
      #url: "https://scholar.google.com/"
      #icon: "fas fa-graduation-cap"

feature_row:
  - image_path: Project_Prosocial.png
    alt: "Project Prosocial"
    title: "Building a Harmonious Human–AI Society through Prosociality"
    excerpt: "This project envisions a future of a harmonious human–AI society, built not only on efficiency and productivity but also on empathy, care, and cooperation—values traditionally reserved for human society, now extended to the broader non-human world."
    url: "/research/project-a/"
    btn_label: "Read more"
    btn_class: "btn--primary"
  - image_path: Project_Alignment.jpg
    alt: "Project Alignment"
    title: "Humans Align with AI during Interaction"
    excerpt: "AI is assimilating human beings."
    url: "/research/project-b/"
    btn_label: "Read more"
    btn_class: "btn--primary"
---

{% include feature_row %}

## All Projects

{% include base_path %}
<div class="grid__wrapper">
  {% assign projects = site.research | sort: "date" | reverse %}
  {% for post in projects %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
</div>

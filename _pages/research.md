---
title: "Research Projects"
permalink: /research/
layout: splash
author_profile: false          # Splash 通常不放侧栏
classes: wide                  # 全宽更好看
excerpt: "Selected and ongoing projects"

# 顶部英雄横幅（可按需换图）
header:
  overlay_image: {{ "/images/Project_Prosocial.png" | relative_url }}
  overlay_filter: 0.25
  caption: "Photo: Your credit"
  #actions:
    #- label: "Get in touch"
      #url: "mailto:jingshu@u.nus.edu"
    #- label: "Google Scholar"
      #url: "https://scholar.google.com/"
      #icon: "fas fa-graduation-cap"

# 精选项目（手动挑 2-3 个）
feature_row:
  - image_path: {{ "/images/Project_Prosocial.png" | relative_url }}
    alt: "Project Prosocial"
    title: "Building a Harmonious Human–AI Society through Prosociality"
    excerpt: "This project envisions a future of a harmonious human–AI society, built not only on efficiency and productivity but also on empathy, care, and cooperation—values traditionally reserved for human society, now extended to the broader non-human world."
    url: {{ "/research/project-a/" | relative_url }}
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

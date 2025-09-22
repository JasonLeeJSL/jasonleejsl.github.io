---
layout: archive
title: "Publications"
excerpt: "Selected publications"
permalink: /publications/
author_profile: true
header:
  overlay_image: Hero_Figure.jpg
  overlay_filter: 0.3
---

{% include base_path %} {%- assign projects = site.research | sort: "date" | reverse -%} <div class="grid__wrapper"> {%- for post in projects -%} {%- include archive-single.html -%} {%- endfor -%} </div>

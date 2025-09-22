---
title: "Research Projects"
permalink: /research/
layout: splash
author_profile: true
---


{% include base_path %}
{%- assign projects = site.research | sort: "date" | reverse -%}
<div class="grid__wrapper">
{%- for post in projects -%}
  {%- include archive-single.html -%}
{%- endfor -%}
</div>

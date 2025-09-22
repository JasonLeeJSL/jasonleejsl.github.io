---
title: "Research Projects"
permalink: /research/
layout: archive
author_profile: true
entries_layout: grid   # list
---

{% include base_path %}

{%- assign projects = site.research | sort: "date" | reverse -%}
{%- for post in projects -%}
  {%- include archive-single.html type="grid" -%}
{%- endfor -%}

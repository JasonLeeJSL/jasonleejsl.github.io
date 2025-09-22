---
title: "Research Projects"
permalink: /research/
layout: archive
author_profile: true
entries_layout: grid      # ← 网格卡片
classes: wide             # ← 拉宽内容区
---


{% include base_path %}
{%- assign projects = site.research | sort: "date" | reverse -%}
<div class="grid__wrapper">
{%- for post in projects -%}
  {%- include archive-single.html type="grid" -%}
{%- endfor -%}
</div>

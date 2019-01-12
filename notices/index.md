---
layout: default
title: Notice
main : true
permalink: /notice/
description: 글을 아주 가끔씩 올립니다.
---

<section class="post-list">
  <div class="container">
    {% assign sorted = site.pages | sort: 'order' | reverse %}
    {% for page in sorted %}
    {% if page.notice == true %}
    {% include info-list.html %}
    {% endif %}
    {% endfor %}
  </div>
</section>



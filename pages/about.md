---
layout: page
title: About
description: 男人就应该对自己狠一点
keywords: 孤独剑, wolfyn, brucezhang13, wolfyn13
comments: true
menu: 关于
permalink: /about/
---

坚信熟能生巧，努力改变人生。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

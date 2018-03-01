---
layout: page
title: About
description: 伪极客一枚
keywords: Bruce zhang, 孤独剑
comments: true
menu: 关于
permalink: /about/
---

最可怕的事情，莫过于：这个世上有诸多美景，而我却碌碌一生。

愿你我能在最好的年华里，活出平凡却不平庸的自己。

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

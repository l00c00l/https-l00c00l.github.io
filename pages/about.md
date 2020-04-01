---
layout: page
title: About
description: 日有所得
keywords: Li Cuilian, 冷处理
comments: true
menu: 关于
permalink: /about/
---

人 人生 家人 亲朋 世界

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

---
layout: page
title: About
description: 打码改变世界
keywords: Bromine_Br
comments: true
menu: 关于
permalink: /about/
---

Bromine妙妙屋，主要发布二次元和音游相关

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
</ul>


## 这里有

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

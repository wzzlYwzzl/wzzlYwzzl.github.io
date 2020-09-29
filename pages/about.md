---
layout: page
title: 自我介绍
description: 不断学习
keywords: Jiawei Zhu , Garvey
comments: true
menu: 关于
permalink: /about/
---

我是 Garvey，性格比较内向的油腻中年。

喜欢钻研、学习，希望在技术的世界中寻求精神的满足。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ assets_base_url }}/assets/images/qrcode.jpg" alt="闷骚的程序员" />
</li>
{% endif %}
</ul>

## Skill Keywords

{% for skill in site.data.skills %}

### {{ skill.name }}

<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

---
layout: page
title: About
description: 改变世界
keywords: Yu Diao, 刁宇
comments: true
menu: 关于
permalink: /about/
---

我是刁宇，可能是一个有趣的人。

仰慕「优雅编码的艺术」。

人间的烟火，尘世的理想。

生而平凡，心向光明。

会在这里写一些自己觉得有趣的，有用的知识。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ assets_base_url }}/assets/images/qrcode.jpg" alt="有趣的程序员" />
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

---
layout: page
title: About
description: 这就是我，不一样的我
keywords: Saitama
comments: true
menu: 关于
permalink: /about/
---

曾子曰：“吾日三省吾身:为人谋而不忠乎? 与朋友交而不信乎? 传不习乎? ”

这只是一个博客

并且还没有弄好

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

---
layout: page
title: About
description: 粥粥粥菌的小站
keywords: 关于，粥粥
comments: true
menu: 关于
permalink: /about/
---
## 关于网站
网站成立辣，这个是个搭建在GitHub的静态网站。
什么？为什么不买个主机，php更香？
有钱买主机我还上GitHub？
233，实际是银行卡不能在线支付，emmm
[我的GitHub项目地址](https://github.com/ZhouJump/site.io)

## 关于作者

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## 奇怪的关键词增加了

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}

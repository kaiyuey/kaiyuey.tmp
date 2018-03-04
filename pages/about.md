---
layout: page
title: About
description: Let's Be Awesome
keywords: Kaiyue Yang
comments: true
menu: About
permalink: /about/
---

> 月·光

![What's next](/assets/img/ZootopiaIN.jpg)

## Introduction

Hey, I'm Kaiyue Yang, currently a Software Engineer at Amazon Alexa. 

## Contact

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

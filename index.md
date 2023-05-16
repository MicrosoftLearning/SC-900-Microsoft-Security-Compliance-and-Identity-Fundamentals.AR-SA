---
title: الإنترنت
permalink: index.html
layout: home
---


# دليل المحتوى

توجد أدناه روابط سريعة لكل من التمارين المعملية والعروض التوضيحية.

## الأنشطة المعملية

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| الوحدة | النشاط المعملي |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}


## العروض التوضيحية

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| الوحدة | عرض توضيحي |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}


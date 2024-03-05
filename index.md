---
title: التعليمات المستضافة عبر الإنترنت
permalink: index.html
layout: home
---

# دليل المحتوى

يتم سرد الارتباطات التشعبية لكل تمرين من التدريبات المعملية أدناه.

## الأنشطة المعملية

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| الوحدة النمطية | النشاط المعملي |
| --- | --- | 
{% للأنشطة في المعامل %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

<!---


## Demos

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| Module | Demo |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

--->

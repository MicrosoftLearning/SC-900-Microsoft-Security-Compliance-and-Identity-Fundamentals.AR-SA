<div id="readme" class="Box-body readme blob js-code-block-container p-5 p-xl-6 gist-border-0" dir="rtl">
    <article class="markdown-body entry-content container-lg" itemprop="text"><table>
  <thead>
  <tr>
  <th>title</th>
  <th>permalink</th>
  <th>layout</th>
  </tr>
  </thead>
  <tbody>
  <tr>
  <td><div>الإنترنت</div></td>
  <td><div>index.html</div></td>
  <td><div>home</div></td>
  </tr>
  </tbody>
</table>


# دليل المحتوى

توجد أدناه روابط سريعة لكل من التمارين المعملية والعروض التوضيحية.

## الأنشطة المعملية

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}
| الوحدة | النشاط المعملي |
| --- | --- | 
{% for activity in labs  %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
<!--

## العروض التوضيحية

{% assign demos = site.pages | where_exp:"page", "page.url contains '/Instructions/Demos'" %}
| الوحدة | عرض توضيحي |
| --- | --- | 
{% for activity in demos  %}| {{ activity.demo.module }} | [{{ activity.demo.title }}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
-->

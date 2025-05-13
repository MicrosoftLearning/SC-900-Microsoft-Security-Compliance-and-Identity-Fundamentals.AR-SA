<div class="readme html-blob blob p-5"><div class="Box-sc-g0xbh4-0 markdown-body container-lg"><div dir="rtl"><markdown-accessiblity-table data-catalyst=""><table>
  <thead>
  <tr>
  <th>title</th>
  <th>permalink</th>
  <th>layout</th>
  </tr>
  </thead>
  <tbody>
  <tr>
  <td><div dir="rtl">التعليمات المستضافة عبر الإنترنت</div></td>
  <td><div dir="rtl">index.html</div></td>
  <td><div dir="rtl">home</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 data-sourcepos="1:1-1:25" class="heading-element" dir="rtl">دليل المحتوى</h1><a id="user-content-دليل-المحتوى" class="anchor" aria-label="Permalink: دليل المحتوى" href="#دليل-المحتوى"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p data-sourcepos="3:1-3:111" dir="rtl">الروابط التشعبية لكل تمرين من التمارين المعملية مدرجة أدناه.</p>
<div class="markdown-heading" dir="rtl"><h2 data-sourcepos="5:1-5:34" class="heading-element" dir="rtl">الأنشطة المعملية</h2><a id="user-content-الأنشطة-المعملية" class="anchor" aria-label="Permalink: الأنشطة المعملية" href="#الأنشطة-المعملية"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p data-sourcepos="0:0-0:0" dir="rtl">{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs'" %}</p>
<markdown-accessiblity-table data-catalyst=""><table data-sourcepos="7:1-11:12">
<thead>
<tr data-sourcepos="7:1-7:153">
<th data-sourcepos="7:94-7:122">الوحدة النمطية</th>
<th data-sourcepos="7:124-7:152">النشاط المعملي</th>
</tr>
</thead>
<tbody>
<tr data-sourcepos="10:1-10:202">
<td data-sourcepos="10:1-10:40">{% للأنشطة في المعامل %}</td>
<td data-sourcepos="10:42-10:68">{{ activity.lab.module }}</td>
</tr>
<tr data-sourcepos="11:1-11:12">
<td data-sourcepos="11:1-11:12">{% endfor %}</td>
<td data-sourcepos="11:0-11:0"></td>
</tr>
</tbody>
</table></markdown-accessiblity-table>

</div></div>

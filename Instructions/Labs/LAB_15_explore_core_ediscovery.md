---
lab:
  title: استكشاف eDiscovery
  module: Describe the data compliance solutions of Microsoft Purview
---

# التمرين المعملي: استكشاف eDiscovery

يقوم هذا النشاط المعملي بتعيين محتوى Learn التالي:

- مسار التعلم: وصف قدرات Microsoft Priva وMicrosoft Purview
- الوحدة: وصف حلول توافق البيانات من Microsoft Purview
- الوحدة: وصف eDiscovery

## سيناريو النشاط المعملي

في هذا النشاط المعملي، ستتعرف على الخطوات المطلوبة لإعداد eDiscovery، بما في ذلك إعداد أذونات الدور وإنشاء حالة eDiscovery وإنشاء احتجاز eDiscovery وإنشاء استعلام بحث.  ملاحظة: يتطلب ترخيص eDiscovery (قياسي) اشتراك المؤسسة المناسب والترخيص لكل مستخدم. إذا لم تكن متأكداً من التراخيص التي تدعم eDiscovery (قياسي)، فتفضل بزيارة [بدء استخدام eDiscovery (قياسي) في Microsoft Purview](https://docs.microsoft.com/microsoft-365/compliance/get-started-core-ediscovery?view=o365-worldwide).

**الوقت** المقدر: 45 دقيقة

### المهمة 1

للوصول إلى eDiscovery (قياسي) أو إمكانية إضافته كعضو في حالة eDiscovery، ينبغي تعيين المستخدم للأذونات المناسبة. في هذه المهمة، بصفتك المسؤول العام، ستتولى إضافة مستخدمين محددين كأعضاء في مجموعة دور مدير eDiscovery.

1. افتح علامة تبويب المستعرض للصفحة الرئيسية لـ Microsoft Purview.  إذا أغلقتَه مسبقًا، فافتح علامة تبويب المستعرض وأدخل **https://admin.microsoft.com**. سجل الدخول باستخدام بيانات اعتماد المسؤول لمستأجر Microsoft 365 الذي يوفره مضيف النشاط المعملي المعتمد (ALH).

1. من جزء التنقل الأيمن من مركز إدارة Microsoft 365، حدد **عرض الكل**، ثم حدد **التوافق**.  تفتح صفحة مستعرض جديدة على صفحة الترحيب في مدخل Microsoft Purview.  

1. من جزء التنقل الأيمن، حدد **الإعدادات**، وقم بتوسيع **الأدوار والنطاقات**، ثم حدد **مجموعات** الأدوار.

1. في حقل البحث، في الجزء العلوي، يمين الصفحة، أدخل **eDiscovery** ثم اضغط على Enter على لوحة المفاتيح.  حدد **مدير eDiscovery**.

1. حدد **تحرير**. لغرض هذا المختبر، ستقوم بتعيين نفسك كمسؤول MOD كمدير eDiscovery ومسؤول.  في الممارسة العملية، يمكنك تعيين مستخدمين محددين لأدوار محددة.
    1. تتيح لك صفحة "إدارة eDiscovery Manager" إضافة مستخدمين إلى دور مدير eDiscovery.
    1. حدد **اختيار مستخدمين**. ابحث عن MOD Administrator** وحدده**، ثم اضغط **على Select** في أسفل الصفحة، ثم حدد **Next**.
    1. في صفحة "إدارة مسؤول eDiscovery"، حدد **اختيار المستخدمين**. ابحث عن MOD Administrator وحدده **، ثم اضغط **على Select** في أسفل الصفحة، ثم حدد **Next** ثم **Save**.**
    1. في صفحة "لقد قمت بتحديث مجموعة الأدوار بنجاح"، حدد **تمّ**.

1. اترك علامة تبويب المستعرض هذه مفتوحة، حيث ستستخدمها في المهمة التالية.

### المهمة 2

في هذه المهمة، بصفتك مسؤول eDiscovery (مسؤول MOD هو مسؤول eDiscovery)، ستنشئ حالة لبدء استخدام eDiscovery (قياسي).

1. يجب أن تظل على صفحة أدوار مدخل التوافق. إذا أغلقت علامة تبويب المستعرض من المهمة السابقة، فافتح علامة تبويب مستعرض جديدة وأدخل **compliance.microsoft.com** للوصول إلى مدخل Microsoft Purview.

1. من لوحة التنقل اليسرى، ضمن Solutions، قم بتوسيع **eDiscovery** ثم حدد **Standard Cases**.

1. من أعلى صفحة eDiscovery (قياسي)، حدد **+ إنشاء حالة**.

1. في نافذة حالة جديدة، أدخل اسم الحالة، **حالة اختبار SC900** ثم حدد **حفظ** في أسفل الصفحة.

1. ينبغي أن تظهر الحالة الآن في القائمة.

1. بصفتك منشئ الحالة ولأن لديك امتيازات مسؤول eDiscovery، يمكنك البدء في التعامل معها.  

1. اترك علامة تبويب المستعرض هذه مفتوحة، لأننا ستستخدمها في المهمة اللاحقة.

### المهمة 3

الآن بعد أن أنشأت حالة eDiscovery (Standard)، يمكنك البدء في التعامل مع هذه الحالة.  في هذه المهمة، ستنشئ احتجازًا في eDiscovery للحالة التي أنشأتها.  على وجه التحديد، ستقوم باحتجاز علبة بريد التبادل الذي ينتمي إلى Adele Vance.

1. افتح علامة تبويب eDiscovery (قياسي) في المستعرض.

1. من صفحة eDiscovery (قياسي)، حدد الحالة التي أنشأتها في علامة التبويب السابقة، **حالة اختبار SC900**.

1. من الصفحة الرئيسية للحالة، حدد علامة التبويب **احتجاز** ثم حدد **+ إنشاء**.

1. في حقل name، أدخل **Test hold** ثم حدد **Next**.

1. في صفحة Choose locations، حدد مفتاح التبديل بجوار **Exchange mailboxes** لتعيين الحالة إلى **On**.  

1. الآن حدد **Choose users, groups, or teams**.  في مربع البحث، أدخل **Adele** ثم اضغط على Enter بلوحة المفاتيح. من نتائج البحث، حدد **Adele Vance**، ثم حدد **Done**.

1. من صفحة اختيار المواقع، حدد **التالي**.  للملاءمة مع النشاط المعملي، لن يتم تضمين أي مواقع أخرى في هذا الاحتجاز.

1. تمكنك صفحة شروط الاستعلام من إنشاء قائمة احتجاز للعناصر استنادا إلى استعلام يمكنك إنشاؤه.  يمكنك اختيار استخدام منشئ الاستعلام لإنشاء استعلام أو للمستخدمين الأكثر تقدما، يمكنك استخدام محرر KQL. لهذا التمرين، تريد أن يحتفظ الاحتجاز بكافة المحتويات في الموقع المحدد للمستخدم المحدد، لذلك لن تقوم بإنشاء استعلام.

1. راجع إعداداتك وحدد **إرسال**، قد يستغرق الأمر دقيقة، ثم حدد **تمّ**.  ينبغي أن يظهر اختبار الاحتجاز في القائمة.  إذا لم تشاهده على الفور، حدد **تحديث**

1. اترك علامة تبويب المستعرض هذه مفتوحة، لأننا ستستخدمها في المهمة اللاحقة.

### المهمة 4

مع تطبيق الاحتجاز، ستتولى إنشاء استعلام بحث.  بمجرد اكتمال البحث، يدعم eDiscovery الإجراءات، مثل تصدير النتائج وتنزيلها للتحقيق في المستقبل.   ملاحظة: لا يتم سرد عمليات البحث المقترنة بحالة eDiscovery (قياسي) في صفحة البحث في المحتوى في مدخل Microsoft Purview. يتم سرد عمليات البحث هذه فقط في صفحة عمليات البحث الخاصة بحالة eDiscovery (قياسي) المقترنة.

1. افتح علامة تبويب SC900 Test Case في المستعرض.

1. من صفحة SC900 Test Case، حدد **Searches**.

1. من صفحة البحث، حدد **+ بحث جديد**.

1. في حقل الاسم، أدخل **اختبار الاحتجاز - بحث المبيعات**، ثم حدد **التالي** من أسفل الصفحة.

1. في الصفحة اختيار المواقع، حدد **المواقع الخاضعة للاحتجاز** ثم قم بإلغاء تحديد **إضافة محتوى التطبيق للمستخدمين المحليين**، حيث لا يوجد مستخدمين محليين في بيئة مختبرك، ثم حدد **التالي**.

1. تمكّنك صفحة شروط الاستعلام من إنشاء البحث، بناءً على كلمات رئيسية أو شروط محددة يتم استيفائها، في حقل الكلمة الأساسية، أدخل **المبيعات**، حدد **التالي**.

1. راجع إعداداتك وحدد **إرسال**، قد يستغرق الأمر دقيقة، ثم حدد **تمّ**.  ينبغي أن يظهر البحث في القائمة.  إذا لم تشاهده على الفور، حدد **تحديث**

1. من نافذة عمليات البحث، حدد البحث الذي أنشأته، **اختبار الاحتجاز - بحث المبيعات**.  تفتح نافذة تفتح تحديد علامة تبويب الملخص.  بمجرد اكتمال البحث، ستشير الحالة أن البحث قد اكتمل.  ستظهر لك علامة تبويب Search statistics (إذا لم تشاهد علامة التبويب إحصائيات البحث، فقد لا يزال البحث قيد التشغيل وقد يستغرق إكماله بضع دقائق).  حدد علامة التبويب **إحصائيات البحث** وحدد القائمة المنسدلة بجوار محتوى البحث.  يمكنك أيضًا عرض مزيد من المعلومات لتقرير الحالة وأهم المواقع.  

1. من أسفل الصفحة، حدد **الإجراءات**.  لاحظ الخيارات المتوفرة التي تتضمن خيارات التصدير (لا يمكن تحديد خيارات التصدير من داخل النظام الأساسي للنشاط المعملي الذي يوفره مضيف النشاط المعملي المعتمد، ولكنها متوفرة في بيئة إنتاج وتعتبر جزءًا من سير العمل القياسي). حدد **إغلاق**.

1. سَجِّل الخروج وأغلِق جميع نوافذ المستعرض المفتوحة.

### المراجعة

في هذا النشاط المعملي، استكشفت الخطوات المطلوبة لبدء استخدام eDiscovery (قياسي)، بما في ذلك إعداد أذونات الدور لـ eDiscovery وإنشاء حالة eDiscovery.  وباستخدام الحالة التي تم إنشاؤها، استعرضت عناصر سير عمل eDiscovery (قياسي) عن طريق إنشاء احتجاز eDiscovery، وإنشاء استعلام بحث.

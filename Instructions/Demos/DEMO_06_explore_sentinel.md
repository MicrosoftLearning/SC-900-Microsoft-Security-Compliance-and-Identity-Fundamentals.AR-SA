<!---
---
عرض توضيحي: العنوان: "Microsoft Sentinel" مسار التعلم/الوحدة النمطية/العنوان: "مسار التعلم: وصف قدرات حلول أمان Microsoft؛ الوحدة النمطية 3: وصف قدرات الأمان لـ Microsoft Sentinel؛ الوحدة 3: وصف كيف يوفر Microsoft Sentinel إدارة متكاملة للمخاطر"
---
--->

# عرض توضيحي: Microsoft Sentinel

يعيّن هذا العرض التوضيحي محتوى Learn التالي:

- مسار التعليم: وصف إمكانات حلول الأمان من Microsoft
- الوحدة النمطية: وصف القدرات الأمنية لـ Microsoft Sentinel
- الوحدة: وصف قدرات الكشف عن التهديدات والتخفيف منها في Microsoft Sentinel

## سيناريو العرض التوضيحي

في هذا العرض التوضيحي، ستتعرف على بعض الخيارات المتوفرة مع Microsoft Sentinel، بما في ذلك استخدام مركز المحتوى للعثور على الحلول المجمعة التي يمكنك نشرها.  ولكن أولًا، ستتعرف على عملية إعداد أذونات التحكم في الوصول المستندة إلى الأدوار للمستخدمين الذين سيحتاجون إلى الوصول إلى موارد Microsoft Sentinel.

### العرض التوضيحي - الجزء 1

يجب أن يكون مثيل Microsoft Sentinel قد تم إنشاؤه بالفعل كجزء من الإعداد السابق للعرض التجريبي. فتحقق من أنه تم إنشاؤه.

1. افتح علامة تبويب **الصفحة الرئيسية - Microsoft Azure** في المستعرض.  إذا قمت بإغلاق علامة التبويب مسبقا، فافتح صفحة مستعرض وفي شريط العناوين، أدخل **https://portal.azure.com**. سجل الدخول باستخدام بيانات اعتماد Azure التي يوفرها مضيف النشاط المعملي المعتمد (ALH).  ينقلك ذلك إلى الصفحة الرئيسية لخدمات Azure.

1. في مربع البحث، في الشريط الأزرق بأعلى الصفحة بجوار مكان ظهور Microsoft Azure، أدخل **Microsoft Sentinel** ثم حدد **Microsoft Sentinel** من نتائج البحث.  

1. في صفحة Microsoft Sentinel، ينبغي أن ترى مثيل Sentinel مدرجًا وحدده.  وإذا لم يكن مدرجًا، فبادر بإنشائه الآن.
    1. من صفحة Microsoft Sentinel، حدد **Create Microsoft Sentinel**.

    1. من صفحة "إضافة Microsoft Sentinel إلى مساحة العمل"، حدد **Create a new workspace**. من علامة تبويب الأساسيات في مساحة عمل إنشاء تحليلات السجل، أدخل ما يلي:
        1. Subscription: اترك الإعداد الافتراضي.
        1. مجموعة الموارد: حدد **إنشاء جديد** ثم أدخل الاسم **SC900-Sentinel-RG** ثم حدد **موافق**.
        1. الاسم: **SC900-LogAnalytics-workspace**.
        1. المنطقة: **شرق الولايات المتحدة** (يمكن تحديد منطقة افتراضية مختلفة استنادًا إلى موقعك)
        1. حدد **Review + Create** (لن يتم تكوين أي علامات).
        1. تحقق من المعلومات التي أدخلتها ثم حدد **إنشاء**.
        1. قد يستغرق الأمر دقيقة أو دقيقتين لإدراج مساحة العمل الواحدة، إذا كنت لا تزال لا تراها، فحدد **تحديث**، ثم حدد **إضافة**.
        1. بمجرد إضافة مساحة العمل الجديدة، سيتم عرض صفحة Microsoft Sentinel | News & guides، مما يظهر Microsoft Sentinel free trial is activated.  حدد **موافق**.

1. اترك علامة تبويب المستعرض هذه مفتوحة، لأنك ستستخدمها في المهمة اللاحقة.

### العرض التوضيحي - الجزء 2

كما هو الحال مع جميع موارد Azure، تريد التأكد من أن المستخدمين لديهم الأذونات المناسبة للوصول إلى موارد Microsoft Sentinel. وهنا، سوف تظهر الخطوات لتعيين دور والأدوار المتاحة للاستخدام مع Microsoft Sentinel.  

1. في مربع البحث، في الشريط الأزرق أعلى الصفحة بجوار المكان الذي تظهر فيه كلمة Microsoft Azure، أدخِل **مجموعة الموارد**، ثم حدد **مجموعات الموارد** من نتائج البحث. سيضمن تعيين الدور على مستوى مجموعة الموارد تطبيق الدور على جميع الموارد التي تم نشرها لدعم Microsoft Sentinel.

1. من صفحة مجموعات الموارد، حدد مجموعة الموارد التي قمت بإنشائها باستخدام Microsoft Sentinel، **SC900-Sentinel-RG**.

1. من صفحة SC900-Sentinel-RG، حدد **التحكم في الوصول (IAM)** من جزء التنقّل الأيسر.

1. من صفحة التحكم في الوصول، حدد **عرض الوصول الخاص بي**.  سترى على الأرجح تعيين دور مخصص تم تكوينه بالفعل لهذا الاشتراك وسيمنحك الأذونات اللازمة.  كان هذا الدور المخصص قد تم إعداده من قبل مضيف المختبر المعتمد (ALH) الذي يوفر بيئة المختبر. ولكن لأغراض العرض التوضيحي، من الجيد عرض الأدوار المحددة لـ Sentinel.  أغلق نافذة assignments بتحديد **X** في الزاوية العلوية اليمنى من النافذة.

    1. من صفحة التحكم في الوصول، حدد **+ إضافة**، ثم حدد **إضافة تعيين دور**.

    1. تفتح نافذة إضافة تعيين دور.  في مربع البحث، أدخل **Microsoft Sentinel** لعرض الأدوار المرتبطة بـ Microsoft Sentinel.
    1. من أي من الأدوار المدرجة، حدد **view** لعرض تفاصيل هذا الدور.  كأفضل ممارسة، ينبغي لك تعيين الامتياز الأقل طلبًا بالنسبة للوظيفة.  

    1. أغلق هذه النافذة بتحديد **X** في الزاوية العلوية اليمنى من النافذة.

1. من صفحة access control، أغلق النافذة بتحديد **X** في الزاوية العلوية اليمنى من النافذة.

### العرض التوضيحي - الجزء 3

في هذا الجزء من العرض التوضيحي، ستعرض خطوات الاتصال بمصدر بيانات. يتم نشر العديد من موصلات البيانات كجزء من حل Microsoft Sentinel، جنبًا إلى جنب مع قواعد التحليلات ذات الصلة والمصنفات ودلائل المبادئ. مركز محتوى Microsoft Sentinel هو الموقع المركزي لاكتشاف المحتوى الجاهز (المدمج) وإدارته. في هذه الخطوة، ستستخدم مركز المحتوى لنشر حل Microsoft Defender for Cloud لـ Microsoft Sentinel.  يسمح لك هذا الحل باستيعاب تنبيهات الأمان التي تم الإبلاغ عنها في Microsoft Defender for Cloud.

1. افتح علامة تبويب المستعرض لـ Microsoft Sentinel.

1. من لوحة التنقل اليسرى، حدد **مركز المحتوى**.

1. خصص بعض الوقت للتمرير لأسفل لرؤية القائمة الطويلة للحلول المتاحة وخيارات تصفية القائمة.  بالنسبة لهذه المهمة، أنت تبحث عن **Microsoft Defender for Cloud**.  حدده من القائمة.  في النافذة الجانبية التي تنفتح، اقرأ الوصف ثم حدد **تثبيت**.  بمجرد اكتمال التثبيت، سيظهر عمود الحالة في النافذة الرئيسية على أنه مثبت.

1. على الجانب الأيسر من صفحة Microsoft Defender for Cloud يوجد الوصف والملاحظات المقترنة بالحل من مركز المحتوى وما هو مضمن بوصفه جزءاً من هذا الحل.  في النافذة الرئيسية، توجد مكونات الحل.  في هذه الحالة هناك موصلان للبيانات وقاعدة بيانات واحدة. يشير المثلث البرتقالي إلى أن هناك حاجة إلى بعض التكوين. حدد المربع المجاور للمكان الذي يشير فيه إلى **Microsoft Defender for Cloud (قديم) القائم على الاشتراك**.  يتم فتح نافذة على الجانب الأيمن من الصفحة.  حدد **فتح صفحة الموصل**.

1. لاحظ تعليمات التكوين  حدد المربع بجوار اسم الاشتراك ثم حدد **اتصال**.  ستغير الحالة إلى متصل.  تم تمكين الموصل الآن، على الرغم من أن الأمر قد يستغرق بعض الوقت حتى يظهر الموصل في صفحة موصلات البيانات.  

1. الآن، اعرض معلومات حول قاعدة التحليلات.  من أعلى الصفحة (في مسار التنقل) حدد **Microsoft Defender for Cloud**. ألغِ تحديد المربع بجوار المكان الذي يظهر فيه Microsoft Defender for Cloud، حيث قمت بالفعل بتكوين الموصل (قد يستغرق الأمر بعض الوقت حتى تختفي أيقونة التحذير). حدد المربع الموجود بجانب المكان الذي تظهر فيه جملة، **الكشف عن نشاط حذف CoreBackUp من تنبيهات الأمان ذات الصلة**.  يؤدي ذلك إلى ظهور صفحة قواعد التحليلات.  مرة أخرى، حدد اكتشاف **نشاط الحذف CoreBackUp من قاعدة التنبيهات الأمنية** ذات الصلة. نافذة تفتح على اليسار توفر معلومات حول القاعدة وما تفعله.  حدد **إنشاء قاعدة**.  
    1. على الرغم من أن تفاصيل منطق القاعدة تقع خارج نطاق الأساسيات، اطلع على كل علامة تبويب في إنشاء القاعدة لعرض نوع المعلومات التي يمكن تكوينها
    1. عند الوصول إلى علامة التبويب مراجعة + إنشاء، حدد **حفظ**.

1. ارجع إلى صفحة Sentinel عن طريق تحديد **Microsoft Sentinel | مركز المحتوى** من مسار التنقل في أعلى الصفحة، حيث تُذكر جملة قواعد Analytics.

1. أوضح أنه باستخدام مركز المحتوى، يمكن نشر الحل بسهولة وسرعة.

1. اترك هذه الصفحة مفتوحة، لأننا ستستخدمها في المهمة التالية.

### العرض التوضيحي - الجزء 4

في هذا الجزء من العرض التوضيحي، سوف تعرض بعض الخيارات المتوفرة في Sentinel.

1. من لوحة التنقل إلى اليسار، حدد **Hunting**.  من أعلى الصفحة، حدد علامة تبويب **الاستعلامات**. اقرأ وصف استعلام التتبع. يمكن إضافة استعلامات التتبع من خلال مركز المحتوى. وسيتم سرد أي استعلامات تم تثبيتها مسبقًا هنا. حدد **الانتقال إلى مركز المحتوى**.  مركز المحتوى يسرد المحتوى الذي يتضمن الاستعلامات إما كجزء من حل أو استعلام مستقل.  انتقل لأسفل لرؤية الخيارات المتاحة.

1. من لوحة التنقل إلى اليسار، حدد **MITRE ATT&CK**.  MITRE ATT&CK هي قاعدة معارف متاحة للجمهور من الأساليب والتقنيات التي يشيع استخدامها من قبل المهاجمين. باستخدام Microsoft Sentinel، يمكنك عرض الاكتشافات النشطة بالفعل في مساحة العمل لديك، وتلك المتوفرة لك لتكوينها، لفهم التغطية الأمنية لمؤسستك، استنادًا إلى الأساليب والتقنيات من إطار عمل MITRE ATT&CK®.  حدد أي خلية من المصفوفة ولاحظ المعلومات المتوفرة على الجانب الأيمن من الشاشة.  

1. من لوحة التنقل إلى اليسار، حدد **Community**. تتضمن صفحة المجتمع نتائج تحليلات الأمان عبر الإنترنت من Microsoft Research وتحديثاته، وارتباطاً إلى قائمة مدونات Microsoft Sentinel، وارتباطاً إلى منتديات Microsoft Sentinel، وارتباطات أحدث الإصدارات إلى مركز Microsoft Sentinel والمزيد. استكشف هذه متى تشاء.

1. من جزء التنقّل الأيسر، حدد **التحليلات**.  يجب أن تكون هناك قاعدتان نشطتان، واحدة متوفرة بشكل افتراضي والقاعدة التي قمت بإنشائها في المهمة السابقة. حدد القاعدة الافتراضية: **اكتشاف الهجوم المتقدم متعدد المراحل**.  راجع المعلومات التفصيلية.  Microsoft Sentinel يستخدم Fusion، وهو محرك ارتباط يعتمد على خوارزميات التعلم الآلي القابلة للتطوير، للكشف تلقائيًا عن الهجمات متعددة المراحل (المعروفة أيضًا باسم التهديدات المستمرة المتقدمة) من خلال تحديد مجموعات من السلوكيات المخالفة للطبيعة والأنشطة المشبوهة التي تتم ملاحظتها في مراحل مختلفة من سلسلة القتل. على أساس هذه الاكتشافات، ينشئ Microsoft Sentinel أحداث كان من الصعب التقاطها لولا ذلك.

1. من جزء التنقّل الأيسر، حدد **الأتمتة**.  هنا يمكنك إنشاء قواعد تشغيل تلقائي ببساطة، أو التكامل مع دلائل المبادئ الحالية، أو إنشاء دلائل مبادئ جديدة.  حدد **+ Create** ثم حدد **Automation rule**.  لاحظ النافذة التي تفتح على الجانب الأيمن من الشاشة والخيارات المتاحة لإنشاء الشروط والإجراءات.  حدد **Cancel** من أسفل الصفحة.

1. من جزء التنقّل الأيسر، حدد **المصنفات**. اقرأ وصف مصنف Microsoft Sentinel.  يمكن إضافة المصنفات من خلال مركز المحتوى. وسيتم إدراج أي مصنفات تم تثبيتها مسبقًا هنا. حدد **الانتقال إلى مركز المحتوى**.  مركز المحتوى يسرد المحتوى الذي يتضمن المصنفات إما كجزء من حل أو كمصنف مستقل. انتقل لأسفل لرؤية الخيارات المتاحة.

1. أغلق هذه النافذة بتحديد **X** في الزاوية العلوية اليمنى من النافذة.

1. من الزاوية العلوية إلى اليسار من النافذة، أسفل الشريط الأزرق مباشرة، حدد **Home** للعودة إلى الصفحة الرئيسية لمدخل Azure.  

### المراجعة

في هذا العرض التوضيحي، استعرضت خطوات توصيل Microsoft Sentinel بمصادر البيانات، وقمت بإعداد مصنف، واستعرضت العديد من الخيارات المتوفرة في Microsoft Sentinel.

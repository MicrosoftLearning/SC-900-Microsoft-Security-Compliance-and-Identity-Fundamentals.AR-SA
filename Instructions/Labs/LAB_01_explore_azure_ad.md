---
lab:
  title: استكشاف إعدادات مستخدم Microsoft Entra ID
  module: Describe the function and identity types of Microsoft Entra ID
---

# نشاط معملي: استكشاف إعدادات مستخدم Microsoft Entra ID

يقوم هذا النشاط المعملي بتعيين محتوى Learn التالي:

- مسار التعلم: وصف قدرات Microsoft Entra،
- الوحدة النمطية: وصف أنواع الدالة والهوية لمعرف Microsoft Entra.
- الوحدة: وصف أنواع الهويات.

## سيناريو النشاط المعملي

في هذا النشاط المعملي، ستصل إلى معرف Microsoft Entra (يشار إليه سابقا باسم Azure Active Directory).  بالإضافة إلى ذلك، ستتولى إنشاء مستخدم وتكوين الإعدادات المختلفة، بما في ذلك إضافة التراخيص.  

**الوقت المقدر:** 30 دقيقة

### المهمة 1

بصفتك مشتركا في Microsoft 365، فأنت تستخدم معرف Microsoft Entra بالفعل.  في هذه المهمة، ستتعلم كيفية إنشاء مستخدم جديد في معرف Microsoft Entra واستكشاف بعض الخدمات التي يمكن إدارتها على مستوى المستخدم.

1. فتح مستعرض Microsoft Edge . في شريط العناوين، أدخل **`https://admin.microsoft.com`** وسجل الدخول باستخدام بيانات اعتماد Microsoft 365 التي يوفرها مضيف المختبر المعتمد (ALH).
    1. في نافذة تسجيل الدخول، أدخل **admin@WWLxZZZZZZ.onmicrosoft.com** (حيث يعد ZZZZZZ هو معرّف حساب المستأجر الفريد الذي يوفره مضيف النشاط المعملي المعتمد (ALH)) ثم حدد **التالي**.
    1. أدخل كلمة مرور المسؤول التي يجب أن يوفرها موفر استضافة النشاط المعملي الخاص بك. حدد **تسجيل الدخول**.
    1. اعتمادا على مضيف المختبر الخاص بك وإذا كانت هذه هي المرة الأولى التي تقوم فيها بتسجيل الدخول إلى المستأجر، فقد تتم مطالبتك بإكمال عملية تسجيل المصادقة متعددة العوامل. إذا كان الأمر كذلك، فاتبع المطالبات على الشاشة لإعداد المصادقة متعددة العوامل.
    1. بمجرد تسجيل الدخول، يتم نقلك إلى صفحة مركز مسؤولي Microsoft 365.

1. ضمن مراكز مسؤول، حدد **الهوية** (قد تحتاج إلى تحديد **عرض الكل** والتمرير لأسفل).  يتم فتح صفحة مستعرض جديدة على صفحة النظرة العامة لمركز إدارة Microsoft Entra.

1. من جزء التنقل الأيسر، قم بتوسيع **المستخدمون** ثم حدد **كل المستخدمين**. لاحظ أن حساب المستأجر قد تم تكوينه بالفعل مع المستخدمين.

1. من أعلى الصفحة، حدد **+ New user** ثم من المربع المنسدل، حدد **Create new user**.

1. أنت الآن في علامة تبويب **الأساسيات** في صفحة إنشاء مستخدم جديد. احرص على تعبئة الحقول كما يلي:
    1. اسم المستخدم الرئيسي: **سارا**.

    1. اسم مستعار للبريد: اترك الاسم الافتراضي، الذي تم تعيينه إلى مشتق من اسم المستخدم الأساسي.

    1. اسم العرض: **Sara Perez**.

    1. كلمة المرور: احرص على إلغاء تحديد المربع الذي يشير إلى إنشاء كلمة مرور تلقائيا وأدخل كلمة مرور مؤقتة تلتزم بمتطلبات كلمة المرور ودوّنها، حيث ستحتاج إليها لإكمال المهمة اللاحقة.

    1. تمكين الحساب: اترك علامة الاختيار للتأكد من تمكين الحساب.

    1. في أسفل الصفحة، حدد **التالي: خصائص**.

1. هنا ستتولى تكوين عدد قليل من الحقول في علامة تبويب **خصائص**.

    1. الاسم الأول: سارة

    1. اسم العائلة: بيريز

    1. أنواع المستخدمين: اترك الإعداد الافتراضي **للعضو**، ولكن لاحظ أنه من القائمة المنسدلة لديك خيار تحديد الضيف.

    1. موقع الاستخدام: اختر البلد/المنطقة التي تتواجد فيها.  لاحظ أنه للوصول إلى حقل موقع الاستخدام، ستحتاج إلى التمرير لأسفل على الصفحة لأنه الحقل الأخير على الصفحة.  **ملاحظة**: إذا لم تفعل ذلك، فلن تتمكن من تعيين ترخيص في خطوة لاحقة.

    1. حدد **التالي: التعيينات**.

1. أنت الآن في علامة تبويب **التعيينات** حيث تقوم بإضافة تعيين مجموعة وعرض الخيارات المتوفرة لإضافة دور.

    1. حدد **إضافة مجموعة**.

    1. تعرض النافذة التي تفتح جميع المجموعات المتوفرة.  

    1. لاحظ قائمة المجموعات المتاحة.  من القائمة، حدد **العمليات**.  في الجزء السفلي من الصفحة، حدد زر **تحديد**.  قد يستغرق الأمر بضع ثوان ولكن ينبغي أن تشاهد مجموعة العمليات تظهر على صفحة التعيينات.

    1. من أعلى الصفحة، حدد **+ إضافة دور**.  تفتح نافذة تعرض جميع أدوار الدليل المتوفرة.  اعرض الخيارات المتوفرة، ولكن لا تُضِف أي أدوار جديدة.  أغلق هذه الصفحة عن طريق تحديد **X** في الزاوية اليمنى العليا من صفحة أدوار الدليل.
    1. من أسفل الصفحة، حدد **مراجعة + إنشاء**. سيتم عرض ملخص للإعدادات.  من أسفل الصفحة، حدد **Create**.

1. يتم إرجاعك إلى صفحة المستخدمين.  بعد بضع ثوان، سيتم إدراج Sara Perez.  قد تحتاج إلى تحديد أيقونة **تحديث** في أعلى الصفحة.

1. من قائمة المستخدمين، حدد المستخدم الذي أنشأته، **Sara Perez**.  تفتح صفحة **نظرة عامة**.

1. تعرض لوحة التنقل اليسرى الخيارات المختلفة التي يمكن تكوينها للمستخدم. عرض الخيارات المتاحة.

1. من لوحة التنقل اليسرى، حدد **التراخيص**.  لاحظ أنه لا توجد تعيينات ترخيص لهذا المستخدم، لاحظ أيضا رمز التحذير الذي يقول: "تتوفر إضافة تعيينات الترخيص وإزالتها وإعادة معالجتها فقط داخل مركز إدارة M365."  ستقوم بذلك في المهمة التالية.  ملاحظة: لا يمكن تعيين التراخيص إلا إذا تم تكوين موقع استخدام. إذا لم تقم بتعيين موقع الاستخدام، فارجع إلى هذه الخطوة الآن.

### المهمة الثانية

في هذه المهمة، ستقوم بتعيين ترخيص للمستخدم الذي أنشأته للتو، باستخدام مركز مسؤولي Microsoft 365.

1. افتح علامة تبويب **المستعرض الصفحة الرئيسية - مركز مسؤولي Microsoft 365**.

1. من لوحة التنقل اليسرى، ضمن users، حدد **Active users**.  من قائمة المستخدمين، حدد **Sara Perez**.  تفتح نافذة تعرض معلومات حول المستخدم.  

    1. **حدد علامة التبويب التراخيص والتطبيقات**.
    1. لكل ترخيص من التراخيص المدرجة، سترى عدد التراخيص المتوفرة.  نظرا لعدم وجود تراخيص Microsoft 365 E5 متوفرة (تم تعيينها بالفعل لمستخدمين آخرين)، قم بتعيين **Microsoft Power Apps Developer** وتراخيص **Microsoft Power Automate Free** عن طريق تحديد خانة الاختيار بجوارها.
    1. حدد **حفظ التغييرات**. ينبغي أن يُظهر إشعار في الزاوية العلوية اليمنى من الشاشة أن تعيينات الترخيص قد نجحت.
    1. أغلق الصفحة عن طريق تحديد **X** في الزاوية العلوية اليسرى من الصفحة.

1. ارجع إلى مركز مسؤولي Microsoft Entra عن طريق تحديد **الصفحة الرئيسية** من لوحة التنقل اليسرى أو من الجزء العلوي الأيسر من الشاشة (كسرة الخبز)، أعلاه حيث تقول Sara Perez | التراخيص.

1. لقد قمت بتعيين تراخيص للمستخدم بنجاح.

1. سجل الخروج من جميع علامات تبويب المستعرض المفتوحة. سجّل الخروج عن طريق تحديد أيقونة المستخدم بجوار عنوان البريد الإلكتروني في الزاوية اليمنى العليا من الشاشة ثم تحديد **تسجيل الخروج**. أغلق جميع نوافذ المستعرض.

### المهمة الثالثة

في هذه المهمة، ستتولى تسجيل الدخول باسم Sara Perez، لأول مرة.

1. افتح مستعرض Microsoft Edge.

1. في شريط العناوين، أدخِل **https://login.microsoft.com**.

1. تسجيل الدخول باسم **sara@WWLxZZZZZ.onmicrosoft.com**، (حيث يعد ZZZZZZ هو معرف حساب المستأجر الفريد الذي يوفره مضيف النشاط المعملي المعتمد)
1. أدخل كلمة المرور المؤقتة التي سجلتها من المهمة السابقة وحدد تسجيل الدخول.

1. يُطلب منك الآن تحديث كلمة المرور . في حقل كلمة المرور الحالية، أدخل كلمة المرور المؤقتة من المهمة السابقة.

1. في الحقل كلمة مرور جديدة، أدخل كلمة مرور جديدة، وتأكد من كلمة المرور، ثم حدد **تسجيل الدخول**.  دوّن كلمة المرور الجديدة حيث ستحتاج إليها للنشاط المعملي اللاحق على SSPR.

1. نظرا لأن هذه هي المرة الأولى التي تقوم فيها بتسجيل الدخول باسم Sara Perez، فقد تتم مطالبتك بإعداد المصادقة متعددة العوامل. اتبع المطالبات التي تظهر على الشاشة لإعداد المصادقة متعددة العوامل.

1. يجب أن يتم الآن تسجيل الدخول بنجاح إلى حساب Microsoft الخاص ب Sara.  لاحظ أن ترخيص Sara الذي قمت بتعيينه في المهمة السابقة كان يقتصر فقط على Power Automate Free وPower Apps for Developer ولم يتضمن ترخيص E5.

1. سجّل الخروج عن طريق تحديد الأيقونة الموجودة في الزاوية العلوية اليمنى من نافذة Microsoft 365 التي تظهر كدائرة مع الأحرف SP (بجوار أيقونة علامة الاستفهام)، ثم تحديد **Sign out**، ثم أغلق المستعرض.

### المراجعة

في هذا النشاط المعملي، بدأت استكشافك الأولي لدليل Microsoft Entra ID. نظراً لأن المشتركين في Microsoft 365 يستخدمون Microsoft Entra ID تلقائياً، فقد رأيت أنه يمكنك الوصول إلى ميزات Microsoft Entra ID وخدماته من خلال مدخل مسؤولي Microsoft 365 أو من خلال مدخل Azure.  أيًا كان النهج الذي تفضله للوصول إلى نفس المكان.  استعرضت أيضًا عملية إنشاء مستخدم جديد والإعدادات المختلفة التي يمكن تكوينها، بما يشمل المجموعات التي يمكن تعيين المستخدم لها، وتوفر الأدوار، وتعيين تراخيص المستخدم.

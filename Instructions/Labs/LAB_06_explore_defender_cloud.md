---
lab:
  title: استكشاف Microsoft Defender for Cloud
  module: 'Module 3 Lesson 2: Describe the capabilities of Microsoft security solutions: Describe security management capabilities of Azure'
ms.openlocfilehash: 208e11a7e82497fbb900b4fa024fb6fb367d458e
ms.sourcegitcommit: a341c2fc38e9b37dafb792d82e3c948f7ba4a099
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/14/2022
ms.locfileid: "137893681"
---
# <a name="lab-explore-microsoft-defender-for-cloud"></a>نشاط معملي: استكشاف Microsoft Defender for Cloud

## <a name="lab-scenario"></a>سيناريو النشاط المعملي
في هذا النشاط المعملي، ستستكشف Microsoft Defender for Cloud وتتعلم كيف يمكن استخدام Azure Secure Score لتحسين وضع أمان المؤسسة.

**الزمن المقدر**: 30 دقيقة

#### <a name="task-1-in-this-task-you-will-take-a-brief-tour-of-microsoft-defender-for-cloud"></a>المهمة 1: في هذه المهمة، ستأخذ جولة قصيرة في Microsoft Defender for Cloud.
1.  افتح مستعرض Microsoft Edge. في شريط العناوين، أدخل **portal.azure.com.**

1. سجل الدخول باستخدام بيانات اعتماد المسؤول خاصتك.
    1. في نافذة تسجيل الدخول، أدخل **admin@WWLxZZZZZZ.onmicrosoft.com** (حيث يعد ZZZZZZ هو معرّف المستأجر الفريد الذي يوفره موفّر استضافة نشاطك المعملي) ثم حدد **Next**.
    1. أدخل كلمة مرور المسؤول التي يجب أن يوفرها موفر استضافة النشاط المعملي خاصتك. حدد **"Sign in"**.
    1. عند مطالبتك بالبقاء مسجلاً للدخول، حدد **نعم**.

1. ِفي الزاوية اليسرى العليا من الشاشة، بجوار المكان الذي تظهر فيه Microsoft Azure، حدد رمز Show portal menu (الخطوط الأفقية الثلاثة المشار إليها أيضًا برمز على شكل هامبرغر) ثم من لوحة التنقل اليسرى، ضمن Favorites، حدد **Microsoft Defender for Cloud**.  إذا لم يتم إدراجها ضمن favorites، ففي مربع البحث، أدخل **Microsoft Defender for Cloud**، ثم من قائمة النتائج، حدد **Microsoft Defender for Cloud**.

1. لاحظ المعلومات المتوفرة في صفحة Microsoft Defender for Cloud overview.  

1. ربما ترى مربع معلومات أزرق أعلى الصفحة يشير إلى أنك ربما تستعرض معلومات محدودة.  حدد **انقر هنا**.
    1. لضمان حصولك على رؤية شاملة للمستأجر، خصص لنفسك الدور اللازم.  حدد **مسؤول الأمان**، ثم حدد **الحصول على وصول** في أسفل الصفحة.
    1. من المحتمل أن ترى الرسالة؛ مجموعة إدارة الجذر غير موجودة.  حسب الوصف، سيقوم النظام بإنشاء المجموعة لك.  قد يستغرق الأمر ما يصل إلى 15 دقيقة لإكماله (ولكن عادة ما يحدث بشكل أسرع).  بمجرد منح الوصول حدد **Microsoft Defender for Cloud** في الزاوية العلوية اليسرى من الصفحة، أعلاه حيث تظهر عبارة Get permissions ثم قم بتحديث صفحة Microsoft Defender for Cloud overview.

1. تتضمن المعلومات الموجودة أعلى الصفحة عدد اشتراكات Azure وعدد الموارد التي تم تقييمها وعدد التوصيات النشطة وأي تنبيهات أمان.  توجد في الجزء الرئيسي من الصفحة بطاقات تمثل درجة الأمان والتوافق التنظيمي ونتائج التحليلات والمزيد.  

1. من أعلى الصفحة، حدد **الموارد المقيّمة**.  (لاحظ أن هذا يعادل تحديد Inventory من لوحة التنقل اليسرى لصفحة Microsoft Defender for Cloud الرئيسية).
    1. ينقلك هذا إلى صفحة **المخزون** التي تعرض اشتراك Azure Pass خاصتك.  **حدد Azure Pass - وصول محدود**.
    1. توفر صفحة سلامة الموارد قائمة بالتوصيات.  من القائمة المتاحة، حدد **يجب أن يكون هناك أكثر من مالك معيَّن لاشتراكك.**
    1. حدد سهم القائمة المنسدلة بجوار خطوات المعالجة. لاحظ كيف يتم توفير خطوات المعالجة التفصيلية إلى جانب خيار اتخاذ الإجراء.  
    1. حدد **Microsoft Defender for Cloud** من الزاوية العلوية اليسرى من الشاشة للعودة إلى صفحة Microsoft Defender for Cloud overview.

1. من أعلى الصفحة، حدد **التوصيات النشطة**.  (لاحظ أن هذا يعادل تحديد Recommendations من لوحة التنقل اليسرى لصفحة Microsoft Defender for Cloud الرئيسية).
    1. تعرض صفحة التوصيات لوحة معلومات "درجة الأمان" خاصتك.
    1. يوجد أسفل لوحة معلومات "درجة الأمان" قائمة من عناصر التحكم. يمثل كل عنصر تحكم أمان خطرًا أمنيًا يجب تخفيفه ويتضمن أيضًا معلومات حول الحد الأقصى للدرجات المرتبطة بعنصر التحكم، والنتيجة الحالية، وزيادة الدرجة المحتملة، وحالة سلامة الموارد.  
    1. حدد أحد عناصر التحكم، مثل **تمكين MFA**.  حدد أحد العناصر الفرعية، مثل **يجب تمكين MFA على الحسابات ذات أذونات المالك في اشتراكك**.  في الصفحة التي تفتح، سترى وصفًا وخطوات "المعالجة" والموارد المتأثرة. اخرج من هذه الصفحة، عن طريق تحديد **X** في الزاوية العلوية اليمنى من الشاشة.
    1. اخرج من صفحة التوصيات عن طريق تحديد **X** في الزاوية العلوية اليمنى من الشاشة، للعودة إلى صفحة النظرة العامة.

1. من الصفحة الرئيسية، حدد **التوافق التنظيمي**. توفر صفحة التوافق التنظيمي قائمة بضوابط التوافق.  تحت كل عنصر تحكم، توجد مجموعة من التقييمات التي تستند إلى Azure Security Benchmark الذي يوفر توصيات حول كيفية تأمين حلول السحابة خاصتك على Azure.
    1. حدد **IM. Identity Management** ثم حدد **IM-6 Use strong authentication controls**.  تعرض القائمة إجراءات مسؤولية العميل التي يمكن اتخاذها لتحسين وضع التوافق.
    1. حدد **X** في الزاوية العلوية اليمنى من الشاشة لإغلاق الصفحة والعودة إلى صفحة Microsoft Defender for Cloud overview. 
    1. إبقاء صفحة Microsoft Defender for Cloud overview مفتوحة، سوف تستخدمها في المهمة التالية.


#### <a name="task-2-in-this-task-you-will-navigate-to-azure-secure-score-and-explore-recommendations-that-can-improve-your-secure-score"></a>المهمة 2: في هذه المهمة، سوف تنتقل إلى Azure Secure Score وتستكشف التوصيات التي يمكن أن تحسن درجات الأمان خاصتك. 

1. من صفحة Microsoft Defender for Cloud overview، حدد بطاقة **Secure Score**.
1. **حدد Azure Pass - وصول محدود**.  لاحظ درجة الأمان خاصتك.
1. من صفحة التوصيات، حدد **Implement security best practices** للتوسع في القائمة. لاحظ أن هذا يظهر الحالة الصحية للمورد باللون الأحمر.
1. حدد العنصر **يجب أن يكون هناك أكثر من مالك معين لاشتراكك**، الذي يعرض حالة سلامة المورد باللون الأحمر. 
1. أسفل حيث يظهر **Affected resources**، تأكد من تحديد/التسطير أسفل Unhealthy resources، ثم حدد Azure subscription المدرجة.
1. من أعلى صفحة التحكم بالوصول (IAM)، حدد **+ إضافة** ثم من القائمة المنسدلة حدد **إضافة تعيين دور**.
    1. من الجانب الأيسر من الصفحة، حدد **Owner** (يجب أن يكون هذا العنصر الأول مدرجًا) بحيث يتم تمييز الصف باللون الرمادي، ثم حدد **Next** من أسفل الصفحة.
    1. بجوار المكان الذي يظهر Members، حدد **+ Select members**. 
    1. من نافذة Select members التي تفتح على الجانب الأيمن من الشاشة، حدد **Alex Wilber**، ثم اضغط على **Select** أسفل الصفحة.  
    1. من صفحة Add role assignment، تحقق من إدراج Alex Wilber كعضو، ثم حدد **Next** متبوعًا بـ **Review + assign**.
    1. قد يستغرق تحديث الحالة ما يصل إلى 24 ساعة، وبعد ذلك سيتم أيضًا تحديث درجات الأمان خاصتك حيث يتم استيفاء جميع العناصر الموجودة في مجموعة إدارة الوصول والأذونات.
    1. من أعلى يسار الصفحة، أعلى حيث يظهر Azure Pass، حدد **Microsoft Defender for Cloud** لإرجاع صفحة Microsoft Defender for Cloud overview.
1. اترك هذه الصفحة مفتوحة للمهمة التالية.


#### <a name="task-3--recall-that-microsoft-defender-for-cloud-is-offered-in-two-modes-without-enhanced-security-features-free-and-with-enhanced-security-features-which-are-available-through-the-microsoft-defender-for-cloud-plans-in-this-task-you-discover-how-to-enabledisable-the-various-microsoft-defender-for-cloud-plans"></a>المهمة 3:  تذكر أن Microsoft Defender for Cloud يتم تقديمه في وضعين: بدون ميزات أمان محسنة (مجانية) ومع ميزات أمان محسنة متوفرة من خلال خطط Microsoft Defender for Cloud. في هذه المهمة تكتشف كيفية تمكين/تعطيل خطط متعددة لـ Microsoft Defender for Cloud.

1.  من صفحة Microsoft Defender for Cloud overview، حدد **Environment settings** من لوحة التنقل اليسرى.
1. حدد علامة أكبر من **>** بجانب المكان الذي يظهر Tenant Root Group لتوسيعه (لا تحدد Tenant Root Group مباشرة لأن ذلك سوف يوجهك إلى صفحة مختلفة)، ثم حدد **Azure Pass - Sponsorship**
1.  في الصفحة Defender plans، لاحظ كيف يمكنك تحديد خطة Enable all أو تحديد خطة individual Defender. اترك الإعدادات كما هي مع تعيين كافة الخطط إلى off.
1.  يمكنك الآن إغلاق علامة تبويب المستعرض للخروج من مدخل Azure.


#### <a name="review"></a>مراجعة
في هذا النشاط المعملي، قد استكشفت Microsoft Defender for Cloud وتعلمت كيف يمكن استخدام Azure Secure Score لتحسين وضع أمان المؤسسة.


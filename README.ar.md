<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="تطبيق سطح المكتب FarmPanel، شاشة الحسابات: شريط تنقّل جانبي (Dashboard وAccounts وWorkflows وMonitoring وSandboxes وServers وMatchmaking وLobby وLogs) وجدول حسابات بأعمدة الحالة واسم الدخول والاسم المستعار وسير العمل والصندوق المعزول وآخر تسجيل دخول"/>

<br/>

# FARMPANEL

**لوحة إدارة مزرعة حسابات Steam وCS2 — تنسيق تعدّد الحسابات على Windows**

`تشغيل · عزل · مراقبة · استعادة`

FarmPanel هي لوحة سطح المكتب على Windows لتشغيل **مزرعة حسابات Steam** على
نطاق واسع. فهي تُشغّل كل **حساب CS2** في مزرعتك وتعزله داخل صندوق معزول
وتراقبه وتعيد تشغيله تلقائيًا — من خمسة حسابات إلى بضع مئات — من نافذة واحدة،
دون أي زراعة آلية ودون أي بوتات.

[**التنزيل لنظام Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[الموقع](https://farmpanel.cc) ·
[المنتج](https://farmpanel.cc/ar/product) ·
[Telegram](https://t.me/farmpanel_ar)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__ar-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_ar)

متوفر أيضًا باللغات: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md)

</div>

---

## ما هو FarmPanel

إذا كنت تُدير أكثر من حساب Steam واحد، فأنت تعرف هذا الروتين جيدًا: عشرات
النوافذ مفتوحة في آن واحد، وعميل CS2 تعطّل ويجب أن تنتبه إليه وتُعيد تشغيله
يدويًا، ولا توجد طريقة واضحة لمعرفة من عَلِق في شاشة التحميل ومن دخل المباراة
بالفعل. وكلّما زاد عدد الحسابات في مزرعتك، ازدادت هذه المهمة إرهاقًا.

**FarmPanel هي لوحة إدارة مزرعة حسابات Steam وCS2 صُمّمت خصّيصًا لإزالة هذا
العناء تمامًا.** إنه تطبيق سطح مكتب على Windows يُشغّل مزرعة متعدّدة الحسابات
بالكامل ويعزلها ويراقبها من نافذة واحدة — بديل حقيقي عن إدارة حسابات Steam
المتعدّدة يدويًا، أو التعامل مع خليط من السكربتات والأجهزة الافتراضية.

FarmPanel **ليس بوت زراعة آلية**. فهو لا يلعب نيابةً عنك ولا يُحاكي أفعال
داخل اللعبة — بل يُدير كل ما يجري *حول* اللعبة: تشغيل العملاء، وإرسال دعوات
اللوبي، واستعادة الجلسات المتعطّلة، ومنحك رؤية مباشرة لكل حساب. تبقى كل أفعال
اللعب داخل اللعبة بيد شخص حقيقي، فتتصرّف مزرعتك — وتبدو — مثل لاعبين حقيقيين،
لأنها كذلك فعلًا.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## لماذا يختار أصحاب المزارع FarmPanel

**01 — لا زراعة آلية على الإطلاق.**
FarmPanel لا يلعب نيابةً عنك أبدًا. كل فعل داخل اللعبة يتم يدويًا، فتبدو
الحسابات بشرية، لأنها كذلك.

**02 — اضبطه مرّة واحدة.**
كل تشغيل وكل تسجيل دخول يتبع التسلسل الحتمي نفسه. ما نجح بالأمس ينجح غدًا،
دون مفاجآت.

**03 — الأعطال تُصلح نفسها.**
إذا تعطّل Steam أو CS2، يلاحظ FarmPanel ذلك ويُعيده خلال ثوانٍ، دون تدخّل منك.

**04 — عزل حقيقي داخل الصناديق المعزولة.**
كل حساب يعمل في بيئته المعزولة الخاصة — لا جلسات مشتركة، ولا ملفات مشتركة،
ولا اختلاط للبصمات بين الحسابات.

**05 — كلمات المرور لا تغادر جهازك أبدًا.**
تُشفَّر بيانات الاعتماد بأمان Windows المدمج وتُخزَّن على جهازك فقط، ولا تُرسَل
إلى أي مكان.

**06 — رؤية مباشرة لكل حساب.**
لوحة معلومات فورية لكل حساب: الحالة، وحالة المباراة، ومدّة التشغيل. لا مجال
للتخمين بشأن ما تفعله المزرعة.

**07 — توجيه شبكي لكل حساب.**
اختر أفضل منطقة خادم لكل حساب؛ ويتولّى FarmPanel إعداد الشبكة نيابةً عنك.

**08 — ينمو مع مزرعتك.**
ابدأ بخمسة حسابات وتوسّع إلى المئات. اللوحة نفسها، وسير العمل نفسه، من البداية
إلى النهاية.

## كيف تبدأ

1. نزّل المُثبِّت — **[التنزيل لنظام Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   بالأعلى، أو من صفحة [Releases](https://github.com/leryqq/farmpanel-releases/releases) في هذا المستودع.
2. شغّل `Setup.exe`. يفحص FarmPanel نظامك ويرشدك خطوة بخطوة خلال الإعداد.
3. أضِف حسابات Steam الخاصة بك وشغّل مزرعتك الأولى.

```
المتطلبات:    Windows 10/11 (64-bit) · .NET 8
المُوصى به:    ذاكرة 32 غيغابايت · SSD · 16-32 حساب CS2 في آن واحد
التحديثات:    تلقائية، من هذا المستودع
```

## الأسئلة الشائعة

**هل يلعب FarmPanel نيابةً عني؟**
لا — وهذا هو بيت القصيد. لا بوتات ولا زراعة آلية. يُدير FarmPanel الحسابات:
التشغيل، والمراقبة، وتكوين اللوبيات، وإصلاح الأعطال. أما كل ما يجري داخل
اللعبة فتفعله أنت، فتتصرّف حساباتك مثل لاعبين حقيقيين، لأنها كذلك.

**أين تُخزَّن كلمات المرور الخاصة بي؟**
على جهازك فقط. تُشفَّر بأمان Windows المدمج، ولا تُخزَّن أبدًا كنصّ صريح،
ولا تُرسَل إلى أي مكان.

**هل يدعم CS2 فقط؟**
يحظى CS2 اليوم بأعمق دعم، بما في ذلك بيانات المباراة الحيّة. وألعاب أخرى في
الطريق.

**كم تبلغ التكلفة؟**
يعتمد السعر على حجم المزرعة. [راسلنا على Telegram](https://t.me/farmpanel_ar)
وسنُلائم خطّة مع إعدادك — من التكوينات الصغيرة إلى مئات الحسابات.

مزيد من الإجابات في [الأسئلة الشائعة للمنتج](https://farmpanel.cc/ar/product#faq).

## الأدلّة والموارد

- [كيفية تشغيل عدّة حسابات Steam بأمان](https://farmpanel.cc/ar/guides/run-multiple-steam-accounts-safely)
- [شرح عزل حسابات Steam داخل الصناديق المعزولة](https://farmpanel.cc/ar/guides/steam-account-sandboxing)
- [كم عدد حسابات CS2 التي يستطيع جهاز واحد تشغيلها؟](https://farmpanel.cc/ar/guides/how-many-cs2-accounts-per-pc)
- [شرح الإسقاط الأسبوعي في CS2](https://farmpanel.cc/ar/guides/cs2-weekly-drop-explained)
- [مخاطر حظر تعدّد الحسابات في CS2](https://farmpanel.cc/ar/guides/cs2-multi-account-ban-risks)
- [هل تحتاج إلى حسابات Prime لزراعة CS2؟](https://farmpanel.cc/ar/guides/prime-accounts-for-cs2-farming)
- [اقتصاديات زراعة الصناديق في CS2](https://farmpanel.cc/ar/guides/cs2-case-farming-economics)
- [بيع إسقاطات CS2 وسحب الأموال](https://farmpanel.cc/ar/guides/sell-cs2-drops-steam-market)
- [مزرعة CS2: يدويًا مقابل لوحة إدارة](https://farmpanel.cc/ar/compare/manual-multi-accounting)

## الروابط

| | |
| --- | --- |
| الموقع | [farmpanel.cc](https://farmpanel.cc) |
| المنتج | [farmpanel.cc/ar/product](https://farmpanel.cc/ar/product) |
| سجلّ التغييرات | [farmpanel.cc/ar/changelog](https://farmpanel.cc/ar/changelog) |
| Telegram | [t.me/farmpanel_ar](https://t.me/farmpanel_ar) |

---

<div align="center">

يوزّع هذا المستودع الملفات الثنائية الموقّعة لـ FarmPanel فقط.
الشيفرة المصدرية للتطبيق مملوكة ومغلقة.

`حالة النظام · جميع الأنظمة تعمل`

**FarmPanel Systems** · جميع الحقوق محفوظة

</div>

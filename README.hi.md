<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="FarmPanel डेस्कटॉप ऐप, Accounts स्क्रीन: साइडबार नेविगेशन (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) और स्टेटस, लॉगिन, निकनेम, वर्कफ़्लो, सैंडबॉक्स तथा अंतिम लॉगिन कॉलम वाला अकाउंट ग्रिड"/>

<br/>

# FARMPANEL

**Steam और CS2 अकाउंट फ़ार्म पैनल — Windows के लिए मल्टी-अकाउंट ऑर्केस्ट्रेशन**

`लॉन्च · आइसोलेट · मॉनिटर · रिकवर`

FarmPanel एक Windows डेस्कटॉप पैनल है जो बड़े पैमाने पर **Steam अकाउंट फ़ार्म**
चलाता है। यह आपके फ़ार्म के हर **CS2 अकाउंट** को — पाँच अकाउंट से लेकर कई सौ
तक — एक ही विंडो से लॉन्च करता है, सैंडबॉक्स में आइसोलेट करता है, निगरानी करता
है और अपने आप दोबारा शुरू करता है — बिना किसी ऑटोफ़ार्म और बिना किसी बॉट के।

[**Windows के लिए डाउनलोड करें**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[वेबसाइट](https://farmpanel.cc) ·
[उत्पाद](https://farmpanel.cc/hi/product) ·
[Telegram](https://t.me/farmpanel_hi)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__hi-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_hi)

अन्य भाषाओं में भी उपलब्ध: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## FarmPanel क्या है

अगर आप एक से ज़्यादा Steam अकाउंट चलाते हैं, तो यह रोज़मर्रा आपको पता ही है:
एक साथ दर्जन भर विंडो खुली रहती हैं, कोई CS2 क्लाइंट क्रैश हो जाता है जिसे आपको
ख़ुद देखकर हाथ से दोबारा खोलना पड़ता है, और यह जानने का कोई साफ़ तरीका नहीं होता
कि कौन लोडिंग पर अटका है और कौन पहले से मैच में है। फ़ार्म में जितने ज़्यादा
अकाउंट, यह काम उतना ही मुश्किल।

**FarmPanel एक Steam और CS2 अकाउंट फ़ार्म पैनल है जिसे ठीक इसी झंझट को हटाने के
लिए बनाया गया है।** यह एक Windows डेस्कटॉप ऐप्लिकेशन है जो पूरे मल्टी-अकाउंट
फ़ार्म को एक ही विंडो से लॉन्च, आइसोलेट और मॉनिटर करता है — Steam मल्टी-अकाउंट
को हाथ से चलाने या स्क्रिप्ट्स और वर्चुअल मशीनों के जुगाड़ से जूझने का एक असली
विकल्प।

FarmPanel कोई **ऑटोफ़ार्म बॉट नहीं है**। यह आपके लिए गेम नहीं खेलता और इन-गेम
क्रियाओं की नक़ल नहीं करता — यह गेम के *आस-पास* की हर चीज़ संभालता है:
क्लाइंट शुरू करना, लॉबी इनवाइट भेजना, क्रैश हुए सेशन रिकवर करना, और हर अकाउंट
पर लाइव निगरानी देना। गेम के अंदर की हर क्रिया एक असली इंसान के हाथ में रहती है,
इसलिए आपका फ़ार्म असली खिलाड़ियों जैसा व्यवहार करता है — और दिखता है — क्योंकि
वह है ही।

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## फ़ार्म मालिक FarmPanel क्यों चुनते हैं

**01 — कभी ऑटोफ़ार्म नहीं।**
FarmPanel कभी आपके लिए नहीं खेलता। हर इन-गेम क्रिया हाथ से होती है, इसलिए
अकाउंट इंसानी लगते हैं, क्योंकि वे हैं ही।

**02 — एक बार सेट करें।**
हर लॉन्च और लॉगिन वही निश्चित क्रम चलाता है। जो कल चला, वह कल भी चलेगा, बिना
किसी हैरानी के।

**03 — क्रैश ख़ुद ठीक हो जाते हैं।**
अगर Steam या CS2 बंद हो जाए, तो FarmPanel इसे भाँप लेता है और कुछ ही सेकंड में,
बिना निगरानी के, वापस चालू कर देता है।

**04 — असली सैंडबॉक्स आइसोलेशन।**
हर अकाउंट अपने अलग आइसोलेटेड माहौल में चलता है — न साझा सेशन, न साझा फ़ाइलें,
न अकाउंटों के बीच फ़िंगरप्रिंट का मेल।

**05 — पासवर्ड कभी आपके PC से बाहर नहीं जाते।**
क्रेडेंशियल Windows की बिल्ट-इन सुरक्षा से एन्क्रिप्ट होकर सिर्फ़ आपकी मशीन पर
रहते हैं, कहीं नहीं भेजे जाते।

**06 — हर अकाउंट पर लाइव निगरानी।**
हर अकाउंट के लिए रियल-टाइम डैशबोर्ड: स्टेटस, मैच की स्थिति, अपटाइम। फ़ार्म क्या
कर रहा है, इसका अंदाज़ा लगाने की ज़रूरत नहीं।

**07 — हर अकाउंट के लिए अलग नेटवर्क रूटिंग।**
हर अकाउंट के लिए सबसे अच्छा सर्वर क्षेत्र चुनें; नेटवर्क सेटअप FarmPanel आपके
लिए कर देता है।

**08 — आपके फ़ार्म के साथ बढ़ता है।**
पाँच अकाउंट से शुरू करें, सैकड़ों तक बढ़ाएँ। शुरू से आख़िर तक वही पैनल, वही
वर्कफ़्लो।

## शुरुआत कैसे करें

1. इंस्टॉलर डाउनलोड करें — ऊपर दिया **[Windows के लिए डाउनलोड करें](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   बटन, या इस रिपॉज़िटरी के [Releases](https://github.com/leryqq/farmpanel-releases/releases) पेज से।
2. `Setup.exe` चलाएँ। FarmPanel आपका सिस्टम जाँचता है और सेटअप में क़दम-दर-क़दम मार्गदर्शन करता है।
3. अपने Steam अकाउंट जोड़ें और अपना पहला फ़ार्म लॉन्च करें।

```
आवश्यकताएँ:   Windows 10/11 (64-bit) · .NET 8
अनुशंसित:     32 GB RAM · SSD · एक साथ 16-32 CS2 अकाउंट
अपडेट:        स्वचालित, इसी रिपॉज़िटरी से
```

## अक्सर पूछे जाने वाले सवाल

**क्या FarmPanel मेरे लिए गेम खेलता है?**
नहीं — यही तो पूरी बात है। कोई बॉट नहीं और कोई ऑटोफ़ार्म नहीं। FarmPanel
अकाउंट संभालता है: लॉन्च करना, निगरानी, लॉबी बनाना, क्रैश ठीक करना। गेम के अंदर
सब कुछ आप करते हैं, इसलिए आपके अकाउंट असली खिलाड़ियों जैसा व्यवहार करते हैं,
क्योंकि वे हैं ही।

**मेरे पासवर्ड कहाँ रखे जाते हैं?**
सिर्फ़ आपकी मशीन पर। वे Windows की बिल्ट-इन सुरक्षा से एन्क्रिप्ट होते हैं,
कभी सादे टेक्स्ट में नहीं रखे जाते, और कहीं नहीं भेजे जाते।

**क्या यह सिर्फ़ CS2 को सपोर्ट करता है?**
आज सबसे गहरा सपोर्ट CS2 का है, जिसमें लाइव मैच टेलीमेट्री भी शामिल है। और गेम
जल्द आ रहे हैं।

**इसकी कीमत क्या है?**
कीमत फ़ार्म के आकार पर निर्भर करती है। [Telegram पर हमें लिखें](https://t.me/farmpanel_hi)
और हम आपके सेटअप के हिसाब से प्लान चुनेंगे — छोटे कॉन्फ़िगरेशन से लेकर सैकड़ों
अकाउंट तक।

और जवाबों के लिए [उत्पाद FAQ](https://farmpanel.cc/hi/product#faq) देखें।

## गाइड और संसाधन

- [कई Steam अकाउंट सुरक्षित रूप से कैसे चलाएँ](https://farmpanel.cc/hi/guides/run-multiple-steam-accounts-safely)
- [Steam अकाउंट सैंडबॉक्सिंग, समझाया गया](https://farmpanel.cc/hi/guides/steam-account-sandboxing)
- [एक PC कितने CS2 अकाउंट चला सकता है?](https://farmpanel.cc/hi/guides/how-many-cs2-accounts-per-pc)
- [CS2 का साप्ताहिक ड्रॉप, समझाया गया](https://farmpanel.cc/hi/guides/cs2-weekly-drop-explained)
- [CS2 मल्टी-अकाउंट बैन के जोखिम](https://farmpanel.cc/hi/guides/cs2-multi-account-ban-risks)
- [क्या CS2 फ़ार्म के लिए Prime अकाउंट ज़रूरी हैं?](https://farmpanel.cc/hi/guides/prime-accounts-for-cs2-farming)
- [CS2 केस फ़ार्मिंग की अर्थव्यवस्था](https://farmpanel.cc/hi/guides/cs2-case-farming-economics)
- [CS2 ड्रॉप बेचना और पैसे निकालना](https://farmpanel.cc/hi/guides/sell-cs2-drops-steam-market)
- [CS2 फ़ार्म: हाथ से बनाम पैनल से](https://farmpanel.cc/hi/compare/manual-multi-accounting)

## लिंक

| | |
| --- | --- |
| वेबसाइट | [farmpanel.cc](https://farmpanel.cc) |
| उत्पाद | [farmpanel.cc/hi/product](https://farmpanel.cc/hi/product) |
| Changelog | [farmpanel.cc/hi/changelog](https://farmpanel.cc/hi/changelog) |
| Telegram | [t.me/farmpanel_hi](https://t.me/farmpanel_hi) |

---

<div align="center">

यह रिपॉज़िटरी सिर्फ़ साइन किए गए FarmPanel बाइनरी वितरित करती है।
ऐप्लिकेशन का सोर्स कोड प्रोप्राइटरी और बंद है।

`सिस्टम स्थिति · सभी सिस्टम चालू`

**FarmPanel Systems** · सर्वाधिकार सुरक्षित

</div>

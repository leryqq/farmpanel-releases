<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="FarmPanel masaüstü uygulaması, Hesaplar ekranı: yan menü (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) ve durum, giriş, takma ad, iş akışı, sandbox ve son giriş sütunlarıyla bir hesap tablosu"/>

<br/>

# FARMPANEL

**Steam ve CS2 hesap çiftliği paneli — Windows için çoklu hesap orkestrasyonu**

`başlat · yalıt · izle · kurtar`

FarmPanel, bir **Steam hesap çiftliğini** ölçekli biçimde çalıştıran Windows
masaüstü panelidir. Çiftliğinizdeki her **CS2 hesabını** — beş hesaptan
birkaç yüz hesaba kadar — tek bir pencereden başlatır, sandbox içinde yalıtır,
izler ve otomatik olarak yeniden başlatır; otofarm ve bot olmadan.

[**Windows için indir**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Web sitesi](https://farmpanel.cc) ·
[Ürün](https://farmpanel.cc/tr/product) ·
[Telegram](https://t.me/farmpanel_tr)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__tr-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_tr)

Ayrıca şu dillerde mevcut: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Bahasa Indonesia](./README.id.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## FarmPanel nedir

Birden fazla Steam hesabı kullanıyorsanız bu rutini zaten bilirsiniz: aynı
anda açık bir düzine pencere, fark edip elle yeniden açmanız gereken çöken
bir CS2 istemcisi ve kimin yüklemede takıldığını, kimin çoktan maçta
olduğunu anlamanın kolay bir yolunun olmaması. Çiftliğe ne kadar çok hesap
eklerseniz bu iş o kadar zorlaşır.

**FarmPanel, tam da bu zahmeti ortadan kaldırmak için tasarlanmış bir Steam
ve CS2 hesap çiftliği panelidir.** Tüm bir çoklu hesap çiftliğini tek bir
pencereden başlatan, yalıtan ve izleyen bir Windows masaüstü uygulamasıdır —
Steam çoklu hesaplarını elle yönetmeye veya bir yığın betik ile sanal
makineyle uğraşmaya gerçek bir alternatif.

FarmPanel bir **otofarm botu değildir**. Sizin yerinize oynamaz, oyun içi
eylemleri taklit etmez — oyunun *çevresindeki* her şeyi yönetir: istemcileri
başlatmak, lobi davetleri göndermek, çöken oturumları kurtarmak ve her hesap
üzerinde canlı görünürlük sağlamak. Oyun içindeki her eylem gerçek bir
kişinin elinde kalır, böylece çiftliğiniz gerçek oyuncular gibi davranır ve
görünür, çünkü öyledir.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Çiftlik sahipleri neden FarmPanel'i seçiyor

**01 — Asla otofarm yok.**
FarmPanel asla sizin yerinize oynamaz. Her oyun içi eylem elle yapılır,
böylece hesaplar insan gibi görünür, çünkü öyledir.

**02 — Bir kez ayarlayın.**
Her başlatma ve giriş aynı belirlenimci sırayı izler. Dün işe yarayan yarın
da işe yarar, sürpriz yok.

**03 — Çökmeler kendini onarır.**
Steam veya CS2 çökerse FarmPanel bunu fark eder ve saniyeler içinde, sizin
müdahaleniz olmadan geri getirir.

**04 — Gerçek sandbox yalıtımı.**
Her hesap kendi yalıtılmış ortamında çalışır — paylaşılan oturum yok,
paylaşılan dosya yok, hesaplar arası parmak izi karışması yok.

**05 — Şifreler bilgisayarınızdan çıkmaz.**
Kimlik bilgileri Windows'un yerleşik güvenliğiyle şifrelenir ve yalnızca
sizin makinenizde saklanır, hiçbir yere gönderilmez.

**06 — Her hesap üzerinde canlı görünürlük.**
Hesap başına gerçek zamanlı bir pano: durum, maç durumu, çalışma süresi.
Çiftliğin ne yaptığını tahmin etmeye gerek yok.

**07 — Hesap başına ağ yönlendirmesi.**
Her hesap için en iyi sunucu bölgesini seçin; ağ ayarını FarmPanel sizin için
yapar.

**08 — Çiftliğinizle birlikte büyür.**
Beş hesapla başlayın, yüzlerceye ölçekleyin. Baştan sona aynı panel, aynı iş
akışı.

## Başlangıç

1. Kurulumu indirin — yukarıdaki **[Windows için indir](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   düğmesinden ya da bu deponun [Releases](https://github.com/leryqq/farmpanel-releases/releases) sayfasından.
2. `Setup.exe`'yi çalıştırın. FarmPanel sisteminizi kontrol eder ve kurulumda size adım adım yol gösterir.
3. Steam hesaplarınızı ekleyin ve ilk çiftliğinizi başlatın.

```
gereksinimler: Windows 10/11 (64 bit) · .NET 8
önerilen:      32 GB RAM · SSD · aynı anda 16-32 CS2 hesabı
güncellemeler: otomatik, bu depodan
```

## Sık sorulan sorular

**FarmPanel oyunu benim yerime oynar mı?**
Hayır — bütün mesele bu. Bot ve otofarm yok. FarmPanel hesapları yönetir:
başlatma, izleme, lobi kurma, çökmeleri onarma. Oyun içindeki her şeyi siz
yaparsınız, böylece hesaplarınız gerçek oyuncular gibi davranır, çünkü
öyledir.

**Şifrelerim nerede saklanıyor?**
Yalnızca sizin makinenizde. Windows'un yerleşik güvenliğiyle şifrelenir, asla
düz metin olarak saklanmaz ve hiçbir yere gönderilmez.

**Yalnızca CS2 destekli mi?**
Bugün en derin destek CS2'de, canlı maç telemetrisi dahil. Başka oyunlar da
yolda.

**Fiyatı ne kadar?**
Fiyat çiftlik büyüklüğüne göre değişir. [Telegram'dan bize yazın](https://t.me/farmpanel_tr);
küçük kurulumlardan yüzlerce hesaba kadar kurulumunuza uygun bir plan
bulalım.

Daha fazla yanıt için [ürün SSS'sine](https://farmpanel.cc/tr/product#faq) bakın.

## Rehberler ve kaynaklar

- [Birden fazla Steam hesabını güvenle nasıl kullanırsınız](https://farmpanel.cc/tr/guides/run-multiple-steam-accounts-safely)
- [Steam hesap sandbox'ı, açıklandı](https://farmpanel.cc/tr/guides/steam-account-sandboxing)
- [Bir PC kaç CS2 hesabı çalıştırabilir?](https://farmpanel.cc/tr/guides/how-many-cs2-accounts-per-pc)
- [CS2 haftalık drop'u, açıklandı](https://farmpanel.cc/tr/guides/cs2-weekly-drop-explained)
- [CS2 çoklu hesap ban riskleri](https://farmpanel.cc/tr/guides/cs2-multi-account-ban-risks)
- [CS2 farmlamak için Prime hesap gerekir mi?](https://farmpanel.cc/tr/guides/prime-accounts-for-cs2-farming)
- [CS2 sandık farmlama ekonomisi](https://farmpanel.cc/tr/guides/cs2-case-farming-economics)
- [CS2 drop'larını satmak ve parayı çekmek](https://farmpanel.cc/tr/guides/sell-cs2-drops-steam-market)
- [CS2 çiftliği: elle vs. panelle](https://farmpanel.cc/tr/compare/manual-multi-accounting)

## Bağlantılar

| | |
| --- | --- |
| Web sitesi | [farmpanel.cc](https://farmpanel.cc) |
| Ürün | [farmpanel.cc/tr/product](https://farmpanel.cc/tr/product) |
| Changelog | [farmpanel.cc/tr/changelog](https://farmpanel.cc/tr/changelog) |
| Telegram | [t.me/farmpanel_tr](https://t.me/farmpanel_tr) |

---

<div align="center">

Bu depo yalnızca imzalı FarmPanel ikili dosyalarını dağıtır.
Uygulamanın kaynak kodu özel ve kapalıdır.

`sistem durumu · tüm sistemler çalışıyor`

**FarmPanel Systems** · Tüm hakları saklıdır

</div>

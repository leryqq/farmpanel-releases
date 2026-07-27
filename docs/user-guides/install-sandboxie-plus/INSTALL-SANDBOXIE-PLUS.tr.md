# Sandboxie-Plus Kurulumu

**Windows için adım adım kurulum kılavuzu**

Belge sürümü: 1.0 · Sandboxie-Plus sürümü: **1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · **Türkçe** · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · [Tiếng Việt](INSTALL-SANDBOXIE-PLUS.vi.md) · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel her hesabı kendi **sandbox**'ında tutar — Steam ve CS2'nin diğer hesaplarla karışmadığı yalıtılmış bir ortam. Bu yalıtımı **Sandboxie-Plus** adlı ücretsiz bir program sağlar. FarmPanel'de hesap başlatmaya başlamadan önce onu bir kez kurarsınız.

Bu kılavuz sizi kurulumda adım adım yönlendirir. Karmaşık bir şey yok — birkaç dakika sürer.

> **Kısaca.** **Sandboxie-Plus 1.17.5** kurulumunu indirin → çalıştırın → varsayılan ayarları kabul edin → kuruluma izin verin (yönetici hakları gerekir) → tamam.

> **Önemli.** FarmPanel'in kendisinden farklı olarak, Sandboxie-Plus kurulum için **yönetici hakları gerektirir** — bu normaldir, çünkü program uygulamaları güvenilir biçimde yalıtmak için Windows'a derinlemesine yerleşir.

## İçindekiler

1. [Gerekenler](#1-gerekenler)
2. [Adım 1. Kurulumu indirin](#adım-1-kurulumu-indirin)
3. [Adım 2. Kurulumu çalıştırın](#adım-2-kurulumu-çalıştırın)
4. [Adım 3. Kurulum sihirbazından geçin](#adım-3-kurulum-sihirbazından-geçin)
5. [Adım 4. Sandboxie-Plus ilk açılışı](#adım-4-sandboxie-plus-ilk-açılışı)
6. [Adım 5. Her şeyin çalıştığını doğrulayın](#adım-5-her-şeyin-çalıştığını-doğrulayın)
7. [Adım 6. FarmPanel'e bağlayın](#adım-6-farmpanele-bağlayın)
8. [Sandboxie-Plus nasıl kaldırılır](#sandboxie-plus-nasıl-kaldırılır)
9. [Sorun giderme](#sorun-giderme)
10. [Sık sorulan sorular](#sık-sorulan-sorular)

---

# 1. Gerekenler

- **Windows 10 veya 11 çalıştıran bir bilgisayar** (64 bit).
- **Bu bilgisayarda yönetici hakları** (kurulum sırasında bir istem çıkar — **Evet**'e tıklamanız gerekir).
- **İnternet bağlantısı** — programı indirmek için.
- **Yaklaşık 5 dakikanız.**

> Sandboxie-Plus ücretsizdir. Bazı ek özellikler projeyi destekleyenlere sunulur, ancak FarmPanel ile çalışmak için bunlara **gerek yoktur** — sıradan ücretsiz sürüm yeterlidir.

---

# Adım 1. Kurulumu indirin

1. İhtiyacınız olan sürümün resmi sayfasını açın:
   **[GitHub'da Sandboxie-Plus 1.17.5](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. **Assets** bölümüne kadar aşağı kaydırın.
3. **`Sandboxie-Plus-x64-v1.17.5.exe`** benzeri bir adı olan dosyayı bulup indirin — bu, sıradan 64 bit Windows için kurulumdur.

**Doğru dosyayı nasıl seçersiniz:**

| Dosya | Kimin için |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **Çoğu kullanıcı** — Intel veya AMD işlemcili sıradan Windows. Bunu indirin. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Yalnızca ARM işlemcili bilgisayarlar için (nadir). |
| `Sandboxie-Classic-…` | Eski arayüz çeşidi. FarmPanel için **gerekmez** — **Plus**'ı seçin. |
| `.7z` dosyaları | İleri kullanıcılar için taşınabilir sürümler. Kurulum için **gerekmez**. |

**Sonrasında ne olur.** Dosya **İndirilenler** klasörünüzde görünür.

> **İpucu.** Kurulumu yalnızca yukarıda bağlantısı verilen resmi GitHub sayfasından indirin. Böylece gerçek, doğrulanmış sürümü edinirsiniz.

![Assets bölümünü içeren 1.17.5 release sayfası](../images/sandboxie/github-release-assets.png)

---

# Adım 2. Kurulumu çalıştırın

1. **İndirilenler** klasörünüzü açın ve indirdiğiniz **`Sandboxie-Plus-x64-v1.17.5.exe`** dosyasına çift tıklayın.
2. Windows **“Bu uygulamanın cihazınızda değişiklik yapmasına izin veriyor musunuz?”** istemini gösterir — **Evet**'e tıklayın. Bu, yönetici hakları istemidir; onsuz Sandboxie-Plus kurulamaz.

> **Mavi bir SmartScreen penceresi çıkarsa** (“Windows bilgisayarınızı korudu”) — **Ek bilgi**'ye, sonra **Yine de çalıştır**'a tıklayın. Bu, indirilen programlar için sıradan bir uyarıdır, hata değildir.

**Sonrasında ne olur.** Kurulum sihirbazı penceresi açılır.

---

# Adım 3. Kurulum sihirbazından geçin

Kurulum sihirbazı sizi birkaç basit ekrandan geçirir. Çoğu durumda her şeyi varsayılanda bırakıp **Next**'e tıklamanız yeterlidir.

1. **Dil seçimi.** Bir dil seçim penceresi çıkarsa Türkçe (veya dilinizi) seçip **OK**'e tıklayın.
2. **Lisans sözleşmesi.** Okuyup **I Agree** veya **Next**'e tıklayın.
3. **Kurulum klasörü.** Varsayılan klasörü (`C:\Program Files\Sandboxie-Plus`) bırakıp **Next**'e tıklayın. Değiştirmeye gerek yok.
4. **Kurulum seçenekleri.** Hiçbir şeyi değiştirmeye gerek yok — sadece **Next** / **Install**'a tıklayın.
5. Bitmesini bekleyin. Kurulum bir dakikadan az sürer.
6. Son ekranda **Finish**'e tıklayın. Varsa “Sandboxie-Plus'ı başlat” kutusunu işaretli bırakın.

**Sonrasında ne olur.** Sandboxie-Plus kurulur ve simgesi masaüstünüzde ve Başlat menüsünde belirir. Program çoğunlukla kurulumdan hemen sonra açılır.

> **Yeniden başlatma gerekir mi?** Genellikle hayır. Ama sihirbaz bilgisayarı yeniden başlatmanızı isterse, yalıtımın doğru çalışması için bunu yapın.

![varsayılan klasörle kurulum sihirbazı ekranı](../images/sandboxie/installer-wizard.png)

---

# Adım 4. Sandboxie-Plus ilk açılışı

Sandboxie-Plus'ı ilk açtığınızda bir **Setup Wizard** (kurulum sihirbazı) gösterir. Onu adım adım tamamlayın — aşağıda anlatılanı aynen tekrarlayın.

Sihirbazdan önce bir **arayüz dili seçimi** penceresi çıkarsa dilinizi seçip **OK**'e tıklayın.

Ardından sihirbaz sizi birkaç ekrandan geçirir.

### Ekran 1 — Introduction

**“Personally, for private non-commercial use”** (Kişisel, özel ve ticari olmayan kullanım) seçeneğini işaretleyip **Next**'e tıklayın.

![Setup Wizard — “Personally, for private non-commercial use” seçili Introduction ekranı](../images/sandboxie/wizard-1-introduction.png)

### Ekran 2 — Support certificate

Alanı **boş** bırakıp **Next**'e tıklayın. FarmPanel ile çalışmak için sertifika gerekmez.

![Setup Wizard — alanı boş Support certificate ekranı](../images/sandboxie/wizard-2-support-certificate.png)

### Ekran 3 — Configure UI

Değerleri **varsayılanda** bırakın (**Advanced UI for experts** zaten seçili) ve **Next**'e tıklayın.

![Setup Wizard — varsayılan değerlerle arayüz yapılandırma ekranı](../images/sandboxie/wizard-3-ui-configuration.png)

### Ekran 4 — Shell integration

**Tüm kutuların işaretini kaldırın** ve **Next**'e tıklayın.

![Setup Wizard — tüm kutuların işareti kaldırılmış Shell integration ekranı](../images/sandboxie/wizard-4-shell-integration.png)

### Ekran 5 — Updater

**Tüm kutuların işaretini kaldırın** ve **Next**'e tıklayın.

![Setup Wizard — tüm kutuların işareti kaldırılmış Updater ekranı](../images/sandboxie/wizard-5-updater.png)

### Ekran 6 — Complete

Ayarları uygulamak ve sihirbazı kapatmak için **Finish**'e tıklayın.

![Setup Wizard — Finish düğmeli son ekran](../images/sandboxie/wizard-6-complete.png)

> **İpucu.** Herhangi bir ekranda tereddüt ederseniz, kutuların işaretini kaldırıp **Next**'e tıklayın. FarmPanel'in ek entegrasyonlara veya güncelleme hatırlatmalarına ihtiyacı yoktur.

**Sonrasında ne olur.** Ana Sandboxie-Plus penceresi açılır — sandbox listesi ve kontrol paneli.

![ilk açılıştan sonra ana Sandboxie-Plus penceresi](../images/sandboxie/main-window.png)

---

# Adım 5. Her şeyin çalıştığını doğrulayın

Sandboxie-Plus'ın doğru kurulduğundan emin olun:

1. Sandboxie-Plus'ı açın (masaüstündeki veya Başlat menüsündeki simge).
2. Ana pencere bir sandbox listesi gösterir — genellikle **DefaultBox** gibi bir adı olan varsayılan bir sandbox bulunur.
3. Program açılır ve hata iletisi göstermez.

Bunların hepsi yerindeyse — **Sandboxie-Plus kuruludur ve kullanıma hazırdır**.

---

# Adım 6. FarmPanel'e bağlayın

Sandboxie-Plus kurulduğunda FarmPanel onu hesapları yalıtmak için kullanabilir.

1. **FarmPanel**'i açın.
2. **Settings → Sandboxes**'a gidin.
3. Sandbox klasörü yolunun ayarlı olduğundan emin olun. Alan boşsa sandboxlar için bir klasör seçin; zaten doluysa değiştirilecek bir şey yok.
4. **Accounts** ekranına dönün. Artık hesap eklerken sandboxların nasıl atanacağını seçebilirsiniz (**Auto-assign** ve diğerleri) ve hesaplar başlatılabilir.

> **Bu nasıl bağlanır.** FarmPanel'de her hesap bir sandbox'a bağlı olmalıdır, yoksa başlatılamaz. Bu yalıtılmış ortamları “arka planda” oluşturan ve sürdüren Sandboxie-Plus'tır. Sandboxlar ve hesap başlatma hakkında daha fazlası için [FarmPanel Kullanıcı Kılavuzu](../user-guide/USER-GUIDE.tr.md)'na bakın.

**Başarı işareti.** FarmPanel'deki bir hesap başlar ve **Running** durumuna geçer — bu, Sandboxie-Plus üzerinden yalıtımın çalıştığı anlamına gelir.

---

# Sandboxie-Plus nasıl kaldırılır

Programı kaldırmanız gerekirse:

1. Önce sandboxlarda çalışan tüm programları kapatın (FarmPanel'de hesapları **Stop** ile durdurun).
2. **Windows Ayarları** → **Uygulamalar** → **Yüklü uygulamalar**'ı açın
   (veya “Denetim Masası” → “Programlar ve Özellikler”).
3. Listede **Sandboxie-Plus**'ı bulun.
4. **Kaldır**'a tıklayın ve onaylayın. Kaldırmak için de yönetici hakları gerekir.

> **Not.** Sandboxie-Plus kaldırıldıktan sonra, program yeniden kurulana kadar FarmPanel hesap başlatamaz.

---

# Sorun giderme

## Windows kurmaya izin vermiyor — yönetici hakları yok

**Neden.** Sandboxie-Plus kesinlikle yönetici hakları gerektirir.

**Çözüm.** Yönetici haklarına sahip bir hesapla oturum açın veya bilgisayarın yöneticisinden programı kurmasını isteyin. **“Değişikliklere izin veriyor musunuz?”** istemi çıktığında **Evet**'e tıklayın.

## Bir SmartScreen penceresi çıktı

**Neden.** Windows, yakın zamanda indirilen programlar için uyarır. Bu bir hata değildir.

**Çözüm.** **Ek bilgi**'ye, sonra **Yine de çalıştır**'a tıklayın.

## Bir antivirüs kurulumu engelledi

**Neden.** Bazı antivirüsler sisteme yerleşen yazılımlara temkinli yaklaşır.

**Çözüm.**
1. Dosyayı resmi GitHub sayfasından indirdiğinizden emin olun (bağlantı [Adım 1](#adım-1-kurulumu-indirin)'de).
2. Gerekirse dosyayı geçici olarak antivirüs istisnalarına ekleyin ve yeniden indirin.

## Yanlış dosya indirildi

**Neden.** Release sayfasında birkaç dosya var.

**Çözüm.** Sıradan bir Windows için **`Sandboxie-Plus-x64-v1.17.5.exe`** adlı dosya gerekir. **arm64**, **Classic** veya **.7z** çeşitlerini almayın. [Adım 1](#adım-1-kurulumu-indirin)'e dönüp doğru dosyayı indirin.

## FarmPanel kurulumdan sonra hesap başlatmıyor

**Çözüm.**
1. Sandboxie-Plus'ın kurulu olduğundan ve açıldığından emin olun (bkz. [Adım 5](#adım-5-her-şeyin-çalıştığını-doğrulayın)).
2. FarmPanel'de **Settings → Sandboxes**'ı açın ve sandbox klasörü yolunun ayarlı olduğunu kontrol edin.
3. FarmPanel'i yeniden başlatın.
4. Sorun sürerse destekle iletişime geçin (bkz. [Sık sorulan sorular](#sık-sorulan-sorular)).

## Bilgisayar kurulumdan sonra yeniden başlatma istiyor

**Çözüm.** Bilgisayarı yeniden başlatın — bu, kurulumu tamamlar ve yalıtımı etkinleştirir. Yeniden başlatmadan sonra FarmPanel'i tekrar açın.

---

# Sık sorulan sorular

**Sandboxie-Plus kurmak zorunlu mu?**
Evet, FarmPanel'de hesap başlatmak istiyorsanız. Her hesabın ayrı bir ortamda yalıtımını sağlayan Sandboxie-Plus'tır.

**Sandboxie-Plus ücretli mi?**
Hayır, temel sürüm ücretsizdir ve FarmPanel ile çalışmak için yeterlidir. Ek özellikler projeyi destekleyenlere sunulur ama gerekli değildir.

**Kurulum neden yönetici hakları gerektiriyor da FarmPanel gerektirmiyor?**
Sandboxie-Plus programları güvenilir biçimde yalıtmak için Windows'a derinlemesine yerleşir, bu yüzden yönetici haklarına ihtiyaç duyar. FarmPanel ise yalnızca sizin kullanıcı hesabınıza kurulur ve bunlara gerek duymaz.

**Sandboxları kendim yapılandırmam gerekir mi?**
Hayır. Yalnızca Sandboxie-Plus'ı kurun. Hesaplar için sandboxları FarmPanel otomatik olarak oluşturup yapılandırır.

**Destek sertifikası (supporter certificate) gerekir mi?**
Hayır. İlk açılışta o ekranı atlayabilirsiniz. FarmPanel için gerekmez.

**Tam olarak hangi sürümü kurmalıyım?**
**1.17.5** sürümünü — bağlantı [Adım 1](#adım-1-kurulumu-indirin)'de. FarmPanel ile öngörülebilir uyumluluk için tam olarak bunu kurun.

**Bir şey işe yaramazsa nereye başvurmalıyım?**
FarmPanel desteğine Telegram'dan ulaşın: [t.me/farmpanel_tr](https://t.me/farmpanel_tr). Sorunu açıklayın ve varsa hata iletisinin metnini ekleyin.

---

Sandboxie-Plus'ı kurduktan sonra, hesap ekleyip ilk çiftliğinizi başlatmak için [FarmPanel kurulum kılavuzu](../install-guide/INSTALL-GUIDE.tr.md)'na dönün ya da doğrudan [Kullanıcı Kılavuzu](../user-guide/USER-GUIDE.tr.md)'na geçin.

*Sandboxie-Plus kurulum kılavuzunun sonu.*

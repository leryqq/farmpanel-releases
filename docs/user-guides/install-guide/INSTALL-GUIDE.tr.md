# FarmPanel Kurulumu

**Windows için adım adım kurulum kılavuzu**

Belge sürümü: 1.0

🌐 [English](INSTALL-GUIDE.md) · [Русский](INSTALL-GUIDE.ru.md) · [Español](INSTALL-GUIDE.es.md) · [Português](INSTALL-GUIDE.pt.md) · [Français](INSTALL-GUIDE.fr.md) · **Türkçe** · [Bahasa Indonesia](INSTALL-GUIDE.id.md) · [Tiếng Việt](INSTALL-GUIDE.vi.md) · [हिन्दी](INSTALL-GUIDE.hi.md) · [中文](INSTALL-GUIDE.zh.md) · [العربية](INSTALL-GUIDE.ar.md)

---

Bu kılavuz sizi programın indirilmesinden ilk çalıştırmaya kadar götürür. Adımları sırayla izleyin — karmaşık bir şey yok, yalnızca birkaç dakika sürer.

> **Kısaca.** `Setup.exe`'yi indirin → çalıştırın → lisansınızı anahtarla etkinleştirin → tamam. Yönetici hakları gerekmez ve ayrıca başka hiçbir şey kurmanıza gerek yoktur.

## İçindekiler

1. [Gerekenler](#1-gerekenler)
2. [Sistem gereksinimleri](#2-sistem-gereksinimleri)
3. [Adım 1. Kurulumu indirin](#adım-1-kurulumu-indirin)
4. [Adım 2. Kurulumu çalıştırın](#adım-2-kurulumu-çalıştırın)
5. [Adım 3. Uygulamayı açın](#adım-3-uygulamayı-açın)
6. [Adım 4. Başlangıç kurulumu — Steam ve Sandboxie konumları](#adım-4-başlangıç-kurulumu--steam-ve-sandboxie-konumları)
7. [Adım 5. Lisansınızı etkinleştirin](#adım-5-lisansınızı-etkinleştirin)
8. [Adım 6. Her şeyin çalıştığını doğrulayın](#adım-6-her-şeyin-çalıştığını-doğrulayın)
9. [Güncellemeler](#güncellemeler)
10. [Nasıl kaldırılır](#nasıl-kaldırılır)
11. [Kurulum sorunlarını giderme](#kurulum-sorunlarını-giderme)
12. [Sık sorulan sorular](#sık-sorulan-sorular)

---

# 1. Gerekenler

- **Windows 10 veya 11 çalıştıran bir bilgisayar** (64 bit).
- **İnternet bağlantısı** — programı indirmek ve lisansı etkinleştirmek için.
- **Bir lisans anahtarı** — satın alımınızla birlikte alırsınız. Şöyle görünür:
  `XXXX-XXXX-XXXX-XXXX-XXXX` (dörder karakterden beş grup).
- **Yaklaşık 10 dakikanız.**

> Ayrıca başka bir şey (örneğin .NET) kurmanıza **gerek yoktur** — gereken her şey zaten kurulumun içinde bulunur.

---

# 2. Sistem gereksinimleri

| Öğe | En az | Önerilen |
|---|---|---|
| İşletim sistemi | Windows 10 veya 11 (64 bit) | Windows 10 / 11 (64 bit) |
| Bellek | 8 GB | 32 GB |
| Disk | Herhangi biri | SSD |
| Boş alan | yaklaşık 500 MB | 1 GB veya daha fazla |
| Aynı anda hesap | 2 | 4–10 CS2 hesabı |
| Ekran çözünürlüğü | en az 1280 piksel genişlik | Full HD (1920×1080) veya üzeri |

Bilgisayarınız en az gereksinimi karşılıyorsa uygulama çalışır. Bilgisayarınız ne kadar güçlüyse aynı anda o kadar çok hesabı çalışır durumda tutabilirsiniz.

---

# Adım 1. Kurulumu indirin

1. Resmi indirme sayfasını açın:
   **[Windows için indir](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   (indirme bağlantısını [farmpanel.cc](https://farmpanel.cc) sitesinde de bulabilirsiniz).
2. **`Setup.exe`** benzeri bir adı olan dosyayı bulun (releases sayfasındaysanız **Assets** bölümünde) ve indirmek için tıklayın.
3. İndirmenin bitmesini bekleyin. Dosya yaklaşık 50–80 MB'tır, bu yüzden hızlı bir bağlantıda bir dakikadan az sürer.

**Sonrasında ne olur.** `Setup.exe` dosyası **İndirilenler** klasörünüzde görünür.

> **İpucu.** Kurulumu yalnızca yukarıda bağlantısı verilen resmi sayfadan indirin. Böylece programın gerçek, doğrulanmış sürümünü edinirsiniz.

![Setup.exe dosyasının bulunduğu indirme sayfası](../images/install-download-page.png)

---

# Adım 2. Kurulumu çalıştırın

1. **İndirilenler** klasörünüzü açın ve **`Setup.exe`** dosyasına çift tıklayın.
2. Kurulum otomatik başlar. **Yönetici hakları gerekmez** — uygulama yalnızca sizin kullanıcı hesabınıza kurulur.
3. Bitmesini bekleyin. Bu genellikle bir dakikadan az sürer. Tıklanacak ayrı "İleri" düğmeleri yoktur — kurulum her şeyi kendisi yapar.

**Sonrasında ne olur.** Uygulama kurulur ve masaüstünüzde ve Başlat menüsünde bir **FarmPanel** simgesi belirir. Uygulama çoğu zaman kurulumdan hemen sonra açılır.

> **Mavi bir "Windows bilgisayarınızı korudu" (SmartScreen) penceresi çıkarsa** — bu, yeni programlar için sıradan bir uyarıdır, hata değildir. Ne yapmalı:
> 1. **Ek bilgi**'ye tıklayın.
> 2. Beliren **Yine de çalıştır** düğmesine tıklayın.
>
> Kurulum normal şekilde devam eder. Daha fazla ayrıntı: [Kurulum sorunlarını giderme](#kurulum-sorunlarını-giderme).

---

# Adım 3. Uygulamayı açın

Uygulama kendiliğinden açılmadıysa masaüstündeki **FarmPanel** simgesine çift tıklayın veya Başlat menüsünde bulun.

**Ne göreceksiniz.** İlk çalıştırmada uygulama sizi kısa bir başlangıç kurulumu ve lisans etkinleştirmesi boyunca yönlendirir — bunlar sonraki adımlardır.

---

# Adım 4. Başlangıç kurulumu — Steam ve Sandboxie konumları

İlk çalıştırmada uygulama, bilgisayarınızda **Steam** ve **Sandboxie-Plus**'ın nerede bulunduğunu belirtmenizi ister. Bu yollar olmadan uygulama hesapları başlatıp yalıtamaz.

> **Önemli.** Bu noktada Sandboxie-Plus'ın kurulu olması gerekir. Henüz kurmadıysanız ayrı [Sandboxie-Plus Kurulumu](../install-sandboxie-plus/INSTALL-SANDBOXIE-PLUS.tr.md) kılavuzuna bakın.

1. **Steam konumu.** Steam alanının yanındaki klasör seçme düğmesine (**Browse…** / klasör simgesi) tıklayın ve Steam'in kurulu olduğu klasörü seçin. Bu genellikle `C:\Program Files (x86)\Steam`'dir.
2. **Sandboxie konumu.** Sandboxie alanının yanındaki klasör seçme düğmesine tıklayın ve Sandboxie-Plus'ın kurulu olduğu klasörü seçin. Bu genellikle `C:\Program Files\Sandboxie-Plus`'tır.
3. Ayarı onaylayın (**Save** / **Continue** düğmesi).

**Sonrasında ne olur.** Uygulama bu yolları hatırlar ve hesapları her başlattığında kullanır.

**Başarı işareti.** Her iki yol da ayarlanmıştır ve uygulama Steam veya Sandboxie'nin bulunamadığına dair uyarı göstermez.

> **İpucu.** Bu yolları daha sonra istediğiniz zaman **Settings** (Ayarlar) bölümünden değiştirebilirsiniz.

![başlangıç kurulumu — Steam ve Sandboxie konumları](../images/initial-setup-locations.png)

---

# Adım 5. Lisansınızı etkinleştirin

Etkinleştirme yalnızca bir kez gerekir — ilk çalıştırmada.

1. Lisans anahtarınızı giriş alanına yazın veya yapıştırın.
   Panodan yapıştırmak için **Paste from clipboard** (Panodan yapıştır) düğmesine tıklayın.
2. Uygulama, siz yazarken anahtarın biçimini denetler. Biçim doğru olduğunda etkinleştirme düğmesi kullanılabilir hâle gelir.
3. **Activate** (Etkinleştir) düğmesine tıklayın.

**Sonrasında ne olur.** Uygulama sunucuya bağlanır ve anahtarı doğrular. Bu birkaç saniye sürer — **Activating** (Etkinleştiriliyor) durumunu görürsünüz.

**Başarı işareti.** Etkinleştirme penceresi kapanır ve uygulamanın ana ekranı — **Dashboard** — açılır. Lisansınız etkindir. Sonraki çalıştırmalarda anahtarı yeniden girmeniz gerekmez.

> **Anahtar kabul edilmezse** — yazım hatası olmadan girdiğinizden (en kolayı **Paste from clipboard** ile yapıştırmaktır) ve internetiniz olduğundan emin olun. Sık karşılaşılan iletiler [Kurulum sorunlarını giderme](#kurulum-sorunlarını-giderme) bölümünde ele alınmıştır.

![lisans etkinleştirme penceresi](../images/license-activation.png)

---

# Adım 6. Her şeyin çalıştığını doğrulayın

Etkinleştirmenin ardından ana ekrana ulaşırsınız. Kurulumun başarılı olduğunu doğrulayın:

1. Pencerenin üst kısmında bölümleri içeren **kenar çubuğunu** görürsünüz (**Dashboard**, **Accounts**, **Workflows** ve diğerleri).
2. Pencerenin alt kısmında **durum çubuğu** bulunur — bir özet ve uygulama sürümünü (örneğin `v1.0.1`) içeren ince bir şerit.
3. Uygulama açılır ve bölümler arasında hatasız geçiş yapar.

Bunların hepsi yerindeyse — **kurulum tamamlanmıştır ve uygulamayı kullanmaya başlayabilirsiniz**.

**Sırada ne var.** Steam hesaplarınızı ekleyin ve ilk çiftliğinizi başlatın. Adım adım yönergeler için [Kullanıcı Kılavuzu](../user-guide/USER-GUIDE.tr.md)'na bakın (“Temel iş akışları” bölümü).

![kurulumdan sonraki ana ekran](../images/dashboard-overview.png)

---

# Güncellemeler

FarmPanel **otomatik** olarak güncellenir — elle bir şey indirmenize gerek yoktur.

- Uygulama, başlangıçta ve çalışırken ara ara yeni sürüm olup olmadığını denetler.
- Yeni sürüm, çalışmanızı kesmeden arka planda sessizce indirilir.
- Güncelleme, uygulama bir sonraki yeniden başlatıldığında uygulanır.

**Sizin yapacağınız.** Özel bir şey yok. Zaman zaman uygulamayı kapatıp yeniden açmanız yeterli; en son sürüm kurulur. Geçerli sürüm her zaman alttaki durum çubuğunda ve **Settings → About** (Ayarlar → Hakkında) bölümünde görünür.

---

# Nasıl kaldırılır

FarmPanel'i kaldırmanız gerekirse:

1. **Windows Ayarları** → **Uygulamalar** → **Yüklü uygulamalar**'ı açın
   (veya “Denetim Masası” → “Programlar ve Özellikler”).
2. Listede **FarmPanel**'i bulun.
3. **Kaldır**'a tıklayın ve onaylayın.

**Sonrasında ne olur.** Uygulama bilgisayarınızdan kaldırılır. Kaldırmak için yönetici hakları gerekmez.

---

# Kurulum sorunlarını giderme

Aşağıda sık karşılaşılan durumlar ve ne yapılacağı verilmiştir.

## "Windows bilgisayarınızı korudu" (SmartScreen) penceresi çıktı

**Neden.** Windows bu uyarıyı, yakın zamanda indirilmiş ve sistemin henüz iyi tanımadığı programlar için gösterir. Bu, dosyada bir sorun olduğu anlamına gelmez.

**Çözüm.**
1. **Ek bilgi**'ye tıklayın.
2. **Yine de çalıştır**'a tıklayın.

Kurulum devam eder. **Ek bilgi** düğmesi yoksa dosyayı resmi sayfadan indirdiğinizden emin olun ve yeniden deneyin.

## Bir antivirüs dosyayı engelledi veya sildi

**Neden.** Bazı antivirüsler yeni kurulumlara temkinli yaklaşır ve yanlış alarm verebilir.

**Çözüm.**
1. `Setup.exe`'yi resmi sayfadan indirdiğinizden emin olun (bağlantı [Adım 1](#adım-1-kurulumu-indirin)'de).
2. Gerekirse dosyayı antivirüs istisnalarına ekleyin ve yeniden indirin.
3. Emin değilseniz destekle iletişime geçin (bkz. [Sık sorulan sorular](#sık-sorulan-sorular)).

## Tarayıcı dosyayı indirmeye izin vermiyor

**Neden.** Bir `.exe` indirirken tarayıcı da temkinli olabilir.

**Çözüm.** Tarayıcının indirme panelinde dosyanın yanındaki **Sakla** (Keep) seçeneğini seçin. Böylece indirme tamamlanır.

## Kurulum çift tıklamayla başlamıyor

**Çözüm.**
- Dosyanın tam indirildiğinden emin olun (yaklaşık 50–80 MB).
- Dosyaya sağ tıklayın ve **Aç**'ı seçin.
- Dosya bozuksa kurulumu yeniden indirin.

## Lisans anahtarı kabul edilmiyor

| İleti | Ne anlama gelir | Ne yapmalı |
|---|---|---|
| “License key invalid” | Anahtar yazım hatasıyla girildi | Yazımı kontrol edin. En kolayı anahtarı **Paste from clipboard** ile yapıştırmaktır |
| “Used on max devices” | Lisans en fazla cihaz sayısında kullanılıyor | Lisansı başka bir cihazda serbest bırakın, sonra yeniden deneyin. **Manage devices** düğmesi cihaz yönetimine götürür |
| “Cannot reach license server” | Sunucuya bağlantı yok | İnternet bağlantınızı denetleyin ve **Retry**'a tıklayın |

## Uygulama kurulumdan sonra açılmıyor

**Çözüm.**
- Elle açın: masaüstündeki veya Başlat menüsündeki **FarmPanel** simgesi.
- Bilgisayarı yeniden başlatın ve tekrar deneyin.
- Yardımcı olmazsa uygulamayı yeniden kurun: kaldırın (bkz. [Nasıl kaldırılır](#nasıl-kaldırılır)) ve yeniden kurun.

---

# Sık sorulan sorular

**Kurulum için yönetici hakları gerekir mi?**
Hayır. FarmPanel yalnızca sizin kullanıcı hesabınıza kurulur ve yönetici hakları gerektirmez.

**.NET veya başka bileşenleri ayrıca kurmam gerekir mi?**
Hayır. Gereken her şey zaten kurulumun içindedir — yalnızca `Setup.exe`'yi çalıştırın.

**Uygulama nereye kurulur?**
Kişisel kullanıcı klasörünüze. Klasörü elle seçmenize gerek yoktur — kurulum bunu halleder.

**SmartScreen penceresinde "Yine de çalıştır"a tıklamak güvenli mi?**
Evet, `Setup.exe`'yi bu kılavuzda belirtilen resmi sayfadan indirdiyseniz. Uyarı yalnızca program sistem için yeni olduğundan çıkar.

**Kurulumdan sonra şifrelerim nerede saklanır?**
Yalnızca bilgisayarınızda. Windows'un yerleşik korumasıyla şifrelenir, asla düz metin olarak saklanmaz ve hiçbir yere gönderilmez.

**Lisans anahtarını her seferinde girmem gerekir mi?**
Hayır. Anahtar yalnızca bir kez, ilk etkinleştirmede girilir. Sonrasında uygulama doğrudan ana ekranda açılır.

**Uygulamayı yeni sürüme nasıl güncellerim?**
Yapılacak bir şey yok — FarmPanel otomatik güncellenir. En son sürümün kurulması için uygulamayı ara sıra yeniden başlatmanız yeterli (bkz. [Güncellemeler](#güncellemeler)).

**Bir şey işe yaramazsa nereye başvurmalıyım?**
Telegram'dan destekle iletişime geçin: [t.me/farmpanel_tr](https://t.me/farmpanel_tr). Sorunu açıklayın ve varsa hata iletisinin metnini ekleyin.

---

Kurulumdan sonra [Kullanıcı Kılavuzu](../user-guide/USER-GUIDE.tr.md)'na geçin — hesap ekleme, başlatma ve uygulamayla çalışma konularını ayrıntılı anlatır.

*FarmPanel kurulum kılavuzunun sonu.*

# FarmPanel Kullanım Kılavuzu

**Windows'ta Steam ve CS2 hesap çiftliğiniz için kontrol paneli**

Belge sürümü: 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · [Português](USER-GUIDE.pt.md) · [Français](USER-GUIDE.fr.md) · **Türkçe** · [Bahasa Indonesia](USER-GUIDE.id.md) · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Bu kılavuz nasıl okunur.** Düğmeler, sekmeler ve durumlar uygulamada yazıldığı gibi tam olarak **kalın** biçimde görünür (örneğin, **Add Account**, **Start**, **Running**), böylece her zaman doğru yere tıklarsınız. Her işlem, neye tıklayacağınızı, ardından ne olacağını ve başarıyı nasıl doğrulayacağınızı anlatır.

## İçindekiler

1. [Giriş](#1-giriş)
2. [Başlamadan önce](#2-başlamadan-önce)
3. [İlk çalıştırma](#3-i̇lk-çalıştırma)
4. [Arayüze genel bakış](#4-arayüze-genel-bakış)
5. [Temel iş akışları](#5-temel-i̇ş-akışları)
6. [Sık yapılan işler («İstiyorum ki…»)](#6-sık-yapılan-i̇şler-i̇stiyorum-ki)
7. [Özellik başvurusu](#7-özellik-başvurusu)
8. [Durumlar ve göstergeler](#8-durumlar-ve-göstergeler)
9. [Bildirimler](#9-bildirimler)
10. [Hatalar ve sorun giderme](#10-hatalar-ve-sorun-giderme)
11. [En iyi uygulamalar](#11-en-i̇yi-uygulamalar)
12. [Sıkça sorulan sorular](#12-sıkça-sorulan-sorular)

---

# 1. Giriş

## FarmPanel nedir

**FarmPanel**, çok sayıda Steam hesabını ve Counter-Strike 2 istemcisini tek bir pencereden yönetmenize yardımcı olan bir Windows masaüstü uygulamasıdır. Onlarca Steam penceresini elle açmak, her birini gözlemek ve donanları yeniden başlatmak yerine, tüm hesap çiftliğinizi merkezî olarak — tek ve anlaşılır bir panelden — yönetirsiniz.

FarmPanel istemcileri başlatır, hesapları birbirinden yalıtır, durumlarını gerçek zamanlı izler ve arızalardan sonra otomatik olarak toparlar.

> **Önemli.** FarmPanel **bir bot ya da otomatik çiftçi değildir**. Sizin yerinize oynamaz ve oyun içi eylemleri taklit etmez. Oyunun *çevresinde* olup biten her şeyi yönetir: istemcileri başlatma, lobi davetleri, arızalardan sonra toparlanma ve her hesap için canlı görünürlük. Tüm oyun içi eylemler gerçek bir kişi tarafından yapılır.

## Hangi sorunları çözer

Birden fazla hesabınız varsa bu rutin size tanıdık gelecektir:

- onlarca Steam ve CS2 istemcisini başlatmanız gerekir;
- her hesabın diğerlerine karışmadan ayrı ayrı çalışması gerekir;
- lobileri kurmak ve davetleri elle göndermek yavaş ve yorucudur;
- çöken bir CS2'yi zamanında fark edip yeniden başlatmak gerekir;
- kimin zaten maçta olduğunu, kimin yüklenirken takıldığını anlamak zordur.

FarmPanel bu rutini ortadan kaldırır ve her işlemi tek bir uygulamada toplar.

## Kimler için

Uygulama, çok sayıda Steam ve CS2 hesabını — birkaç taneden birkaç yüze kadar — otomatik başlatma, canlı izleme ve arızalardan sonra güvenilir toparlanmayla merkezî olarak yönetmesi gereken herkes için tasarlanmıştır.

## Neler yapabilirsiniz

- Tüm hesapları tek bir yerde tutup ihtiyacınız olanı hızlıca bulun.
- Hesapları tek tek ya da toplu olarak başlatıp durdurun.
- Her hesabı kendi korumalı ortamında (bir sandbox içinde) yalıtın.
- Hesaplardan gruplar kurup birlikte eşleşme sırasına sokun.
- Bilgisayar yükünü, süreç sağlığını ve çökmeleri gerçek zamanlı izleyin.
- Bir çökmeden ya da uygulama kapandıktan sonra hesapları otomatik toparlayın.
- Bir hazır düzen kullanarak CS2 pencerelerini monitörlerinize dizin.

![FarmPanel ana ekranı (Dashboard)](../images/dashboard-overview.png)

---

# 2. Başlamadan önce

## Sistem gereksinimleri

| Öğe | Minimum | Önerilen |
|---|---|---|
| İşletim sistemi | Windows 10 veya 11 (64 bit) | Windows 10 / 11 (64 bit) |
| Bellek | 8 GB | 32 GB |
| Disk | Herhangi biri | SSD |
| Eşzamanlı hesaplar | 2 | 4–10 CS2 hesabı |
| Ekran çözünürlüğü | Çalışma alanı en az 1280 piksel genişliğinde | Full HD (1920×1080) veya daha yüksek |

## Önceden hazırlanacaklar

- **FarmPanel yükleyicisi** — resmi indirme sayfasından indirdiğiniz, `Setup.exe` adlı bir dosya.
- **Bir lisans anahtarı** — satın alımınızla birlikte alırsınız. Şöyle görünür: `XXXX-XXXX-XXXX-XXXX-XXXX` (dörder karakterlik beş grup).
- **Steam hesap bilgileriniz** — kullanıcı adları ve parolalar, kullanıyorsanız Steam Guard kodları. Bunları tek tek girebilir veya bir dosyadan liste hâlinde içe aktarabilirsiniz.
- **Bir internet bağlantısı** — lisansı etkinleştirmek için ilk çalıştırmada, sonrasında ise Steam ve CS2'nin çalışması için gereklidir.

## İzinler

- Kurulum **yönetici hakları gerektirmez** — uygulama yalnızca kullanıcı hesabınıza kurulur.
- Yükleyiciyi ilk çalıştırdığınızda Windows mavi bir **SmartScreen** penceresi gösterebilir (“Windows protected your PC”) — bu, yeni programlar için sıradan bir uyarıdır. **More info** ve ardından **Run anyway** seçeneğine tıklayın.
- Uygulamanın ağ erişimine (Steam için) ve Windows Güvenlik Duvarı kurallarına erişime ihtiyacı olabilir. Bir güvenlik duvarı istemi çıkarsa erişime izin verin.

## Verileriniz nerede saklanır

Kullanıcı adları ve parolalar, Windows'un yerleşik korumasıyla şifrelenir ve **yalnızca bilgisayarınızda** saklanır. Hiçbir zaman düz metin olarak kaydedilmez ve hiçbir yere gönderilmez.

---

# 3. İlk çalıştırma

Aşağıda kurulumdan kullanıma hazır panele kadar izlenecek yol var. Adımları sırayla uygulayın.

## Adım 1. Uygulamayı kurun

1. İndirme sayfasından `Setup.exe` yükleyicisini indirin.
2. `Setup.exe` dosyasına çift tıklayın.
3. Mavi bir **SmartScreen** penceresi çıkarsa (“Windows protected your PC”), **More info** ve ardından **Run anyway** seçeneğine tıklayın. Bu, yeni programlar için sıradan bir uyarıdır, bir hata değildir.
4. Kurulumun bitmesini bekleyin. Yönetici hakları gerekmez — yükleyici sisteminizi denetler ve her şeyi hazırlar.

**Sonrasında ne olur.** Masaüstünüzde ve Başlat menüsünde bir FarmPanel simgesi belirir.

![Setup.exe yükleyici penceresi](../images/setup-installer.png)

## Adım 2. Uygulamayı açın

Masaüstünüzdeki **FarmPanel** simgesine çift tıklayın.

**Ne göreceksiniz.** İlk çalıştırmada, lisans henüz etkinleştirilmediği için **Activation Wizard** (etkinleştirme sihirbazı) açılır. Ana ekran yalnızca başarılı etkinleştirmeden sonra görünür.

## Adım 3. Lisansınızı etkinleştirin

Etkinleştirme penceresi size adım adım yol gösterir.

1. Lisans anahtarınızı giriş alanına yazın veya yapıştırın. Panodan yapıştırmak için **Paste from clipboard** düğmesine tıklayın.
2. Uygulama, siz yazdıkça anahtarın biçimini denetler. Biçim doğru olduğunda etkinleştirme düğmesi kullanılabilir hâle gelir.
3. **Activate** düğmesine tıklayın.

**Sonrasında ne olur.** Uygulama lisans sunucusuna bağlanır ve anahtarı doğrular. Bu birkaç saniye sürer — **Activating** durumunu görürsünüz.

**Başarı işareti.** Etkinleştirme penceresi kapanır ve uygulamanın ana ekranı (**Dashboard**) açılır. Lisansınız etkin — sonraki çalıştırmalarda anahtarı tekrar girmenize gerek kalmaz.

> **Etkinleştirme başarısız olursa**, uygulama anlaşılır bir mesaj gösterir ve ne yapmanız gerektiğini söyler. Sık karşılaşılan durumlar [10. Hatalar ve sorun giderme](#10-hatalar-ve-sorun-giderme) bölümünde ele alınır.

![lisans etkinleştirme penceresi](../images/license-activation.png)

## Adım 4. Temel ayarları gözden geçirin

Hesapları ilk kez başlatmadan önce ayarlarınızı gözden geçirmek yerinde olur.

1. Sol paneldeki **Settings** düğmesine tıklayın veya `Ctrl+,` tuşlarına basın.
2. **Sandboxes** bölümünü açın ve gerekiyorsa sandbox'lar için bir klasör seçin.
3. İsterseniz **Appearance** bölümünü açıp bir tema (**System / Dark / Light**) ile arayüz yoğunluğunu seçin.

Ayarlar otomatik kaydedilir: her değişiklikten sonra kısa bir **Saved** bildirimi belirir.

## Adım 5. Kullanıma hazırsınız

Artık hesap ekleyip ilk çiftliğinizi başlatabilirsiniz. Nasıl yapıldığını [5. Temel iş akışları](#5-temel-i̇ş-akışları) bölümünde görün.

**Her şeyin çalıştığının işareti.** Pencerenin alt çubuğu (durum çubuğu) bir özet gösterir: hesap sayısı, etkin süreçler ve mevcut uygulama sürümü.

---

# 4. Arayüze genel bakış

Uygulama tek bir ana pencerede çalışır. Her zaman yerinde duran sabit öğelerden ve seçtiğiniz bölüme göre değişen bir ekran alanından oluşur.

```
┌────────────────────────────────────────────────────────────┐
│  Command Bar                                                │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Sidebar  │   Seçili ekranın çalışma alanı                  │
│          │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Status Bar                                                 │
└────────────────────────────────────────────────────────────┘
```

![etiketli alanlarla genel pencere yapısı](../images/window-layout.png)

## 4.1. Command Bar (üst çubuk)

**Amacı.** Pencerenin üstünde uzanan sabit bir şerit. Gezinme, genel arama ve bildirimleri barındırır.

**Konumu.** Pencerenin en üst satırı.

**Ana öğeler (soldan sağa):**

- **Hamburger düğmesi (☰)** — yan çubuğu daraltır ve genişletir. Kısayol `Ctrl+B`.
- **Logo** — tıklandığında sizi ana ekrana (**Dashboard**) döndürür.
- **Breadcrumbs (yol izi)** — nerede olduğunuzu gösterir, örneğin `Accounts › alex_42 › Events`. Herhangi bir parçaya tıklayarak oraya atlayın.
- **Arama / komut paleti** — ortada. Komut paletini açmak için `Ctrl+K` tuşlarına basın (aşağıya bakın).
- **Bildirim rozeti** — sayaçlı bir simge (örneğin, `⚠ 3`). Tıklamak bildirim merkezini açar.

**Ne zaman kullanılır.** Command Bar her zaman elinizin altındadır: ekranlar arasında hızlı geçiş, bir hesabı kullanıcı adıyla arama ya da fareye dokunmadan bir komut çalıştırmak için.

### Command Palette

Uygulamadaki her eylem ve nesne için bir arama kutusu olan komut paletini açmak üzere istediğiniz anda `Ctrl+K` tuşlarına basın.

1. Bir komutun, ekranın, hesap kullanıcı adının veya iş akışının adını yazmaya başlayın.
2. Liste, eşleşen sonuçlara daralır. Aralarında `↑` `↓` ile gezinin.
3. Seçili öğeyi çalıştırmak için `Enter` tuşuna basın.

**Neden işe yarar.** Komut paleti, düğmelerin nerede olduğunu ezberlemeden her şeyi bulmanın en hızlı yoludur.

![açık komut paleti](../images/command-palette.png)

## 4.2. Sidebar (yan çubuk)

**Amacı.** Uygulamanın ana gezinme bölmesi.

**Konumu.** Solda, pencerenin tüm yüksekliği boyunca.

**Bölümler (yukarıdan aşağıya):**

| Simge | Bölüm | Ne gösterir |
|---|---|---|
| ▤ | **Dashboard** | Tüm çiftliğe genel bakış |
| 👥 | **Accounts** | Tüm hesapların listesi (ana çalışma ekranı) |
| ⚙ | **Workflows** | Otomatik başlatma senaryoları ve ilerlemeleri |
| ⚔ | **Matchmaking** | Gruplar ve maç arama |
| 📈 | **Monitoring** | Bilgisayar yükü ve süreç sağlığı |
| 📜 | **Logs** | Olay günlüğü |
| ▣ | **Layouts** | CS2 pencerelerini monitörlere dizme |
| ▦ | **Sandboxes** | Sandbox'lar (yalıtılmış ortamlar) |
| ⚙ | **Settings** | Uygulama ayarları |
| ? | **Help** | Yardım |

Bazı bölümler bir sayaç (örneğin, hesap sayısı) ya da etkinlik olduğunda canlı bir nokta gösterir.

**Ana eylemler:**

- Açmak için bir bölüme tıklayın. `Ctrl+1`…`Ctrl+8` tuşlarını da kullanabilirsiniz.
- Daraltma düğmesi (ya da `Ctrl+B`) paneli yer açmak için simgelere küçültür.

**İpucu.** Bölümler arasında geçiş, durumunuzu korur — filtreler, seçim ve kaydırma konumu. Bir ekrana döndüğünüzde onu tam bıraktığınız gibi bulursunuz.

![tüm bölümleriyle yan çubuk](../images/sidebar.png)

## 4.3. Status Bar (durum çubuğu)

**Amacı.** Tüm çiftliğin durumunu hızlıca özetleyen, pencerenin altındaki ince bir çubuk.

**Konumu.** Pencerenin en alt satırı.

**Ne gösterir (örnek):**

```
[env: PROD] | ● 412 accounts (238 running) | ▶ 18 workflows | ◎ 7 matches | CPU 42% RAM 71% | ⚠ 3 errors | 14:32:08 | v1.0.1
```

- kaç hesap olduğu ve şu anda kaçının çalıştığı;
- kaç iş akışının ve kaç etkin maçın sürdüğü;
- işlemci ve bellek yükü;
- hata sayısı (bildirim merkezini açmak için tıklayın);
- saat ve uygulama sürümü.

**Ne zaman kullanılır.** Her şeyin yolunda olup olmadığını bir saniyede anlamak için durum çubuğuna göz atın.

## 4.4. Dashboard ekranı

**Amacı.** Tek bir genel bakış ekranı. Birkaç saniyede şu soruları yanıtlar: kaç hesap çevrimiçi, kaç iş akışı çalışıyor ya da başarısız oldu, eşleşme etkinliği var mı, herhangi bir çökme var mı ve bilgisayar ne kadar yüklü.

**Konumu.** Yan çubuktaki ilk bölüm. Başlatmadan hemen sonra açılır.

**Ana alanlar:**

- **KPI şeridi** — en üstteki beş kart: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Her biri bir ana sayı ve küçük bir grafik gösterir. Bir karta tıklamak sizi ilgili ekrana götürür.
- **Live Activity Feed** — operasyonel olayların gerçek zamanlı akışı. Kaydırmayı duraklatmak için duraklat düğmesini (ya da `Space` tuşunu) kullanın.
- **Account State Heatmap** — her hesabın renkli bir hücre olduğu bir ızgara. Renk, hesabın durumunu yansıtır. Kullanıcı adını ve durumu görmek için üzerine gelin; hesaba atlamak için tıklayın.
- **Active Workflows / Matchmaking Queue / Sandboxes** — iş akışlarını, maç sırasını ve sandbox'ları özetleyen üç kutu.
- **Failures & Crashes** — son bir saatteki hataların ve çökmelerin bir tablosu.

**Tipik kullanım.** Sabahları **Dashboard** ekranını açıp çiftliği bir bakışta değerlendirin, sonra dikkat gereken yere gidin.

**İpuçları.**
- Ölçümler otomatik yenilenir. Tam bir yenileme zorlamak için `F5` tuşuna basın.
- **Errors** kartında ya da hata tablosunda kırmızı vurgulu bir şey varsa incelemenize oradan başlayın.

![KPI şeridi ve etkinlik akışıyla Dashboard](../images/dashboard-screen.png)

## 4.5. Accounts ekranı

**Amacı.** Ana çalışma ekranı. Burada hesapları saklar, ihtiyacınız olanları bulur ve onları başlatıp durdurursunuz.

**Konumu.** Yan çubuktaki ikinci bölüm (`Ctrl+2`).

**Ana alanlar:**

- **Araç çubuğu** — **Add Account**, **Import**, **Export** ve **Refresh** düğmeleri, arama alanı, filtreler ve görünüm denetimleri.
- **Hesap tablosu** — tüm hesapların şu sütunlarla bir listesi: durum, kullanıcı adı, takma ad, rütbe, iş akışı, sandbox, etiketler, son giriş zamanı ve diğerleri.
- **Details Pane (ayrıntı bölmesi)** — sağda. Seçili hesabın ayrıntılarını gösterir. `Ctrl+\` ile gösterin veya gizleyin.

**Neler yapabilirsiniz:**

- Hesapları tek tek ekleyin veya bir liste içe aktarın.
- Hesapları arayın ve filtreleyin.
- Tek bir hesabı ya da aynı anda birçoğunu başlatın, durdurun ve yeniden başlatın.
- Hesapları sandbox'lara bağlayın ve iş akışları atayın.
- Ayrıntılı bir hesap kartı görüntüleyin: veriler, geçmiş, olaylar ve günlükler.

**Tipik kullanım.** Tabloda ihtiyacınız olan hesapları seçin, sonra onlara bir eylem uygulayın — araç çubuğu, bağlam menüsü (sağ tıklama) veya klavye kısayolları aracılığıyla.

Ayrıntılı adım adım yönergeler [5. Temel iş akışları](#5-temel-i̇ş-akışları) bölümündedir.

![tablo ve ayrıntı bölmesiyle Accounts ekranı](../images/accounts-screen.png)

### Hesap ayrıntı bölmesi (Details Pane)

Tablonun sağında, seçili hesap için şu sekmeleri içeren bir kart belirir:

| Sekme | Ne gösterir |
|---|---|
| **Overview** | Temel veriler, sandbox bağlantısı, atanan iş akışı, etiketler, önemli tarihler ve eylem düğmeleri |
| **Inventory** | Hesabın envanteri: eşya sayısı ve değeri |
| **Workflow** | Atanan senaryonun mevcut durumu ve o anki adımı |
| **Events** | Bu hesaba ait son olaylar |
| **Logs** | Bu hesaba göre filtrelenmiş olay günlüğü |
| **History** | Değişiklik geçmişi: oluşturma, düzenlemeler, yeniden adlandırmalar, sandbox yeniden bağlamaları |

**Overview** sekmesinin altında bir düğme bloğu vardır: **Start**, **Stop**, **Restart**, **Pause**, ayrıca **Edit account** ve **Delete**. En uygun eylem vurgulanır: hesap durmuşken **Start**, çalışırken **Stop**.

## 4.6. Workflows ekranı

**Amacı.** Otomatik başlatma senaryolarını yönetin ve çalışmalarını izleyin.

**Konumu.** Yan çubuktaki üçüncü bölüm (`Ctrl+3`).

**İş akışı nedir.** Bir iş akışı, uygulamanın bir hesap için yürüttüğü önceden tanımlı bir adım dizisidir: Steam'e giriş yapma, CS2'yi başlatma vb. Aynı senaryo her zaman aynı şekilde çalışır, dolayısıyla sonuç öngörülebilir.

- **Definition** — senaryo şablonu: bir adımlar kümesi.
- **Instance** — belirli bir hesap için bir definition'ın tek bir çalışması.

**Ana alanlar:**

- **Solda** — definition'ların (şablonların) ve sürümlerinin bir listesi.
- **Ortada** — çalışan instance'ların bir tablosu: hangi senaryo, hangi hesap için, hangi adımda, kaç yeniden deneme, ne zaman başladı.
- **Sağda** — seçili instance'ın ayrıntıları (**Overview**, **State Machine**, **Steps**, **Logs**, **Retries** sekmeleri).
- **Altta** — görünen instance'lar için daraltılabilir bir olay zaman çizelgesi (`Ctrl+T`).

**Ne zaman kullanılır.** Her hesabın başlatmasının hangi adımda olduğunu görmek, bir senaryoyu duraklatmak ya da yeniden başlatmak veya bir şeyin neden bitmediğini anlamak için buraya gelin.

![üç bölmeli Workflows ekranı](../images/workflows-screen.png)

## 4.7. Matchmaking ekranı

**Amacı.** Hesaplardan gruplar kurun ve birlikte eşleşme sırasına sokun.

**Konumu.** Yan çubuktaki dördüncü bölüm (`Ctrl+4`).

**Temel kavramlar:**

| Terim | Anlamı |
|---|---|
| **Party** | Birlikte maç arayan bir hesap grubu |
| **Quorum** | Tüm grup üyeleri giriş yapmış, sırada ve maçta değil |
| **Queue** | Maç bekleme: sıra, bölge, mod |
| **Match Found** | Steam bir maç buldu. Uygulama tüm üyeler için hazır olduğunu otomatik onaylar — bir şey yapmanız gerekmez |
| **Desync** | Üyeler tutarsız bir durumda (örneğin, biri sıradan düştü) |

**Ana alanlar:**

- **Solda** — grupların durumlarıyla listesi (quorum, desync, match found, boşta).
- **Sağda** — seçili grubun ayrıntıları: üyeler, durumları, sıra konumu, ağ gecikmesi, sandbox.
- **Altta** — son eşleşme olaylarının bir zaman çizelgesi.

**Ne zaman kullanılır.** Burada 2–5 hesaptan gruplar kurup sıraya sokarsınız. Bir maç bulunduğunda uygulama tüm üyeler için hazır olduğunu otomatik onaylar.

![gruplar ve ayrıntılarla Matchmaking ekranı](../images/matchmaking-screen.png)

## 4.8. Monitoring ekranı

**Amacı.** Bilgisayar yükünü, süreç sağlığını ve çökmeleri gerçek zamanlı izleyin.

**Konumu.** Yan çubuktaki beşinci bölüm (`Ctrl+5`).

**Ana alanlar:**

- **Kaynak göstergeleri** — güncel değerler ve küçük grafiklerle **CPU**, **RAM**, **Disk**, **Net** ve mümkün olan yerlerde **GPU** kartları.
- **Process Explorer** — çalışan tüm Steam ve CS2 süreçlerinin bir tablosu: her birinin hangi hesaba ait olduğu, ne kadar tükettiği, ne kadar süredir çalıştığı.
- **Crashes & Warnings** — son arızaların bir akışı.
- **Logs panel** — ekranın altında, daraltılabilen bir günlük.

**Zaman denetimleri.** Üstte **Live** (gerçek zaman), **Last 1h / 24h** ve **Custom** (özel bir dönem) arasında geçiş yapabilirsiniz. **Freeze** düğmesi (`Ctrl+Space`) görüntüyü dondurur, böylece onu rahatça inceleyebilirsiniz.

**Ne zaman kullanılır.** Bilgisayar yavaşlamaya başlar ya da çökmeler sıklaşırsa hangi sürecin kaynak tükettiğini ve tam olarak neyin çöktüğünü görmek için **Monitoring** ekranını açın.

> **İpucu.** **Monitoring** ekranını ayır düğmesiyle ayrı bir pencerede açıp ikinci bir monitöre yerleştirebilirsiniz.

![göstergeler ve süreç listesiyle Monitoring ekranı](../images/monitoring-screen.png)

## 4.9. Logs ekranı

**Amacı.** Tüm uygulama olaylarının ayrıntılı bir günlüğü — olup bitenlerin canlı bir akışı gibi.

**Konumu.** Yan çubuktaki altıncı bölüm (`Ctrl+6`).

**Ana özellikler:**

- **Düzey filtresi** — **Error**, **Warn**, **Info**, **Debug** anahtarları. Varsayılan olarak hatalar, uyarılar ve bilgi mesajları gösterilir.
- **Kaynak filtresi** — günlüğü tek bir hesap, iş akışı ya da sandbox ile daraltabilirsiniz.
- **Arama** — `Ctrl+F`, eşleşmeler arasında atlamayla (`F3` / `Shift+F3`).
- **Follow** — günlük yeni satırlara otomatik kayar. `Space` tuşu takibi açıp kapatır. Yukarı kaydırırsanız takip duraklar ve bir en alta git düğmesi belirir.
- **Export** — görünen satırları bir dosyaya kaydedin.

**Ne zaman kullanılır.** Ayrıntılara ihtiyaç duyduğunuzda: belirli bir hesaba tam olarak ne olduğu ve hangi sırayla.

![olay günlüğü olan Logs ekranı](../images/logs-screen.png)

## 4.10. Layouts ekranı

**Amacı.** Bir hazır düzen kullanarak CS2 pencerelerini bir ya da daha fazla monitöre dizin.

**Konumu.** Yan çubuktaki yedinci bölüm (`Ctrl+7`).

**Temel kavramlar:**

- **Preset** — kaydedilmiş bir pencere dizilimi.
- **Slot** — bir pencerenin yerleşeceği, monitör üzerinde dikdörtgen bir alan.
- **Snap** — çalışan pencereleri slot'lara dizen komut.

**Ana alanlar:**

- **Solda** — kaydedilmiş preset'lerin bir listesi.
- **Sağda** — monitörlerinizi gösteren, üzerine slot yerleştirdiğiniz bir tuval.
- **Altta** — bir bağlamalar tablosu: hangi slot'un hangi hesaba ya da role karşılık geldiği.

**Nasıl kullanılır.**
1. **New Preset** düğmesiyle bir preset oluşturun.
2. Slot'ları tuvale yerleştirin.
3. Hangi hesabın hangi slot'a gireceğini belirleyin.
4. **Apply** ya da **Snap windows** düğmesine tıklayın — uygulama çalışan CS2 pencerelerini tanımlı yerlere dizer.

> **Güvenlik ağı.** Dizmeden önce uygulama mevcut pencere konumlarını hatırlar. **Revert layout** düğmesi önceki konumları bir dakika içinde geri getirir.

![monitör tuvaliyle Layouts ekranı](../images/layouts-screen.png)

## 4.11. Sandboxes ekranı

**Amacı.** Sandbox'ları — Steam istemcilerinin çalıştığı yalıtılmış ortamları — yönetin.

**Konumu.** Yan çubuktaki sekizinci bölüm (`Ctrl+8`).

**Sandbox nedir.** Bir sandbox, tek bir Steam istemcisi için ayrı ve korumalı bir ortamdır. Farklı sandbox'lardaki hesaplar hiçbir zaman çakışmaz: oturum, dosya ya da iz paylaşmazlar. Bir hesap bir sandbox'a bağlıdır.

**Ne zaman kullanılır.** Burada sandbox'lar oluşturur ve durumlarını izlersiniz. Çoğu durumda hesap eklerken sandbox'lar otomatik atanır, bu yüzden buraya kasıtlı olarak nadiren gelirsiniz.

## 4.12. Settings ekranı

**Amacı.** Uygulamayı tercihlerinize göre uyarlayın.

**Konumu.** Yan çubuğun altındaki **Settings** bölümü (`Ctrl+,`).

**Yerleşim.** Solda bir ayar bölümleri listesi; sağda ayarların kendisi. Değişiklikler anında kaydedilir: her birinden sonra kısa bir **Saved** bildirimi belirir.

**Ayar bölümleri:**

| Bölüm | Neyi ayarlar |
|---|---|
| **General** | Windows ile başlatma, tepsiye küçültme, güncelleme kanalı |
| **Appearance** | Tema (**System / Dark / Light**), yoğunluk, yazı tipi ölçeği, azaltılmış hareket |
| **Accounts** | Hesap oluştururken davranış, silinenlerin saklanması |
| **Workflows** | Yeniden deneme politikası, eşzamanlı çalışma sınırları |
| **Sandboxes** | Sandbox klasörü, otomatik toparlanma |
| **Monitoring** | Veri yenileme hızı, uyarı eşikleri |
| **Notifications** | Önem düzeyine göre bildirimler ve sesler |
| **Layouts** | Varsayılan düzenler, çok monitörlü davranış |
| **Hotkeys** | Klavye kısayolları — yeniden atanabilir |
| **Advanced** | Günlük düzeyi, tanılama, ortam seçimi, varsayılanlara sıfırlama |
| **About** | Uygulama sürümü, veri ve günlük klasörlerini açma düğmeleri |

> **Not.** Bazı ayarlar (örneğin, sandbox klasörü ya da ortam) yalnızca yeniden başlatmadan sonra geçerli olur. Bu tür ayarların yanında bir “Requires restart” rozeti gösterilir.

![Settings ekranı](../images/settings-screen.png)

---

# 5. Temel iş akışları

Bu, en önemli bölümdür. Başlıca işler için eksiksiz adım adım yönergeler içerir. Her adım, ne göreceğinizi ve başarıyı nasıl doğrulayacağınızı anlatır.

## 5.1. Tek bir hesap ekleme

**Amaç.** Uygulamaya bir yeni Steam hesabı ekleyin.

**Gerekenler.** Hesabın kullanıcı adı ve parolası. Geçerliyse bir Steam Guard kodu.

### Adım 1 — Ekleme formunu açın

**Accounts** ekranına gidin ve araç çubuğundaki **Add Account** düğmesine tıklayın. `Ctrl+N` tuşlarına da basabilirsiniz.

**Beklenen sonuç.** Yeni hesap alanlarını içeren bir form açılır.

### Adım 2 — Bilgileri doldurun

Alanları doldurun:

- **Login** — zorunlu, benzersiz olmalı.
- **Password** — zorunlu.
- **Steam Guard secret** — varsa Steam Guard kodu (isteğe bağlı).
- **Nickname** — isteğe bağlı; ilk girişte otomatik alınabilir.
- **Tags** — gruplama için isteğe bağlı etiketler.
- **Sandbox binding** — **Auto-assign**, belirli bir sandbox ya da **None** seçin.
- **Workflow** — hemen atamak isterseniz başlatma senaryosu.

**Beklenen sonuç.** Kullanıcı adı zaten alınmışsa alan kırmızıyla vurgulanır ve bir açıklama verilir. Zayıf bir parola kehribar renginde vurgulanır — bu bir uyarıdır ve kaydetmeyi engellemez.

### Adım 3 — Hesabı kaydedin

Formdaki kaydet düğmesine tıklayın.

**Beklenen sonuç.** Form kapanır ve yeni hesap tabloda bir **Draft** durumuyla ya da bir sandbox'a bağlıysa başlatmaya hazır olarak belirir.

**Başarı işareti.** Hesap, **Accounts** ekranındaki tabloda görünür.

### İpuçları

- Formda **Validate immediately** seçeneğini açarsanız uygulama kullanıcı adını arka planda denetler ve sonucu bir bildirim olarak gösterir.
- Bir hesabın başlatılabilmesi için bir sandbox'a bağlı olması gerekir. En basit seçim **Auto-assign**'dır.

### Sık yapılan hatalar ve düzeltmeleri

- **“Login already in use.”** Bu kullanıcı adı uygulamada zaten var. Hesap listenizi kontrol edin — onu belki de eklemişsinizdir.
- **Sandbox unutuldu.** Sandbox'sız bir hesap başlatılamaz. Sonradan bağlam menüsü → **Bind sandbox** ile bir tane bağlayın.

![hesap ekleme formu](../images/accounts-add-form.png)

## 5.2. Bir dosyadan hesap listesini içe aktarma

**Amaç.** Bir dosyadan aynı anda birçok hesabı hızlıca ekleyin.

**Gerekenler.** Hesap listesi içeren bir dosya (TXT, CSV veya TSV). En basit TXT satır biçimi `login:password`'dür (ayrıca `login:password:steamguard:nickname` de kullanabilirsiniz).

### Adım 1 — İçe aktarma sihirbazını başlatın

**Accounts** ekranında **Import** düğmesinin yanındaki oka tıklayın ve bir kaynak seçin — örneğin, **From file…**. `Ctrl+I` tuşlarına da basabilirsiniz.

**Beklenen sonuç.** Adım adım bir içe aktarma sihirbazı açılır.

### Adım 2 — Kaynağı ve sandbox'ların nasıl atanacağını seçin

**Browse…** düğmesiyle dosyayı gösterin. Altta, sandbox'ların nasıl atanacağını seçin:

- **Auto-assign (round-robin)** — döngüsel dağıt (önerilir);
- **Bind to specific sandbox** — hepsini tek bir sandbox'a bağla;
- **Leave unbound** — sandbox'suz bırak.

İleri'ye tıklayın.

### Adım 3 — Verinin nasıl tanındığını kontrol edin

Sihirbaz, dosyanın ilk satırlarını bir tablo olarak gösterir. Verinin sütunlara doğru bölündüğünden emin olun. Ayırıcı yanlış algılandıysa elle ayarlayın.

**Beklenen sonuç.** Önizlemede kullanıcı adları ve parolalar kendi sütunlarındadır.

### Adım 4 — Alanları eşleştirin

Sütun başlıklarını gereken hücrelere sürükleyin: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Adım 5 — Satırların geçerli olduğunu kontrol edin

Sihirbaz her satırı işaretler: ✓ geçerli, ⚠ uyarı, ✕ hata. Hatalı satırlar hemen burada düzeltilebilir ya da atlanabilir.

**Beklenen sonuç.** Kaç hesabın ekleneceğini, kaçının yinelenen olduğunu ve kaçında hata olduğunu görürsünüz.

### Adım 6 — İçe aktarmayı onaylayın

**Import N accounts** düğmesine tıklayın.

**Beklenen sonuç.** Satır satır durumla bir ilerleme çubuğu belirir. Bittiğinde hesaplar tabloda görünür.

**Başarı işareti.** Tablodaki hesap sayısı, içe aktarılan sayı kadar artmıştır.

### Nasıl iptal edilir ve geri alınır

İçe aktarmayı çalışırken iptal ederseniz uygulama, zaten eklenmiş toplu işi geri almayı önerir. Özgün duruma dönmek için geri almayı onaylayın.

![içe aktarma sihirbazı, satır doğrulama adımı](../images/import-wizard-validation.png)

## 5.3. Birden fazla hesabı başlatma

**Amaç.** Aynı anda birkaç hesabı başlatın.

**Gerekenler.** Eklenmiş ve sandbox'lara bağlanmış hesaplar.

### Adım 1 — Hesapları seçin

**Accounts** ekranında ilk sütunda istediğiniz hesapları işaretleyin. Görünen hepsini seçmek için `Ctrl+A` tuşlarına basın.

**Beklenen sonuç.** Araç çubuğu toplu moda geçer ve kaç satırın seçili olduğunu gösterir, örneğin `12 selected`.

### Adım 2 — Seçili hesapları başlatın

Toplu araç çubuğundaki **Start** düğmesine tıklayın. `Ctrl+R` tuşlarına da basabilirsiniz.

**Beklenen sonuç.** Seçili hesapların durumu **Starting** olur. Uygulama her hesabı hazırlar ve başlatmaya başlar. Bilgisayar aşırı yüklenmesin diye başlatma gruplar hâlinde yapılır.

### Adım 3 — Başlatmayı bekleyin

Durum sütununu izleyin. Hesaplar **Running** durumuna geçene kadar bekleyin.

**Beklenen sonuç.** Başlatılan hesaplar, yanlarında bir çalışma süresi sayacıyla **Running** gösterir.

**Başarı işareti.** Seçili tüm hesaplar **Running** gösterir. Durum çubuğundaki etkin sayı artmıştır.

### İpuçları

- Her hesabı aynı anda başlatmak zorunda değilsiniz. Küçük bir grupla başlayın, her şeyin kararlı olduğundan emin olun, sonra daha fazlasını ekleyin.
- Tek bir hesabı başlatmak için: bir satır seçin ve **Start** düğmesine tıklayın ya da sağdaki ayrıntı bölmesindeki **Start** düğmesini kullanın.

### Sık yapılan hatalar ve toparlanma

- **Bir hesap çok uzun süre Starting'de kalıyor.** Giriş yavaş olabilir. Bekleyin; durum **Error**'a dönerse **Retry** düğmesini kullanın.
- **Bazı hesaplar başlamadı.** Toplu bir başlatmadan sonra bir özet, kaçının başarılı olduğunu ve kaçının başarısız olduğunu gösterir. Yalnızca onlarla ilgilenmek için **Filter to failed** düğmesine tıklayın.

![hesapların toplu başlatılması, Starting/Running durumları](../images/accounts-bulk-start.png)

## 5.4. Çalışan tüm hesapları durdurma

**Amaç.** Tüm etkin hesapları temiz bir şekilde kapatın.

### Adım 1 — Hesapları seçin

Çalışan hesapları seçin. Görünen hepsini seçmek için `Ctrl+A` tuşlarına basın.

### Adım 2 — Onları durdurun

Toplu araç çubuğundaki **Stop** düğmesine tıklayın ya da `Ctrl+.` (Ctrl ve nokta) tuşlarına basın.

**Beklenen sonuç.** Uygulama her hesabı temiz bir şekilde kapatır. Durum **Stopped** olur. Bir hesap yanıt vermezse uygulama bir süre sonra onu zorla kapatır.

**Başarı işareti.** Tüm hesaplar **Stopped** gösterir. Durum çubuğundaki etkin sayı azalmıştır.

### İpuçları

- **Stop** düzgün bir kapatmadır. Uygulama önce istemcileri doğru şekilde kapatmayı dener.
- Bir hesap maçtaysa önce oyun içi eylemleri bitirin, sonra durdurun.

## 5.5. Bir grup kurma ve sıraya sokma

**Amaç.** Birkaç hesaptan bir grup kurun ve birlikte eşleşme sırasına sokun.

**Gerekenler.** Giriş yapmış, çalışan (**Running**) birkaç hesap.

### Adım 1 — Bir grup oluşturun

**Matchmaking** ekranına gidin ve **Create Party** düğmesine tıklayın. `Ctrl+N` tuşlarına da basabilirsiniz.

**Beklenen sonuç.** Gruba hesap ekleyebileceğiniz ve ona bir ad verebileceğiniz bir pencere açılır.

### Adım 2 — Üye ekleyin ve kaydedin

Gruba 2 ila 5 hesap ekleyin, bir ad verin ve kaydedin.

**Beklenen sonuç.** Yeni grup, soldaki listede belirir.

### Adım 3 — Quorum'u kontrol edin

Grubu seçin ve sağdaki üyelerine bakın. Grubun **Quorum** durumunda olduğundan — yani tüm üyelerin giriş yapmış ve hazır olduğundan — emin olun.

**Beklenen sonuç.** Grup bir **✓ Quorum** rozeti gösterir. Bir üyede sorun varsa (örneğin, yavaş bir giriş) ayrı bir satır olarak gösterilir.

### Adım 4 — Grubu sıraya sokun

Seçili grup için **Queue** düğmesine (ya da `Ctrl+Q`) tıklayın. Tüm grupları aynı anda sıraya sokmak için araç çubuğundaki **Queue All** düğmesini kullanın.

**Beklenen sonuç.** Sıraya sokmadan önce uygulama denetimlerini yapar. Ardından tüm üyeler, konumları ve ağ gecikmeleri gösterilerek sıraya girer.

**Başarı işareti.** Üyeler sırada durumundadır ve bir bekleme süresi sayacı işlemektedir.

### İpuçları

- Sıraya sokmadan önce araç çubuğundan bölgeyi ve modu seçin (örneğin, `EU` ve `Premier`).
- Grup **Desync** durumuna girerse sırayı duraklatmak ve tutarlı bir durumu beklemek için **Re-sync** eylemini kullanın.

![üye konumlarıyla sırada bir grup](../images/matchmaking-party-queue.png)

## 5.6. Bir maç bulunduğunda ne olur

**Amaç.** Bir maç bulunduğu anda uygulamanın ne yaptığını anlayın.

**Gerekenler.** Sırada olan bir grup.

### Maç kabulü otomatiktir

Steam bir maç bulduğunda grup için belirgin bir **MATCH FOUND** afişi belirir. **Bir şeye tıklamanız gerekmez** — uygulama, verilen süre içinde tüm grup üyeleri için hazır olduğunu onaylar. Sizden herhangi bir eylem beklenmez.

**Beklenen sonuç.** Grup üyeleri maçı otomatik kabul eder; durumları **✓ Accepted** olur.

**Başarı işareti.** Tüm üyeler **Accepted** gösterir ve maç başlar.

> **İpucu.** Ekranı izlemeden bir maç bulunduğunu bilmek ister misiniz? **Settings → Notifications** bölümünde **Match found** için bir sesli uyarı açın. Kabul yine otomatik gerçekleşir — ses yalnızca sizi bilgilendirmek içindir.

### Grup desync olursa ne yapmalı

Bazen bir maç herkes için onaylanamaz — örneğin, bir üye sıradan düştüyse. Grup o zaman **Desync** durumuna girer. **Re-sync** eylemini kullanın, gerekirse sorunlu üyeyi **Drop member** ile çıkarın, sonra kalanları tekrar sıraya sokun.

![Match Found afişi](../images/matchmaking-match-found.png)

## 5.7. Bir çökme ya da uygulama yeniden başlatmasından sonra toparlanma

**Amaç.** Bir istemci çökmesinden ya da uygulama kapatılıp yeniden açıldıktan sonra çiftliği çalışır duruma döndürün.

**Gerekenler.** Ekstra bir şey yok — toparlanma büyük ölçüde otomatik olur.

### Otomatik olarak ne olur

- **Bir istemci çökmesinden sonra.** Steam ya da CS2 beklenmedik şekilde kapanırsa uygulama bunu fark eder, hesabı **Crashed** durumuyla işaretler ve bir **Restart** düğmesiyle bir bildirim gösterir. Toparlanma çoğu zaman birkaç saniye içinde kendi başına gerçekleşir.
- **Bir uygulama yeniden başlatmasından sonra.** Başlangıçta uygulama, önceki oturumdan kalan Steam ve CS2 süreçlerini arar ve onları yeniden yönetimine alır. Bu sırada durum çubuğunda bir **Recovering** göstergesi belirir. Yeniden bağlanan hesaplar kısa süre “Reattached” olarak işaretlenir.

### Elle ne yapmalı

1. **Dashboard** ekranını açın ve **Failures & Crashes** tablosuna bakın.
2. Çöken bir hesap için bildirimdeki, hesap satırındaki ya da ayrıntı bölmesindeki **Restart** düğmesine tıklayın.
3. Uygulama bildirim merkezinde bir **Orphan process** bildirirse **Adopt** ya da **Kill** seçin.

**Başarı işareti.** Hesaplar yeniden **Running** durumundadır, kırmızı çökme işaretleri kaybolmuştur ve durum çubuğunda etkin bir **Recovering** göstergesi yoktur.

### İpuçları

- Bir çökmeden hemen sonra her şeyi elle yeniden başlatmayın — önce otomatik toparlanmaya birkaç saniye tanıyın.
- Çökmeler yinelenirse yükü görmek için **Monitoring** ekranını açın: bu bilgisayarın kaldırabileceğinden daha fazla hesap çalıştırıyor olabilirsiniz.

![durum çubuğundaki Recovering göstergesi](../images/status-recovering.png)

---

# 6. Sık yapılan işler («İstiyorum ki…»)

Sık karşılaşılan amaçlara kısa yanıtlar. Tam yönergeler için 5. bölümdeki bağlantıları izleyin.

## «Yeni hesaplar eklemek istiyorum»

- **Ne zaman gerekir.** Yeni Steam hesaplarınız var.
- **Ne yapmalı.** Tek bir hesap için **Accounts** ekranındaki **Add Account** düğmesini kullanın. Aynı anda birçoğu için **Import** düğmesini ve içe aktarma sihirbazını kullanın.
- **Ne olur.** Hesaplar tabloda belirir ve (bir sandbox'a sahip olunca) başlatmaya hazır olur.
- Devamı: [5.1](#51-tek-bir-hesap-ekleme), [5.2](#52-bir-dosyadan-hesap-listesini-i̇çe-aktarma).

## «Steam'i başlatmak istiyorum»

- **Ne zaman gerekir.** Bir hesabın Steam'e giriş yapmasını istiyorsunuz.
- **Ne yapmalı.** **Accounts** ekranında hesabı seçip **Start** düğmesine tıklayın.
- **Ne olur.** Uygulama, Steam'i hesabın sandbox'ında başlatır ve giriş yapar. Durum **Starting → Running** olur.

## «CS2'yi başlatmak istiyorum»

- **Ne zaman gerekir.** Steam zaten çalışıyor ve oyunu başlatmanız gerekiyor.
- **Ne yapmalı.** Hesabı **Start** ile başlatmak, onu (atanan iş akışı içeriyorsa) CS2'yi başlatma dâhil tüm senaryodan geçirir.
- **Ne olur.** Steam'e giriş yaptıktan sonra uygulama CS2'yi başlatır. Adımları **Workflows** ekranında izleyebilirsiniz.

## «Bir lobi oluşturmak istiyorum»

- **Ne zaman gerekir.** Hesapları bir oyun lobisinde toplamanız gerekiyor.
- **Ne yapmalı.** **Matchmaking** ekranında **Create Party** ile bir grup kurun ve üyeler ekleyin.
- **Ne olur.** Uygulama seçili hesapları bir grupta birleştirir ve onları tutarlı bir duruma (quorum) getirmeye yardımcı olur.
- Devamı: [5.5](#55-bir-grup-kurma-ve-sıraya-sokma).

## «Eşleşmeyi başlatmak istiyorum»

- **Ne zaman gerekir.** Grup kuruldu ve hazır.
- **Ne yapmalı.** Grubu seçin ve **Queue** (ya da hepsi için **Queue All**) düğmesine tıklayın.
- **Ne olur.** Üyeler sıraya girer; konumlarını ve bekleme sürelerini görürsünüz.

## «Çalışan tüm oturumları durdurmak istiyorum»

- **Ne zaman gerekir.** Bitirme vakti geldi.
- **Ne yapmalı.** Hesapları seçin (`Ctrl+A`) ve **Stop** düğmesine tıklayın.
- **Ne olur.** Uygulama istemcileri temiz bir şekilde kapatır ve durumlar **Stopped** olur.
- Devamı: [5.4](#54-çalışan-tüm-hesapları-durdurma).

## «Bir çökmeden sonra toparlanmak istiyorum»

- **Ne zaman gerekir.** Bir istemci çöktü ya da uygulama yeniden başlatıldı.
- **Ne yapmalı.** Otomatik toparlanmaya birkaç saniye tanıyın; gerekirse çöken hesap için **Restart** düğmesine tıklayın.
- **Ne olur.** Uygulama hesapları çalışır duruma döndürür.
- Devamı: [5.7](#57-bir-çökme-ya-da-uygulama-yeniden-başlatmasından-sonra-toparlanma).

## «Pencereleri ekranda dizmek istiyorum»

- **Ne zaman gerekir.** CS2 pencerelerini monitörünüzde düzenli dizmek istiyorsunuz.
- **Ne yapmalı.** **Layouts** ekranında bir preset oluşturun ve **Apply** / **Snap windows** düğmesine tıklayın.
- **Ne olur.** Çalışan pencereler tanımlı yerlere taşınır.

---

# 7. Özellik başvurusu

Bu bölüm, amacı, konumu ve ayrıntılarıyla tekil özellikleri ele alır.

## 7.1. Hesap arama ve filtreler

**Amacı.** Büyük bir listede ihtiyacınız olan hesapları hızlıca bulun.

**Konumu.** **Accounts** ekranı araç çubuğu: arama alanı ve **Filters** düğmesi.

**Nasıl kullanılır.**
- Arama alanına yazın (`Ctrl+F`). Parçalarla arayabilirsiniz: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- **Filters** düğmesine tıklayın (bu ekranda `Ctrl+K` filtreler penceresini açar), duruma, rütbeye, sandbox'a, iş akışına ya da etiketlere göre koşullar belirleyin ve kümeyi bir preset olarak kaydedin.

**Beklenen davranış.** Tablo anında yalnızca eşleşen hesapları gösterir. Etkin filtreler araç çubuğunun altında bir çip satırı olarak belirir.

**İpucu.** Sık kullanılan koşul kümelerini preset olarak kaydedin — araç çubuğundaki açılır menüden erişilebilir.

## 7.2. Gruplama ve sütun düzeni

**Amacı.** Tabloyu işinize uyacak şekilde düzenleyin.

**Konumu.** **Accounts** ekranı araç çubuğu: **Density**, **Columns** ve **Group** düğmeleri.

**Nasıl kullanılır.**
- **Group**, hesapları duruma, iş akışına, sandbox'a, etikete ya da rütbeye göre gruplamanızı sağlar. Gruplar sayaçlar gösterir, örneğin `Running (24)`.
- **Columns** — görünen sütunların kümesi. Yerleşik kümeler kullanılabilir: **Operational**, **Identity**, **Audit**, **Compact**. Kendi kümenizi kaydedebilirsiniz.
- **Density** — satır yüksekliği (daha derli toplu ya da daha ferah).

## 7.3. Hesap bağlam menüsü

**Amacı.** Bir hesaba ait her eyleme hızlı erişim.

**Konumu.** Bir hesap satırına sağ tıklayın.

**Neler var.** Düzenle, kullanıcı adını ya da Steam ID'yi kopyala, başlat/durdur/yeniden başlat, sandbox bağla ve çöz, iş akışı ata, yeniden kimlik doğrula (**Re-auth**), girişi yokla (**Probe login now**), etiketlerle çalış, dışa aktar, kopyala ve sil.

## 7.4. Toplu işlemler

**Amacı.** Aynı anda birçok hesaba tek bir eylem uygulayın.

**Konumu.** Seçim modundaki (en az bir satır işaretliyken) **Accounts** ekranı araç çubuğu.

**Nasıl kullanılır.** Hesapları işaretleyin, sonra ihtiyacınız olan düğmeye tıklayın: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export** ya da **Delete**.

**Beklenen davranış.** Hesap başına bir ilerleme görünümüyle bir pencere belirir. İşlemi çalışırken iptal edebilirsiniz.

**Kısıtlama.** Beş veya daha fazla hesap silerken uygulama, `DELETE` sözcüğünü yazarak onaylamanızı ister.

## 7.5. Hesapları dışa aktarma

**Amacı.** Hesap verilerini bir dosyaya kaydedin.

**Konumu.** Araç çubuğundaki ya da bağlam menüsündeki **Export** düğmesi.

**Nasıl kullanılır.** Bir biçim seçin: **TXT** (login:password), **CSV** (tüm alanlar) ya da **JSON** (tam kayıt).

> **Uyarı.** Parolaları dışa aktarmak ayrı bir onay gerektirir — uygulama bir onay kutusunu işaretlemenizi ister. Bu tür dosyaları dikkatli kullanın.

## 7.6. Bir hesabı kopyalama

**Amacı.** Bir başlangıç noktası olarak bir hesabın kopyasını hızlıca oluşturun.

**Konumu.** Satır bağlam menüsü → **Clone…**.

**Beklenen davranış.** Alanları önceden doldurulmuş bir form açılır (kullanıcı adı `original_copy` olur), Steam Guard kodu ve sandbox bağlantısı dışında — onları yeniden ayarlarsınız.

## 7.7. Workflow'lar: başlat, duraklat, durdur

**Amacı.** Otomatik senaryoları yönetin.

**Konumu.** **Workflows** ekranı.

**Nasıl kullanılır.**

| Eylem | Ne yapar | Onay ister mi? |
|---|---|---|
| **Start** | Seçili hesaplar için senaryoyu çalıştırır | 10'dan fazla hesap başlatırken |
| **Pause** | Mevcut adımdan sonra nazikçe duraklatır | Hayır |
| **Resume** | Mevcut noktadan devam eder | Hayır |
| **Stop** | Senaryoyu temizlikle bitirir | Evet |
| **Restart** | Durdurur ve baştan başlatır | Evet (toplu işlem için) |
| **Skip step** | Mevcut adımı tamamlandı işaretler ve geçer | Evet |
| **Retry now** | Mevcut adımı hemen yeniden dener | Hayır |

**İpucu.** Ayrıntı bölmesindeki **State Machine** sekmesi, bir senaryonun hangi adımda olduğunu net gösterir.

## 7.8. Bir sandbox'a bağlama

**Amacı.** Bir hesap için, olmadan başlatılamayacağı yalıtılmış bir ortam ayırın.

**Konumu.** Bağlam menüsü → **Bind sandbox…** ya da **Bind sandbox** toplu işlemi.

**Nasıl kullanılır.** Bir yöntem seçin: round-robin, önce boş olanları doldur ya da belirli bir sandbox.

**Kısıtlama.** Bir hesap, bir sandbox. Seçilen sandbox zaten kullanımdaysa uygulama onu önceki hesaptan boşaltmayı önerir.

## 7.9. Pencere düzenleri

**Amacı.** CS2 pencerelerini bir hazır düzen kullanarak dizin.

**Konumu.** **Layouts** ekranı.

**Nasıl kullanılır.** Bir preset oluşturun, monitör tuvaline slot'lar yerleştirin, bağlamaları ayarlayın ve **Apply** düğmesine tıklayın.

**İpucu.** Bir düzen tutmadıysa, **Revert layout** düğmesi önceki pencere konumlarını bir dakika içinde geri getirir.

## 7.10. Bildirim merkezi

**Amacı.** Tüm uygulama bildirimleri için tek bir yer.

**Konumu.** Üst çubuktaki bildirim rozeti ya da `Ctrl+Shift+N`.

**Nasıl kullanılır.** Panel sağda açılır. **All**, **Errors**, **Warnings** ve **Info** sekmeleri arasında geçiş yapın. Her giriş için kaynağa gidebilir, yeniden deneyebilir ya da kapatabilirsiniz. **Clear all** düğmesi listeyi boşaltır.

**Kısıtlama.** Son 200 giriş tutulur; daha eskiler kaldırılır.

---

# 8. Durumlar ve göstergeler

Her durumun bir rengi, bir simgesi ve bir etiketi vardır. Aşağıda her birinin ne anlama geldiği ve bir eylem gerekip gerekmediği var.

| Durum | Simge | Ne anlama gelir | Eylem gerekir mi |
|---|---|---|---|
| **OK / Success** | ✓ (yeşil) | Hesap çevrimiçi, giriş başarılı | Hayır |
| **Running** | ▶ (mavi) | Hesap ya da iş akışı çalışıyor | Hayır |
| **Starting** | ◐ (mor) | Başlatma sürüyor, geçici bir durum | Bitmesini bekleyin |
| **Queued** | ⏱ (gri) | Sırada bekliyor | Hayır |
| **Stopped** | ■ (gri) | Durdurulmuş, boşta | İsteğe bağlı — başlatabilirsiniz |
| **Paused** | ⏸ (kehribar) | Senaryo duraklatıldı | Devam için **Resume** düğmesine tıklayın |
| **Warning** | △ (kehribar) | Kritik olmayan bir anormallik | Ayrıntıları kontrol edin; çoğu zaman devam edebilirsiniz |
| **Error** | ✕ (kırmızı) | Toparlanabilir bir arıza | **Retry** düğmesine tıklayın ya da nedeni araştırın |
| **Crashed** | ☠ (koyu kırmızı, yanıp söner) | Süreç beklenmedik şekilde kapandı | **Restart** düğmesine tıklayın |
| **Match Found** | ◎ (yeşil, yanıp söner) | Bir CS2 maçı bulundu | Hiçbir şey — uygulama hazır olduğunu otomatik onaylar |
| **Desync** | ⛓ (turuncu) | Grup üyeleri senkron değil | **Re-sync** çalıştırın |
| **Info** | ⓘ (mavi) | Nötr bir mesaj | Hayır |

**Ek göstergeler:**

- **Recovering** — uygulama başlangıcında durum çubuğunda mavi bir gösterge: önceki oturumdan süreçler yeniden yönetime alınıyor. Bitmesini bekleyin.
- **Reattached** — bir hesap satırında geçici bir işaret: süreç yeniden başlatmadan sonra başarıyla devralındı.
- **Frozen at HH:mm:ss** — **Monitoring** ekranında, veri gösteriminin donmuş olduğu anlamına gelir (**Live** modda değil). Canlı veriyi geri getirmek için **Live**'a geçin ya da **Freeze**'i kapatın.

**Ayrıntıları nasıl görürsünüz.** Bir ipucu almak için bir durum simgesinin üzerine gelin: durumun ne zamandır sürdüğü, hesabın hangi adımda olduğu ve son olayın ne olduğu.

![hesap tablosundaki durum örnekleri](../images/status-badges.png)

---

# 9. Bildirimler

Uygulama olayları üç şekilde bildirir: **toast'lar** (köşede belirip kaybolur), **durum çubuğu** (altta kalıcı bir özet) ve **satır içi afişler** (belirli bir ekrana bağlı).

## Toast'lar

Sağ alt köşede belirirler.

| Bildirim | Neden belirir | Ne anlama gelir | Ne yapmalı | Yok sayılabilir mi |
|---|---|---|---|---|
| **Saved** | Bir ayarı değiştirdiniz | Değişiklik kaydedildi | Hiçbir şey | Evet, kendiliğinden kaybolur |
| İşlem başarısı (yeşil) | Bir eylem başarıyla tamamlandı | Her şey yolunda | Hiçbir şey | Evet, ~5 saniye sonra kaybolur |
| Uyarı (kehribar) | Kritik olmayan bir anormallik fark edildi | Bir bakmaya değer | İsteğe bağlı olarak ayrıntıları görün | Genelde evet, ~10 saniye sonra kaybolur |
| Hata (kırmızı) | Bir işlem başarısız oldu | Eylem gerekli | **View** ya da **Retry** düğmesine tıklayın | Hayır, kapatılana dek kalır |
| Çökme | Bir istemci beklenmedik şekilde kapandı | Bir hesap çöktü | **Restart** düğmesine tıklayın ya da dökümü açın | Hayır, onaylanana dek kalır |

**Bilmekte fayda var.**
- Bir bildirimin üzerine gelmek otomatik kapanma sayacını durdurur — onu rahatça okuyabilirsiniz.
- Aynı bildirimler, bir sayaçla tek bir bildirimde toplanır, örneğin `… failed (×4)`.

## Durum çubuğu

Durum çubuğunun sağ tarafında, en önemli okunmamış bildirim gösterilir, örneğin `● 3 errors`. Tıklamak bildirim merkezini açar.

## Satır içi afişler

Bir ekranın üstünde belirirler ve bütünüyle o ekrana uygulanırlar. Örnek: `⚠ Steam network degraded — 12 accounts retrying login`. Engelleyici değilse bir afiş **Dismiss** düğmesiyle kapatılabilir. Engelleyici afişler (örneğin, bir hizmet kullanılamadığında) sorun çözülene dek kalır.

## Sesli uyarılar

Ses varsayılan olarak kapalıdır. Belirli olaylar için (örneğin, **Match found** ya da **Crash**) **Settings → Notifications** bölümünde açabilirsiniz. **Match found** için bir ses, ekranı izlemeden bir maç bulunduğunu bilmek için kullanışlıdır — maç kabulünün kendisi otomatik gerçekleşir.

![View ve Retry düğmeleriyle bir hata toast'ı](../images/notification-error-toast.png)

---

# 10. Hatalar ve sorun giderme

Bir çiftliği çalıştırırken hatalar sıradandır ve uygulama bunları çözmenize yardımcı olur. Aşağıda “Sorun → Olası neden → Çözüm → Beklenen sonuç” biçiminde sık karşılaşılan durumlar var.

## Lisans etkinleştirilemiyor

**Sorun.** Anahtarı girerken uygulama devam etmenize izin vermiyor.

| Mesaj | Olası neden | Çözüm |
|---|---|---|
| “License key invalid” | Anahtar yazım hatasıyla girildi | Yazımı kontrol edin. Anahtarı **Paste from clipboard** ile yapıştırmak daha kolaydır |
| “Used on max devices” | Lisans zaten en fazla sayıda cihazda kullanılıyor | Lisansı başka bir cihazda serbest bırakın, sonra tekrar deneyin. **Manage devices** düğmesi cihaz yönetimine götürür |
| “Cannot reach license server” | Lisans sunucusuna bağlantı yok | İnternet bağlantınızı kontrol edin ve **Retry** düğmesine tıklayın |

**Beklenen sonuç.** Doğru bir anahtar ve sunucuya bağlantı ile etkinleştirme penceresi kapanır ve **Dashboard** açılır.

## Bir hesap başlatılamıyor

**Sorun.** **Start** düğmesine tıkladınız ama hesap **Running**'e geçmiyor.

- **Olası neden.** Hesap bir sandbox'a bağlı değil.
  **Çözüm.** Hesabın bağlam menüsü → **Bind sandbox…** açın ve bir sandbox atayın.
- **Olası neden.** Yeniden kimlik doğrulama gerekiyor (bayat giriş bilgileri); satırın yanında bir “Reauth required” işareti var.
  **Çözüm.** Bağlam menüsü → **Re-auth (Steam Guard)**.
- **Olası neden.** Steam, girişleri geçici olarak hız sınırladı.
  **Çözüm.** Yaklaşık bir dakika bekleyin ve **Retry** düğmesine tıklayın.

**Beklenen sonuç.** Durum **Starting → Running** olur.

## Steam uzun süre Waiting/Starting'de kalıyor

**Sorun.** Hesap giriş aşamasında takılı kaldı.

- **Olası neden.** Yavaş bir giriş ya da geçici Steam ağ sorunları.
  **Çözüm.** Biraz zaman tanıyın. Bir **Error** durumu belirirse **Retry** düğmesine tıklayın. Steam ağı kararsızsa üstte bir uyarı afişi belirir — toparlanmasını bekleyin.

**Beklenen sonuç.** Hesap giriş yapar ve **Running**'e geçer.

## Bir istemci çöktü

**Sorun.** Hesap **Crashed** durumunu aldı.

- **Olası neden.** CS2 ya da Steam istemcisi beklenmedik şekilde kapandı.
  **Çözüm.** Beliren bildirimde **Restart** düğmesine tıklayın. Toparlanma çoğu zaman zaten otomatik sürmektedir. Çökme ayrıntıları **Monitoring** ekranındaki **Crashes & Warnings** akışındadır.

**Beklenen sonuç.** Hesap yeniden başlar ve **Running**'e döner.

## Bir grup Desync'e girdi

**Sorun.** Grup **Desync** durumunda — üyeler tutarsız bir durumda.

- **Olası neden.** Bir üye bir maçı kabul etti, bir başkası zamanında etmedi ya da biri sıradan düştü.
  **Çözüm.** Sırayı duraklatmak ve tutarlılığı beklemek için **Re-sync** düğmesine tıklayın. Bir hesap soruna yol açıyorsa onu **Drop member** ile çıkarın ve kalanları tekrar sıraya sokun.

**Beklenen sonuç.** Grup **Quorum** durumuna döner ve tekrar sıraya sokulmaya hazır olur.

## Bir toplu başlatma hatalarla bitti

**Sorun.** Toplu bir **Start**'tan sonra bazı hesaplar başlamadı.

- **Çözüm.** Özette **Filter to failed** düğmesine tıklayın — tablo yalnızca sorunlu hesapları gösterir. Her birini yukarıdaki nedenlere göre çözün ve tekrar başlatın.

**Beklenen sonuç.** Nedenler çözüldükten sonra tekrarlanan bir **Start**, hesapları **Running**'e taşır.

## Bir ekranın verisi yüklenmiyor

**Sorun.** Ekranın içeriği yerine bir afiş ya da bir hizmetin kullanılamadığına dair bir mesaj var.

- **Olası neden.** Bir arka plan hizmeti geçici olarak kullanılamıyor.
  **Çözüm.** **Retry** düğmesine tıklayın. Yardımcı olmazsa ayrıntıları görmek için **Open logs** düğmesine tıklayın ya da uygulamayı yeniden başlatın.

**Beklenen sonuç.** Ekran yüklenir ve güncel veriyi gösterir.

## Uygulama bir Orphan process bildiriyor

**Sorun.** Bildirim merkezinde “Orphan process … — Adopt or Kill?” gibi bir mesaj.

- **Olası neden.** Önceki oturumdan, bir hesaba otomatik bağlanamayan bir süreç kaldı.
  **Çözüm.** Süreç gerekliyse **Adopt** (yönetime al), değilse **Kill** (bitir) seçin.

**Beklenen sonuç.** Süreç listesi düzene sokulur.

## Bilgisayar yavaş ve çökmeler artıyor

**Sorun.** Genel kararsızlık, sık arızalar.

- **Olası neden.** Bilgisayarın kaldırabileceğinden daha fazla hesap çalışıyor.
  **Çözüm.** **Monitoring** ekranını açın ve **CPU** ile **RAM**'e bakın. Değerler sınırlarına yakınsa **Stop** ile bazı hesapları durdurun.

**Beklenen sonuç.** Yük düşer ve çalışma kararlı hâle gelir.

> **Hata kodları.** Hata ayrıntıları `[E-1042]` gibi kısa bir kod içerir. Onu kopyalayıp destekle iletişime geçerken kullanabilirsiniz. Kodların tam bir başvurusu **Help → Error reference** aracılığıyla kullanılabilir.

![Retry / Open logs düğmeleriyle örnek bir hata ekranı](../images/error-screen.png)

---

# 11. En iyi uygulamalar

## Hesapları hazırlama

- Hesapları **Import** ile liste hâlinde ekleyin — daha hızlıdır ve daha az yazım hatası olur.
- Belirli bir bağlantıya ihtiyacınız yoksa sandbox atamasını **Auto-assign** olarak bırakın.
- Hesapları gruplamak ve hızlıca filtrelemek için **Tags** kullanın.

## Çok sayıda hesabı başlatma

- Gruplar hâlinde başlatın: küçük bir grupla başlayın, kararlılığı doğrulayın, sonra daha fazlasını ekleyin.
- Yükü gerçek zamanlı izlemek için **Dashboard** ya da **Monitoring** ekranını açık tutun.
- Aynı anda önerilen 4–10 CS2 hesabını hedefleyin; güçlü bir PC'de daha fazlasını, zayıf makinelerde daha azını çalıştırabilirsiniz.

## Düzenlerle çalışma

- Farklı durumlar için önceden birkaç preset hazırlayın (örneğin, “4-stack”, “single focused”).
- Bir düzen ters gittikten sonra, bir dakikalık geri alma penceresi etkinken hemen **Revert layout** kullanın.

## Güvenle durdurma

- Hesapları pencereleri elle kapatmak yerine **Stop** düğmesiyle (düzgün bir kapatma) durdurun.
- Uygulamadan çıkmadan önce etkin hesapları durdurun. Senaryolar çalışırken uygulamayı kapatmaya çalışırsanız uyarır.

## Kesintilerden kaçınma

- Sıraya sokmadan önce grubun **Quorum** durumunda olduğundan emin olun.
- Steam ağ durumuna dair afişleri izleyin — kararsızken beklemek daha iyidir.

## Kararlı çalışmayı sürdürme

- **Dashboard**'u düzenli kontrol edin — genel durumu saniyeler içinde gösterir.
- Aynı anda çalışan hesap sayısını bilgisayarınızın kapasitesi içinde tutun.
- Elle müdahale etmeden önce otomatik toparlanmanın birkaç saniye çalışmasına izin verin.

---

# 12. Sıkça sorulan sorular

**Bir hesabı neden başlatamıyorum?**
Büyük olasılıkla hesap bir sandbox'a bağlı değildir — biri olmadan başlatılamaz. Bağlam menüsü → **Bind sandbox…** ile bir tane bağlayın. Bir başlatma, yeniden kimlik doğrulama gereğiyle de engellenebilir (bir “Reauth required” işareti) — o durumda **Re-auth** çalıştırın.

**Steam neden uzun süre bekleme durumunda kalıyor?**
Bu genellikle yavaş bir giriş ya da geçici Steam ağ gecikmeleridir. Biraz zaman tanıyın. Bir **Error** durumu belirirse **Retry** düğmesine tıklayın.

**Bir iş akışını nasıl yeniden başlatırım?**
İhtiyacınız olan hesapları ya da instance'ları seçin ve **Restart** düğmesine (ya da `Ctrl+Shift+R`) tıklayın. Toplu bir işlem için uygulama onay ister.

**Uygulama kapanırsa ne olur?**
Hesaplarınız ve ayarlarınız kaydedilir. Sonraki çalıştırmada uygulama, önceki oturumun süreçlerini yeniden yönetime almaya çalışır — durum çubuğunda bir **Recovering** göstergesi belirir. Kapandığında senaryolar etkinse uygulama sizi önceden uyarır.

**Her şeyin çalıştığını nasıl anlarım?**
Alttaki durum çubuğunu ve **Dashboard**'u kontrol edin. Normal çalışmanın işaretleri: **Running** durumundaki hesaplar, **Errors** kartında ya da **Failures & Crashes** tablosunda kırmızı işaretlerin olmaması ve **CPU** ile **RAM** yükünün normal aralıklarda olması.

**Parolalarım nerede saklanır?**
Yalnızca bilgisayarınızda. Windows'un yerleşik korumasıyla şifrelenir, hiçbir zaman düz metin olarak kaydedilmez ve hiçbir yere gönderilmez.

**FarmPanel benim yerime oynar mı?**
Hayır. Bir bot ya da otomatik çiftçi değildir. Uygulama başlatmayı, izlemeyi, lobi kurmayı ve toparlanmayı yönetir; tüm oyun içi eylemler sizin tarafınızdan yapılır.

**Lisans anahtarını her seferinde girmek zorunda mıyım?**
Hayır. Anahtar bir kez, ilk etkinleştirme sırasında girilir. Ondan sonra uygulama doğrudan **Dashboard**'a açılır.

**Düğmenin nerede olduğunu unuttuysam bir eylemi nasıl hızlıca bulurum?**
Komut paletini açmak için `Ctrl+K` tuşlarına basın. Bir eylemin, ekranın ya da hesap kullanıcı adının adını yazmaya başlayın ve listeden istediğinizi seçin.

**İzlemeyi ikinci bir monitöre taşıyabilir miyim?**
Evet. **Monitoring** ekranında ayır düğmesine tıklayın — ekran, ikinci bir monitöre yerleştirebileceğiniz ayrı bir pencere olarak açılır. Konumu hatırlanır.

**Ayarları varsayılanlarına nasıl sıfırlarım?**
**Settings → Advanced** bölümünde **Reset to defaults** vardır. Yanlışlıkla tıklamalara karşı uygulama, metin yazarak onaylamanızı ister.

---

*FarmPanel Kullanım Kılavuzu'nun sonu.*

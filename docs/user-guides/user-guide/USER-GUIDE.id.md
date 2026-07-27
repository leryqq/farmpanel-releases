# Panduan Pengguna FarmPanel

**Panel kontrol untuk farm akun Steam dan CS2 Anda di Windows**

Versi dokumen: 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · [Português](USER-GUIDE.pt.md) · [Français](USER-GUIDE.fr.md) · [Türkçe](USER-GUIDE.tr.md) · **Bahasa Indonesia** · [Tiếng Việt](USER-GUIDE.vi.md) · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Cara membaca panduan ini.** Tombol, tab, dan status muncul di aplikasi persis seperti yang tertulis dalam **tebal** (misalnya, **Add Account**, **Start**, **Running**), sehingga Anda selalu mengeklik hal yang tepat. Setiap prosedur memberi tahu apa yang harus diklik, apa yang terjadi berikutnya, dan cara memastikan keberhasilan.

## Daftar Isi

1. [Pengantar](#1-pengantar)
2. [Sebelum memulai](#2-sebelum-memulai)
3. [Peluncuran pertama](#3-peluncuran-pertama)
4. [Ikhtisar antarmuka](#4-ikhtisar-antarmuka)
5. [Alur kerja inti](#5-alur-kerja-inti)
6. [Tugas umum («Saya ingin…»)](#6-tugas-umum-saya-ingin)
7. [Referensi fitur](#7-referensi-fitur)
8. [Status dan indikator](#8-status-dan-indikator)
9. [Notifikasi](#9-notifikasi)
10. [Kesalahan dan pemecahan masalah](#10-kesalahan-dan-pemecahan-masalah)
11. [Praktik terbaik](#11-praktik-terbaik)
12. [Pertanyaan yang sering diajukan](#12-pertanyaan-yang-sering-diajukan)

---

# 1. Pengantar

## Apa itu FarmPanel

**FarmPanel** adalah aplikasi desktop Windows yang membantu Anda mengelola banyak akun Steam dan klien Counter-Strike 2 dari satu jendela. Alih-alih membuka puluhan jendela Steam secara manual, mengawasi masing-masing, dan memulai ulang yang macet, Anda mengelola seluruh farm akun secara terpusat — dari satu panel yang jelas.

FarmPanel meluncurkan klien, mengisolasi akun satu sama lain, mengawasi keadaannya secara waktu nyata, dan memulihkannya secara otomatis setelah kegagalan.

> **Penting.** FarmPanel **bukan bot dan bukan auto-farmer**. Ia tidak bermain untuk Anda dan tidak meniru tindakan di dalam gim. Ia mengelola segala sesuatu yang terjadi *di sekitar* gim: meluncurkan klien, undangan lobi, pemulihan setelah kegagalan, dan visibilitas langsung untuk setiap akun. Semua tindakan di dalam gim dilakukan oleh orang sungguhan.

## Masalah apa yang dipecahkannya

Jika Anda punya lebih dari satu akun, rutinitas ini pasti terasa akrab:

- Anda harus meluncurkan puluhan klien Steam dan CS2;
- setiap akun harus berjalan terpisah, tanpa mengganggu yang lain;
- membangun lobi dan mengirim undangan secara manual itu lambat dan melelahkan;
- CS2 yang mogok harus segera disadari dan dimulai ulang tepat waktu;
- sulit membedakan siapa yang sudah di dalam pertandingan dan siapa yang macet saat memuat.

FarmPanel menghapus rutinitas ini dan membawa setiap operasi ke dalam satu aplikasi.

## Untuk siapa

Aplikasi ini dibuat untuk siapa saja yang perlu mengelola banyak akun Steam dan CS2 secara terpusat — dari segelintir hingga beberapa ratus — dengan peluncuran otomatis, pemantauan langsung, dan pemulihan andal setelah kegagalan.

## Apa yang bisa Anda lakukan

- Simpan semua akun di satu tempat dan temukan cepat yang Anda butuhkan.
- Mulai dan hentikan akun satu per satu atau sekaligus.
- Isolasi setiap akun di lingkungannya sendiri yang terlindungi (sebuah sandbox).
- Bangun party dari akun-akun dan antrekan mereka untuk matchmaking bersama.
- Awasi beban komputer, kesehatan proses, dan mogok secara waktu nyata.
- Pulihkan akun secara otomatis setelah mogok atau setelah aplikasi ditutup.
- Atur jendela CS2 di seluruh monitor Anda menggunakan tata letak siap pakai.

![Layar utama FarmPanel (Dashboard)](../images/dashboard-overview.png)

---

# 2. Sebelum memulai

## Persyaratan sistem

| Item | Minimum | Disarankan |
|---|---|---|
| Sistem operasi | Windows 10 atau 11 (64-bit) | Windows 10 / 11 (64-bit) |
| Memori | 8 GB | 32 GB |
| Disk | Apa saja | SSD |
| Akun bersamaan | 2 | 4–10 akun CS2 |
| Resolusi layar | Area kerja setidaknya selebar 1280 piksel | Full HD (1920×1080) atau lebih tinggi |

## Apa yang perlu disiapkan lebih dulu

- **Pemasang FarmPanel** — sebuah berkas bernama `Setup.exe` yang Anda unduh dari halaman unduhan resmi.
- **Kunci lisensi** — Anda menerimanya bersama pembelian. Bentuknya seperti ini: `XXXX-XXXX-XXXX-XXXX-XXXX` (lima kelompok berisi empat karakter).
- **Detail akun Steam Anda** — nama pengguna dan kata sandi, serta kode Steam Guard jika Anda memakainya. Anda bisa memasukkannya satu per satu atau mengimpor daftar dari berkas.
- **Koneksi internet** — diperlukan pada peluncuran pertama untuk mengaktifkan lisensi, dan sesudahnya agar Steam dan CS2 bisa bekerja.

## Izin

- Pemasangan **tidak memerlukan hak administrator** — aplikasi terpasang hanya untuk akun pengguna Anda.
- Saat Anda menjalankan pemasang pertama kali, Windows mungkin menampilkan jendela **SmartScreen** biru (“Windows protected your PC”) — ini peringatan rutin untuk program baru. Klik **More info**, lalu **Run anyway**.
- Aplikasi mungkin memerlukan akses jaringan (untuk Steam) dan akses ke aturan Windows Firewall. Jika muncul permintaan firewall, izinkan akses.

## Di mana data Anda disimpan

Nama pengguna dan kata sandi dienkripsi dengan proteksi bawaan Windows dan disimpan **hanya di komputer Anda**. Semua itu tidak pernah disimpan sebagai teks biasa dan tidak pernah dikirim ke mana pun.

---

# 3. Peluncuran pertama

Berikut jalur dari pemasangan hingga panel siap pakai. Ikuti langkah-langkahnya secara berurutan.

## Langkah 1. Pasang aplikasi

1. Unduh pemasang `Setup.exe` dari halaman unduhan.
2. Klik dua kali berkas `Setup.exe`.
3. Jika muncul jendela **SmartScreen** biru (“Windows protected your PC”), klik **More info**, lalu **Run anyway**. Ini peringatan rutin untuk program baru, bukan sebuah kesalahan.
4. Tunggu hingga pemasangan selesai. Tidak diperlukan hak administrator — pemasang memeriksa sistem Anda dan menyiapkan segalanya.

**Apa yang terjadi berikutnya.** Ikon FarmPanel muncul di desktop Anda dan di menu Start.

![jendela pemasang Setup.exe](../images/setup-installer.png)

## Langkah 2. Buka aplikasi

Klik dua kali ikon **FarmPanel** di desktop Anda.

**Apa yang akan Anda lihat.** Pada peluncuran pertama, selama lisensi belum diaktifkan, **Activation Wizard** (wizard aktivasi) terbuka. Layar utama baru muncul setelah aktivasi berhasil.

## Langkah 3. Aktifkan lisensi Anda

Jendela aktivasi memandu Anda langkah demi langkah.

1. Ketik atau tempel kunci lisensi Anda ke kolom masukan. Untuk menempelnya dari papan klip, klik **Paste from clipboard**.
2. Aplikasi memeriksa format kunci saat Anda mengetik. Ketika formatnya benar, tombol aktivasi menjadi tersedia.
3. Klik **Activate**.

**Apa yang terjadi berikutnya.** Aplikasi menghubungi server lisensi dan memverifikasi kunci. Ini butuh beberapa detik — Anda akan melihat keadaan **Activating**.

**Tanda keberhasilan.** Jendela aktivasi menutup dan layar utama aplikasi (**Dashboard**) terbuka. Lisensi Anda aktif — Anda tidak perlu memasukkan kunci lagi pada peluncuran berikutnya.

> **Jika aktivasi gagal**, aplikasi menampilkan pesan yang jelas dan memberi tahu apa yang harus dilakukan. Kasus-kasus umum dibahas di [10. Kesalahan dan pemecahan masalah](#10-kesalahan-dan-pemecahan-masalah).

![jendela aktivasi lisensi](../images/license-activation.png)

## Langkah 4. Periksa pengaturan dasar

Sebelum meluncurkan akun untuk pertama kali, ada baiknya memeriksa pengaturan Anda.

1. Klik **Settings** di panel kiri, atau tekan `Ctrl+,`.
2. Buka bagian **Sandboxes** dan, jika perlu, pilih folder untuk sandbox.
3. Secara opsional buka **Appearance** dan pilih tema (**System / Dark / Light**) serta kepadatan antarmuka.

Pengaturan tersimpan otomatis: setelah setiap perubahan muncul notifikasi singkat **Saved**.

## Langkah 5. Siap untuk mulai

Kini Anda bisa menambahkan akun dan meluncurkan farm pertama Anda. Lihat [5. Alur kerja inti](#5-alur-kerja-inti) untuk caranya.

**Tanda bahwa semuanya bekerja.** Bilah bawah jendela (bilah status) menampilkan ringkasan: jumlah akun, proses aktif, dan versi aplikasi saat ini.

---

# 4. Ikhtisar antarmuka

Aplikasi berjalan dalam satu jendela utama. Ia terdiri dari elemen tetap yang selalu ada di tempatnya dan sebuah area layar yang berubah tergantung bagian yang Anda pilih.

```
┌────────────────────────────────────────────────────────────┐
│  Command Bar                                                │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Sidebar  │   Area kerja layar terpilih                     │
│          │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Status Bar                                                 │
└────────────────────────────────────────────────────────────┘
```

![struktur jendela keseluruhan dengan area berlabel](../images/window-layout.png)

## 4.1. Command Bar (bilah atas)

**Tujuan.** Pita tetap di bagian atas jendela. Ia memuat navigasi, pencarian global, dan notifikasi.

**Lokasi.** Baris paling atas jendela.

**Elemen utama (kiri ke kanan):**

- **Tombol hamburger (☰)** — menciutkan dan memperluas sidebar. Pintasan `Ctrl+B`.
- **Logo** — mengekliknya mengembalikan Anda ke layar utama (**Dashboard**).
- **Breadcrumbs** — menunjukkan posisi Anda, misalnya `Accounts › alex_42 › Events`. Klik segmen mana pun untuk melompat ke sana.
- **Pencarian / palet perintah** — di tengah. Tekan `Ctrl+K` untuk membuka palet perintah (lihat di bawah).
- **Lencana notifikasi** — ikon dengan penghitung (misalnya, `⚠ 3`). Mengekliknya membuka pusat notifikasi.

**Kapan menggunakannya.** Command Bar selalu dalam jangkauan: untuk berpindah cepat antarlayar, mencari akun berdasarkan nama pengguna, atau menjalankan perintah tanpa mouse.

### Command Palette

Tekan `Ctrl+K` kapan saja untuk membuka palet perintah — kotak pencarian untuk setiap tindakan dan objek di aplikasi.

1. Mulai mengetik nama perintah, layar, nama pengguna akun, atau alur kerja.
2. Daftar menyempit ke hasil yang cocok. Berpindah di antaranya dengan `↑` `↓`.
3. Tekan `Enter` untuk menjalankan item terpilih.

**Kenapa membantu.** Palet perintah adalah cara tercepat menemukan apa pun tanpa menghafal letak tombol.

![palet perintah terbuka](../images/command-palette.png)

## 4.2. Sidebar

**Tujuan.** Navigasi utama aplikasi.

**Lokasi.** Di kiri, setinggi penuh jendela.

**Bagian (atas ke bawah):**

| Ikon | Bagian | Apa yang ditampilkan |
|---|---|---|
| ▤ | **Dashboard** | Ikhtisar seluruh farm |
| 👥 | **Accounts** | Daftar semua akun (layar kerja utama) |
| ⚙ | **Workflows** | Skenario peluncuran otomatis dan progresnya |
| ⚔ | **Matchmaking** | Party dan pencarian pertandingan |
| 📈 | **Monitoring** | Beban komputer dan kesehatan proses |
| 📜 | **Logs** | Log peristiwa |
| ▣ | **Layouts** | Menata jendela CS2 di seluruh monitor |
| ▦ | **Sandboxes** | Sandbox (lingkungan terisolasi) |
| ⚙ | **Settings** | Pengaturan aplikasi |
| ? | **Help** | Bantuan |

Beberapa bagian menampilkan penghitung (misalnya, jumlah akun) atau titik langsung saat ada aktivitas.

**Tindakan utama:**

- Klik sebuah bagian untuk membukanya. Anda juga bisa memakai `Ctrl+1`…`Ctrl+8`.
- Tombol ciutkan (atau `Ctrl+B`) menyusutkan panel menjadi ikon untuk membebaskan ruang.

**Kiat.** Berpindah antarbagian mempertahankan keadaan Anda — filter, pilihan, dan posisi gulir. Ketika Anda kembali ke suatu layar, Anda menemukannya persis seperti saat ditinggalkan.

![sidebar dengan semua bagian](../images/sidebar.png)

## 4.3. Status Bar

**Tujuan.** Bilah tipis di bagian bawah jendela dengan ringkasan cepat keadaan seluruh farm.

**Lokasi.** Baris paling bawah jendela.

**Apa yang ditampilkan (contoh):**

```
[env: PROD] | ● 412 accounts (238 running) | ▶ 18 workflows | ◎ 7 matches | CPU 42% RAM 71% | ⚠ 3 errors | 14:32:08 | v1.0.1
```

- berapa banyak akun yang ada dan berapa yang sedang berjalan;
- berapa banyak alur kerja dan pertandingan aktif yang sedang berlangsung;
- beban prosesor dan memori;
- jumlah kesalahan (klik untuk membuka pusat notifikasi);
- waktu dan versi aplikasi.

**Kapan menggunakannya.** Sekilas lihat bilah status untuk tahu dalam sedetik apakah semuanya baik-baik saja.

## 4.4. Layar Dashboard

**Tujuan.** Satu layar ikhtisar. Dalam beberapa detik ia menjawab: berapa akun daring, berapa alur kerja yang berjalan atau gagal, apakah ada aktivitas matchmaking, apakah ada mogok, dan seberapa terbebani komputernya.

**Lokasi.** Bagian pertama di sidebar. Ia terbuka tepat setelah peluncuran.

**Area utama:**

- **KPI strip** — lima kartu di bagian atas: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Masing-masing menampilkan angka utama dan grafik mini. Mengeklik kartu membawa Anda ke layar yang sesuai.
- **Live Activity Feed** — aliran waktu nyata peristiwa operasional. Gunakan tombol jeda (atau tombol `Space`) untuk menjeda gulir.
- **Account State Heatmap** — kisi tempat setiap akun berupa sel berwarna. Warnanya mencerminkan statusnya. Arahkan kursor untuk melihat nama pengguna dan status; klik untuk melompat ke akun.
- **Active Workflows / Matchmaking Queue / Sandboxes** — tiga ubin yang meringkas alur kerja, antrean pertandingan, dan sandbox.
- **Failures & Crashes** — tabel kesalahan dan mogok terkini dari satu jam terakhir.

**Penggunaan umum.** Di pagi hari, buka **Dashboard** untuk menilai farm sekilas, lalu pergi ke mana pun perhatian diperlukan.

**Kiat.**
- Metrik menyegar otomatis. Untuk memaksa penyegaran penuh, tekan `F5`.
- Jika ada yang disorot merah di kartu **Errors** atau tabel kegagalan, mulai penyelidikan Anda dari sana.

![Dashboard dengan KPI strip dan activity feed](../images/dashboard-screen.png)

## 4.5. Layar Accounts

**Tujuan.** Layar kerja utama. Di sini Anda menyimpan akun, menemukan yang dibutuhkan, serta memulai dan menghentikannya.

**Lokasi.** Bagian kedua di sidebar (`Ctrl+2`).

**Area utama:**

- **Toolbar** — tombol **Add Account**, **Import**, **Export**, dan **Refresh**, kolom pencarian, filter, dan kontrol tampilan.
- **Tabel akun** — daftar semua akun dengan kolom: status, nama pengguna, nickname, rank, alur kerja, sandbox, tag, waktu login terakhir, dan lainnya.
- **Details Pane** — di kanan. Menampilkan detail akun terpilih. Tampilkan atau sembunyikan dengan `Ctrl+\`.

**Apa yang bisa Anda lakukan:**

- Tambahkan akun satu per satu atau impor daftar.
- Cari dan filter akun.
- Mulai, hentikan, dan mulai ulang satu akun atau banyak sekaligus.
- Ikat akun ke sandbox dan tetapkan alur kerja.
- Lihat kartu akun terperinci: data, riwayat, peristiwa, dan log.

**Penggunaan umum.** Pilih akun yang Anda butuhkan di tabel, lalu lakukan tindakan pada mereka — melalui toolbar, menu konteks (klik kanan), atau pintasan keyboard.

Instruksi langkah demi langkah terperinci ada di [5. Alur kerja inti](#5-alur-kerja-inti).

![layar Accounts dengan tabel dan details pane](../images/accounts-screen.png)

### Panel detail akun (Details Pane)

Di kanan tabel, kartu untuk akun terpilih muncul dengan tab-tab ini:

| Tab | Apa yang ditampilkan |
|---|---|
| **Overview** | Data inti, ikatan sandbox, alur kerja yang ditetapkan, tag, tanggal penting, dan tombol tindakan |
| **Inventory** | Inventaris akun: jumlah dan nilai item |
| **Workflow** | Keadaan skenario yang ditetapkan saat ini dan langkahnya kini |
| **Events** | Peristiwa terkini untuk akun ini |
| **Logs** | Log peristiwa yang difilter ke akun ini |
| **History** | Riwayat perubahan: pembuatan, penyuntingan, penggantian nama, pengikatan ulang sandbox |

Di bagian bawah tab **Overview** ada blok tombol: **Start**, **Stop**, **Restart**, **Pause**, ditambah **Edit account** dan **Delete**. Tindakan paling relevan disorot: **Start** saat akun berhenti, dan **Stop** saat berjalan.

## 4.6. Layar Workflows

**Tujuan.** Kelola skenario peluncuran otomatis dan awasi jalannya.

**Lokasi.** Bagian ketiga di sidebar (`Ctrl+3`).

**Apa itu alur kerja.** Alur kerja adalah urutan langkah yang telah ditentukan yang dijalankan aplikasi untuk sebuah akun: masuk ke Steam, meluncurkan CS2, dan seterusnya. Skenario yang sama selalu berjalan dengan cara yang sama, sehingga hasilnya dapat diprediksi.

- **Definition** — templat skenario: sekumpulan langkah.
- **Instance** — satu kali jalannya sebuah definition untuk akun tertentu.

**Area utama:**

- **Kiri** — daftar definition (templat) dan versinya.
- **Tengah** — tabel instance yang berjalan: skenario mana, untuk akun mana, pada langkah mana, berapa kali coba ulang, kapan dimulai.
- **Kanan** — detail instance terpilih (tab **Overview**, **State Machine**, **Steps**, **Logs**, **Retries**).
- **Bawah** — linimasa peristiwa yang dapat diciutkan untuk instance yang terlihat (`Ctrl+T`).

**Kapan menggunakannya.** Datanglah ke sini untuk melihat pada langkah mana peluncuran tiap akun berada, menjeda atau memulai ulang skenario, atau mencari tahu mengapa sesuatu tidak selesai.

![layar Workflows dengan tiga panel](../images/workflows-screen.png)

## 4.7. Layar Matchmaking

**Tujuan.** Bangun party dari akun-akun dan antrekan mereka untuk matchmaking bersama.

**Lokasi.** Bagian keempat di sidebar (`Ctrl+4`).

**Konsep kunci:**

| Istilah | Arti |
|---|---|
| **Party** | Sekelompok akun yang mencari pertandingan bersama |
| **Quorum** | Semua anggota party sudah masuk, dalam antrean, dan tidak dalam pertandingan |
| **Queue** | Menunggu pertandingan: posisi, region, mode |
| **Match Found** | Steam menemukan pertandingan. Aplikasi mengonfirmasi kesiapan untuk semua anggota secara otomatis — Anda tak perlu melakukan apa pun |
| **Desync** | Anggota berada dalam keadaan tidak konsisten (misalnya, seseorang keluar dari antrean) |

**Area utama:**

- **Kiri** — daftar party dengan keadaannya (quorum, desync, match found, idle).
- **Kanan** — detail party terpilih: anggota, keadaannya, posisi antrean, latensi jaringan, sandbox.
- **Bawah** — linimasa peristiwa matchmaking terkini.

**Kapan menggunakannya.** Di sini Anda membangun party berisi 2–5 akun dan memasukkannya ke antrean. Ketika pertandingan ditemukan, aplikasi mengonfirmasi kesiapan untuk semua anggota secara otomatis.

![layar Matchmaking dengan party dan detail](../images/matchmaking-screen.png)

## 4.8. Layar Monitoring

**Tujuan.** Awasi beban komputer, kesehatan proses, dan mogok secara waktu nyata.

**Lokasi.** Bagian kelima di sidebar (`Ctrl+5`).

**Area utama:**

- **Pengukur sumber daya** — kartu **CPU**, **RAM**, **Disk**, **Net**, dan, bila tersedia, **GPU** dengan nilai saat ini dan grafik mini.
- **Process Explorer** — tabel semua proses Steam dan CS2 yang berjalan: milik akun mana masing-masing, berapa banyak yang dikonsumsinya, sudah berapa lama berjalan.
- **Crashes & Warnings** — aliran kegagalan terkini.
- **Logs panel** — log di bagian bawah layar, yang dapat diciutkan.

**Kontrol waktu.** Di bagian atas Anda bisa beralih antara **Live** (waktu nyata), **Last 1h / 24h**, dan **Custom** (periode khusus). Tombol **Freeze** (`Ctrl+Space`) membekukan gambar sehingga Anda bisa mempelajarinya dengan tenang.

**Kapan menggunakannya.** Jika komputer mulai melambat atau mogok makin sering, buka **Monitoring** untuk melihat proses mana yang memakan sumber daya dan apa persisnya yang mogok.

> **Kiat.** Anda bisa membuka layar **Monitoring** di jendela terpisah dengan tombol lepas dan meletakkannya di monitor kedua.

![layar Monitoring dengan pengukur dan daftar proses](../images/monitoring-screen.png)

## 4.9. Layar Logs

**Tujuan.** Log terperinci dari semua peristiwa aplikasi — seperti umpan langsung tentang apa yang sedang terjadi.

**Lokasi.** Bagian keenam di sidebar (`Ctrl+6`).

**Fitur utama:**

- **Filter level** — sakelar **Error**, **Warn**, **Info**, **Debug**. Secara bawaan pesan kesalahan, peringatan, dan info ditampilkan.
- **Filter sumber** — Anda bisa mempersempit log ke satu akun, alur kerja, atau sandbox.
- **Pencarian** — `Ctrl+F`, dengan lompat antarhasil (`F3` / `Shift+F3`).
- **Follow** — log menggulir otomatis ke baris baru. Tombol `Space` mengaktifkan dan menonaktifkan pengikutan. Jika Anda menggulir ke atas, pengikutan berhenti sejenak dan tombol lompat-ke-bawah muncul.
- **Export** — simpan baris yang terlihat ke berkas.

**Kapan menggunakannya.** Ketika Anda butuh detail: apa persisnya yang terjadi pada akun tertentu dan dalam urutan apa.

![layar Logs dengan log peristiwa](../images/logs-screen.png)

## 4.10. Layar Layouts

**Tujuan.** Tata jendela CS2 di satu monitor atau lebih menggunakan tata letak siap pakai.

**Lokasi.** Bagian ketujuh di sidebar (`Ctrl+7`).

**Konsep kunci:**

- **Preset** — susunan jendela yang tersimpan.
- **Slot** — area persegi panjang pada monitor tempat satu jendela akan diletakkan.
- **Snap** — perintah yang menata jendela yang berjalan ke dalam slot.

**Area utama:**

- **Kiri** — daftar preset tersimpan.
- **Kanan** — kanvas yang menampilkan monitor Anda, tempat Anda menempatkan slot.
- **Bawah** — tabel ikatan: slot mana berkorespondensi dengan akun atau peran mana.

**Cara menggunakannya.**
1. Buat preset dengan tombol **New Preset**.
2. Tempatkan slot pada kanvas.
3. Tetapkan akun mana masuk ke slot mana.
4. Klik **Apply** atau **Snap windows** — aplikasi menata jendela CS2 yang berjalan ke tempat yang telah ditentukan.

> **Jaring pengaman.** Sebelum menata, aplikasi mengingat posisi jendela saat ini. Tombol **Revert layout** memulihkan posisi sebelumnya dalam waktu satu menit.

![layar Layouts dengan kanvas monitor](../images/layouts-screen.png)

## 4.11. Layar Sandboxes

**Tujuan.** Kelola sandbox — lingkungan terisolasi tempat klien Steam berjalan.

**Lokasi.** Bagian kedelapan di sidebar (`Ctrl+8`).

**Apa itu sandbox.** Sandbox adalah lingkungan terpisah dan terlindungi untuk satu klien Steam. Akun di sandbox berbeda tidak pernah tumpang tindih: mereka tidak berbagi sesi, berkas, atau jejak. Satu akun terikat ke satu sandbox.

**Kapan menggunakannya.** Di sini Anda membuat sandbox dan mengawasi keadaannya. Dalam kebanyakan kasus sandbox ditetapkan otomatis saat Anda menambahkan akun, sehingga Anda jarang perlu ke sini dengan sengaja.

## 4.12. Layar Settings

**Tujuan.** Sesuaikan aplikasi dengan preferensi Anda.

**Lokasi.** Bagian **Settings** di bagian bawah sidebar (`Ctrl+,`).

**Tata letak.** Di kiri ada daftar bagian pengaturan; di kanan ada pengaturannya sendiri. Perubahan tersimpan seketika: notifikasi singkat **Saved** muncul setelah masing-masing.

**Bagian pengaturan:**

| Bagian | Apa yang diatur |
|---|---|
| **General** | Luncurkan dengan Windows, minimalkan ke tray, saluran pembaruan |
| **Appearance** | Tema (**System / Dark / Light**), kepadatan, skala fon, gerak dikurangi |
| **Accounts** | Perilaku saat membuat akun, penyimpanan yang dihapus |
| **Workflows** | Kebijakan coba ulang, batasan jalan bersamaan |
| **Sandboxes** | Folder sandbox, pemulihan otomatis |
| **Monitoring** | Laju penyegaran data, ambang peringatan |
| **Notifications** | Notifikasi dan suara per tingkat keparahan |
| **Layouts** | Tata letak bawaan, perilaku multi-monitor |
| **Hotkeys** | Pintasan keyboard — bisa ditetapkan ulang |
| **Advanced** | Level pencatatan, diagnostik, pemilihan lingkungan, atur ulang ke bawaan |
| **About** | Versi aplikasi, tombol membuka folder data dan log |

> **Catatan.** Beberapa pengaturan (misalnya, folder sandbox atau lingkungan) baru berlaku setelah pemulaian ulang. Pengaturan semacam itu menampilkan lencana “Requires restart” di sebelahnya.

![layar Settings](../images/settings-screen.png)

---

# 5. Alur kerja inti

Ini bagian terpenting. Ia berisi instruksi langkah demi langkah lengkap untuk tugas-tugas utama. Setiap langkah menjelaskan apa yang akan Anda lihat dan cara memastikan keberhasilan.

## 5.1. Menambahkan satu akun

**Tujuan.** Tambahkan satu akun Steam baru ke aplikasi.

**Yang Anda butuhkan.** Nama pengguna dan kata sandi akun. Kode Steam Guard jika berlaku.

### Langkah 1 — Buka formulir penambahan

Buka layar **Accounts** dan klik **Add Account** di toolbar. Anda juga bisa menekan `Ctrl+N`.

**Hasil yang diharapkan.** Formulir dengan kolom untuk akun baru terbuka.

### Langkah 2 — Isi detailnya

Isi kolom-kolomnya:

- **Login** — wajib, harus unik.
- **Password** — wajib.
- **Steam Guard secret** — kode Steam Guard, jika Anda memilikinya (opsional).
- **Nickname** — opsional; bisa diambil otomatis pada login pertama.
- **Tags** — tag opsional untuk pengelompokan.
- **Sandbox binding** — pilih **Auto-assign**, sandbox tertentu, atau **None**.
- **Workflow** — skenario peluncuran, jika Anda ingin menetapkannya langsung.

**Hasil yang diharapkan.** Jika nama pengguna sudah dipakai, kolom disorot merah dengan penjelasan. Kata sandi lemah disorot kuning — ini peringatan dan tidak mencegah penyimpanan.

### Langkah 3 — Simpan akun

Klik tombol simpan di formulir.

**Hasil yang diharapkan.** Formulir menutup dan akun baru muncul di tabel dengan status **Draft** atau, jika terikat ke sandbox, siap diluncurkan.

**Tanda keberhasilan.** Akun terlihat di tabel pada layar **Accounts**.

### Kiat

- Jika Anda mengaktifkan **Validate immediately** di formulir, aplikasi memeriksa nama pengguna di latar belakang dan menampilkan hasilnya sebagai notifikasi.
- Agar sebuah akun dapat diluncurkan, ia harus terikat ke sandbox. Pilihan paling sederhana adalah **Auto-assign**.

### Kesalahan umum dan cara memperbaikinya

- **“Login already in use.”** Nama pengguna ini sudah ada di aplikasi. Periksa daftar akun Anda — mungkin Anda sudah menambahkannya.
- **Lupa sandbox.** Akun tanpa sandbox tidak bisa diluncurkan. Ikat satu nanti melalui menu konteks → **Bind sandbox**.

![formulir penambahan akun](../images/accounts-add-form.png)

## 5.2. Mengimpor daftar akun dari berkas

**Tujuan.** Tambahkan cepat banyak akun sekaligus dari sebuah berkas.

**Yang Anda butuhkan.** Berkas berisi daftar akun (TXT, CSV, atau TSV). Format baris TXT paling sederhana adalah `login:password` (Anda juga bisa memakai `login:password:steamguard:nickname`).

### Langkah 1 — Mulai wizard impor

Di layar **Accounts**, klik panah di sebelah tombol **Import** dan pilih sumber — misalnya, **From file…**. Anda juga bisa menekan `Ctrl+I`.

**Hasil yang diharapkan.** Wizard impor langkah demi langkah terbuka.

### Langkah 2 — Pilih sumber dan cara sandbox ditetapkan

Tunjuk berkasnya dengan tombol **Browse…**. Di bagian bawah, pilih cara menetapkan sandbox:

- **Auto-assign (round-robin)** — distribusikan secara siklus (disarankan);
- **Bind to specific sandbox** — ikat semuanya ke satu sandbox;
- **Leave unbound** — biarkan tanpa sandbox.

Klik Next.

### Langkah 3 — Periksa cara data dikenali

Wizard menampilkan baris-baris pertama berkas sebagai tabel. Pastikan data terbelah ke kolom dengan benar. Jika pembatas terdeteksi salah, atur secara manual.

**Hasil yang diharapkan.** Pada pratinjau, nama pengguna dan kata sandi berada di kolomnya masing-masing.

### Langkah 4 — Petakan kolom

Seret judul kolom ke sel yang diperlukan: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Langkah 5 — Periksa bahwa baris valid

Wizard menandai setiap baris: ✓ valid, ⚠ peringatan, ✕ kesalahan. Baris dengan kesalahan bisa diperbaiki di sini atau dilewati.

**Hasil yang diharapkan.** Anda melihat berapa akun yang akan ditambahkan, berapa yang duplikat, dan berapa yang bermasalah.

### Langkah 6 — Konfirmasi impor

Klik **Import N accounts**.

**Hasil yang diharapkan.** Bilah kemajuan dengan status per baris muncul. Ketika selesai, akun muncul di tabel.

**Tanda keberhasilan.** Jumlah akun di tabel bertambah sebanyak yang diimpor.

### Cara membatalkan dan memulihkan

Jika Anda membatalkan impor saat sedang berjalan, aplikasi menawarkan untuk mengembalikan batch yang sudah ditambahkan. Konfirmasi pengembalian untuk kembali ke keadaan semula.

![wizard impor, langkah validasi baris](../images/import-wizard-validation.png)

## 5.3. Meluncurkan beberapa akun

**Tujuan.** Mulai beberapa akun pada saat yang sama.

**Yang Anda butuhkan.** Akun yang sudah ditambahkan dan diikat ke sandbox.

### Langkah 1 — Pilih akun

Di layar **Accounts**, centang akun yang Anda inginkan di kolom pertama. Untuk memilih semua yang terlihat, tekan `Ctrl+A`.

**Hasil yang diharapkan.** Toolbar beralih ke mode massal dan menampilkan berapa baris yang terpilih, misalnya `12 selected`.

### Langkah 2 — Mulai akun terpilih

Klik **Start** di toolbar massal. Anda juga bisa menekan `Ctrl+R`.

**Hasil yang diharapkan.** Status akun terpilih berubah menjadi **Starting**. Aplikasi menyiapkan tiap akun dan mulai meluncurkan. Peluncuran terjadi dalam batch agar komputer tidak kelebihan beban.

### Langkah 3 — Tunggu peluncuran

Awasi kolom status. Tunggu hingga akun berpindah ke keadaan **Running**.

**Hasil yang diharapkan.** Akun yang diluncurkan menampilkan **Running**, dengan penghitung waktu aktif di sebelahnya.

**Tanda keberhasilan.** Semua akun terpilih menampilkan **Running**. Jumlah aktif di bilah status meningkat.

### Kiat

- Anda tak harus meluncurkan setiap akun sekaligus. Mulai dengan batch kecil, pastikan semuanya stabil, lalu tambahkan lagi.
- Untuk meluncurkan satu akun: pilih satu baris dan klik **Start**, atau gunakan tombol **Start** di details pane di kanan.

### Kesalahan umum dan pemulihan

- **Sebuah akun terlalu lama di Starting.** Login mungkin lambat. Tunggu; jika status berubah menjadi **Error**, gunakan tombol **Retry**.
- **Beberapa akun tidak jalan.** Setelah peluncuran massal, ringkasan menunjukkan berapa yang berhasil dan gagal. Klik **Filter to failed** untuk menangani hanya yang itu.

![peluncuran massal akun, status Starting/Running](../images/accounts-bulk-start.png)

## 5.4. Menghentikan semua akun yang berjalan

**Tujuan.** Matikan bersih semua akun aktif.

### Langkah 1 — Pilih akun

Pilih akun yang berjalan. Untuk memilih semua yang terlihat, tekan `Ctrl+A`.

### Langkah 2 — Hentikan

Klik **Stop** di toolbar massal, atau tekan `Ctrl+.` (Ctrl dan titik).

**Hasil yang diharapkan.** Aplikasi mematikan bersih setiap akun. Status berubah menjadi **Stopped**. Jika sebuah akun tidak merespons, setelah beberapa saat aplikasi menutupnya secara paksa.

**Tanda keberhasilan.** Semua akun menampilkan **Stopped**. Jumlah aktif di bilah status berkurang.

### Kiat

- **Stop** adalah penutupan yang mulus. Aplikasi terlebih dahulu mencoba menutup klien dengan benar.
- Jika sebuah akun sedang dalam pertandingan, selesaikan dulu tindakan di dalam gim, lalu hentikan.

## 5.5. Membuat party dan mengantrekannya

**Tujuan.** Bangun party berisi beberapa akun dan antrekan mereka untuk matchmaking bersama.

**Yang Anda butuhkan.** Beberapa akun berjalan (**Running**) yang sudah masuk.

### Langkah 1 — Buat party

Buka layar **Matchmaking** dan klik **Create Party**. Anda juga bisa menekan `Ctrl+N`.

**Hasil yang diharapkan.** Jendela terbuka tempat Anda bisa menambahkan akun ke party dan memberinya nama.

### Langkah 2 — Tambahkan anggota dan simpan

Tambahkan 2 hingga 5 akun ke party, setel nama, dan simpan.

**Hasil yang diharapkan.** Party baru muncul di daftar sebelah kiri.

### Langkah 3 — Periksa quorum

Pilih party dan lihat anggotanya di kanan. Pastikan party berada dalam keadaan **Quorum** — yakni semua anggota sudah masuk dan siap.

**Hasil yang diharapkan.** Party menampilkan lencana **✓ Quorum**. Jika seorang anggota bermasalah (misalnya, login lambat), ia ditampilkan sebagai baris terpisah.

### Langkah 4 — Antrekan party

Klik **Queue** untuk party terpilih (atau `Ctrl+Q`). Untuk mengantrekan semua party sekaligus, gunakan **Queue All** di toolbar.

**Hasil yang diharapkan.** Sebelum mengantre, aplikasi menjalankan pemeriksaannya. Lalu semua anggota masuk ke antrean, dengan posisi dan latensi jaringan ditampilkan.

**Tanda keberhasilan.** Anggota berada dalam keadaan antre, dengan penghitung waktu tunggu berjalan.

### Kiat

- Pilih region dan mode di toolbar (misalnya, `EU` dan `Premier`) sebelum mengantre.
- Jika party masuk ke keadaan **Desync**, gunakan tindakan **Re-sync** untuk menjeda antrean dan menunggu keadaan yang konsisten.

![party dalam antrean dengan posisi anggota](../images/matchmaking-party-queue.png)

## 5.6. Apa yang terjadi saat pertandingan ditemukan

**Tujuan.** Pahami apa yang dilakukan aplikasi pada saat pertandingan ditemukan.

**Yang Anda butuhkan.** Party yang berada dalam antrean.

### Penerimaan pertandingan bersifat otomatis

Ketika Steam menemukan pertandingan, banner **MATCH FOUND** yang menonjol muncul untuk party. **Anda tak perlu mengeklik apa pun** — aplikasi mengonfirmasi kesiapan untuk semua anggota party dalam jendela waktu yang diberikan. Tidak ada tindakan yang diperlukan dari Anda.

**Hasil yang diharapkan.** Anggota party menerima pertandingan secara otomatis; keadaan mereka berubah menjadi **✓ Accepted**.

**Tanda keberhasilan.** Semua anggota menampilkan **Accepted**, dan pertandingan dimulai.

> **Kiat.** Ingin tahu pertandingan ditemukan tanpa menatap layar? Aktifkan peringatan suara untuk **Match found** di **Settings → Notifications**. Penerimaan tetap terjadi otomatis — suara hanya ada untuk memberi tahu Anda.

### Apa yang dilakukan jika party desync

Kadang pertandingan tidak bisa dikonfirmasi untuk semua orang — misalnya, jika seorang anggota keluar dari antrean. Party lalu masuk ke keadaan **Desync**. Gunakan tindakan **Re-sync**, dan jika perlu keluarkan anggota bermasalah dengan **Drop member**, lalu antrekan sisanya lagi.

![banner Match Found](../images/matchmaking-match-found.png)

## 5.7. Memulihkan setelah mogok atau pemulaian ulang aplikasi

**Tujuan.** Kembalikan farm ke keadaan berfungsi setelah klien mogok, atau setelah aplikasi ditutup dan dibuka lagi.

**Yang Anda butuhkan.** Tidak ada yang tambahan — pemulihan sebagian besar terjadi otomatis.

### Apa yang terjadi otomatis

- **Setelah klien mogok.** Jika Steam atau CS2 menutup tak terduga, aplikasi menyadarinya, menandai akun dengan status **Crashed**, dan menampilkan notifikasi dengan tombol **Restart**. Pemulihan sering terjadi sendiri dalam beberapa detik.
- **Setelah pemulaian ulang aplikasi.** Saat menyala, aplikasi mencari proses Steam dan CS2 yang tersisa dari sesi sebelumnya dan mengambilnya kembali ke dalam pengelolaan. Selama ini, indikator **Recovering** muncul di bilah status. Akun yang tersambung ulang ditandai “Reattached” sebentar.

### Apa yang dilakukan secara manual

1. Buka **Dashboard** dan lihat tabel **Failures & Crashes**.
2. Untuk akun yang mogok, klik **Restart** di notifikasi, di baris akun, atau di details pane.
3. Jika aplikasi melaporkan **Orphan process** di pusat notifikasi, pilih **Adopt** atau **Kill**.

**Tanda keberhasilan.** Akun berada kembali dalam status **Running**, penanda mogok merah hilang, dan tak ada indikator **Recovering** aktif di bilah status.

### Kiat

- Jangan luncurkan ulang semuanya secara manual tepat setelah mogok — beri dulu pemulihan otomatis beberapa detik.
- Jika mogok berulang, buka **Monitoring** untuk melihat beban: Anda mungkin menjalankan lebih banyak akun daripada yang bisa ditangani komputer ini.

![indikator Recovering di bilah status](../images/status-recovering.png)

---

# 6. Tugas umum («Saya ingin…»)

Jawaban singkat untuk tujuan umum. Untuk instruksi lengkap, ikuti tautan ke bagian 5.

## «Saya ingin menambahkan akun baru»

- **Kapan diperlukan.** Anda punya akun Steam baru.
- **Apa yang dilakukan.** Untuk satu akun, gunakan tombol **Add Account** di layar **Accounts**. Untuk banyak sekaligus, gunakan tombol **Import** dan wizard impor.
- **Apa yang terjadi.** Akun muncul di tabel dan siap diluncurkan (setelah punya sandbox).
- Selengkapnya: [5.1](#51-menambahkan-satu-akun), [5.2](#52-mengimpor-daftar-akun-dari-berkas).

## «Saya ingin meluncurkan Steam»

- **Kapan diperlukan.** Anda butuh sebuah akun untuk masuk ke Steam.
- **Apa yang dilakukan.** Pilih akun di layar **Accounts** dan klik **Start**.
- **Apa yang terjadi.** Aplikasi meluncurkan Steam di sandbox akun dan masuk. Status berpindah **Starting → Running**.

## «Saya ingin meluncurkan CS2»

- **Kapan diperlukan.** Steam sudah berjalan dan Anda perlu memulai gim.
- **Apa yang dilakukan.** Meluncurkan akun dengan **Start** membawanya melalui seluruh skenario, termasuk memulai CS2 (jika alur kerja yang ditetapkan menyertakannya).
- **Apa yang terjadi.** Setelah masuk ke Steam, aplikasi meluncurkan CS2. Anda bisa mengawasi langkahnya di layar **Workflows**.

## «Saya ingin membuat lobi»

- **Kapan diperlukan.** Anda perlu mengumpulkan akun ke dalam lobi gim.
- **Apa yang dilakukan.** Bangun party di layar **Matchmaking** dengan **Create Party** dan tambahkan anggota.
- **Apa yang terjadi.** Aplikasi menggabungkan akun terpilih ke dalam party dan membantu membawa mereka ke keadaan konsisten (quorum).
- Selengkapnya: [5.5](#55-membuat-party-dan-mengantrekannya).

## «Saya ingin memulai matchmaking»

- **Kapan diperlukan.** Party sudah dibangun dan siap.
- **Apa yang dilakukan.** Pilih party dan klik **Queue** (atau **Queue All** untuk semuanya).
- **Apa yang terjadi.** Anggota masuk ke antrean; Anda melihat posisi dan waktu tunggu mereka.

## «Saya ingin menghentikan semua sesi yang berjalan»

- **Kapan diperlukan.** Saatnya beres-beres.
- **Apa yang dilakukan.** Pilih akun (`Ctrl+A`) dan klik **Stop**.
- **Apa yang terjadi.** Aplikasi menutup bersih klien, dan status menjadi **Stopped**.
- Selengkapnya: [5.4](#54-menghentikan-semua-akun-yang-berjalan).

## «Saya ingin memulihkan setelah mogok»

- **Kapan diperlukan.** Klien mogok atau aplikasi dimulai ulang.
- **Apa yang dilakukan.** Beri pemulihan otomatis beberapa detik; jika perlu, klik **Restart** untuk akun yang mogok.
- **Apa yang terjadi.** Aplikasi mengembalikan akun ke keadaan bekerja.
- Selengkapnya: [5.7](#57-memulihkan-setelah-mogok-atau-pemulaian-ulang-aplikasi).

## «Saya ingin menata jendela di layar»

- **Kapan diperlukan.** Anda ingin menata jendela CS2 dengan rapi di monitor Anda.
- **Apa yang dilakukan.** Di layar **Layouts**, buat preset dan klik **Apply** / **Snap windows**.
- **Apa yang terjadi.** Jendela yang berjalan berpindah ke tempat yang telah ditentukan.

---

# 7. Referensi fitur

Bagian ini membahas fitur individual dengan tujuan, lokasi, dan kekhususannya.

## 7.1. Pencarian akun dan filter

**Tujuan.** Temukan cepat akun yang Anda butuhkan dalam daftar besar.

**Lokasi.** Toolbar layar **Accounts**: kolom pencarian dan tombol **Filters**.

**Cara menggunakannya.**
- Ketik ke kolom pencarian (`Ctrl+F`). Anda bisa mencari berdasarkan bagian: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Klik **Filters** (`Ctrl+K` di layar ini membuka jendela filter), setel kondisi berdasarkan status, rank, sandbox, alur kerja, atau tag, dan simpan set sebagai preset.

**Perilaku yang diharapkan.** Tabel langsung hanya menampilkan akun yang cocok. Filter aktif muncul sebagai deretan chip di bawah toolbar.

**Kiat.** Simpan set kondisi yang sering dipakai sebagai preset — tersedia dari menu turun di toolbar.

## 7.2. Pengelompokan dan penataan kolom

**Tujuan.** Atur tabel agar sesuai dengan tugas Anda.

**Lokasi.** Toolbar layar **Accounts**: tombol **Density**, **Columns**, dan **Group**.

**Cara menggunakannya.**
- **Group** memungkinkan Anda mengelompokkan akun berdasarkan status, alur kerja, sandbox, tag, atau rank. Grup menampilkan penghitung, misalnya `Running (24)`.
- **Columns** — set kolom yang terlihat. Set bawaan tersedia: **Operational**, **Identity**, **Audit**, **Compact**. Anda bisa menyimpan milik Anda sendiri.
- **Density** — tinggi baris (lebih ringkas atau lebih lapang).

## 7.3. Menu konteks akun

**Tujuan.** Akses cepat ke setiap tindakan untuk sebuah akun.

**Lokasi.** Klik kanan sebuah baris akun.

**Apa yang tersedia.** Sunting, salin nama pengguna atau Steam ID, mulai/hentikan/mulai ulang, ikat dan lepas ikat sandbox, tetapkan alur kerja, autentikasi ulang (**Re-auth**), periksa login (**Probe login now**), kerjakan tag, ekspor, klon, dan hapus.

## 7.4. Operasi massal

**Tujuan.** Lakukan satu tindakan pada banyak akun sekaligus.

**Lokasi.** Toolbar layar **Accounts** dalam mode pilihan (saat setidaknya satu baris dicentang).

**Cara menggunakannya.** Centang akun, lalu klik tombol yang Anda butuhkan: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export**, atau **Delete**.

**Perilaku yang diharapkan.** Muncul jendela dengan tampilan kemajuan per akun. Anda bisa membatalkan operasi selama berjalan.

**Batasan.** Saat menghapus lima akun atau lebih, aplikasi meminta Anda mengonfirmasi dengan mengetik kata `DELETE`.

## 7.5. Mengekspor akun

**Tujuan.** Simpan data akun ke berkas.

**Lokasi.** Tombol **Export** di toolbar atau di menu konteks.

**Cara menggunakannya.** Pilih format: **TXT** (login:password), **CSV** (semua kolom), atau **JSON** (rekaman lengkap).

> **Peringatan.** Mengekspor kata sandi memerlukan persetujuan terpisah — aplikasi meminta Anda mencentang kotak. Tangani berkas semacam itu dengan hati-hati.

## 7.6. Mengklon akun

**Tujuan.** Buat cepat salinan akun sebagai titik awal.

**Lokasi.** Menu konteks baris → **Clone…**.

**Perilaku yang diharapkan.** Formulir terbuka dengan kolom yang sudah terisi (nama pengguna menjadi `original_copy`), kecuali kode Steam Guard dan ikatan sandbox — itu Anda setel lagi.

## 7.7. Workflow: mulai, jeda, hentikan

**Tujuan.** Kelola skenario otomatis.

**Lokasi.** Layar **Workflows**.

**Cara menggunakannya.**

| Tindakan | Apa yang dilakukan | Minta konfirmasi? |
|---|---|---|
| **Start** | Menjalankan skenario untuk akun terpilih | Saat meluncurkan lebih dari 10 akun |
| **Pause** | Menjeda dengan lembut setelah langkah saat ini | Tidak |
| **Resume** | Melanjutkan dari titik saat ini | Tidak |
| **Stop** | Mengakhiri skenario dengan pembersihan | Ya |
| **Restart** | Menghentikan dan memulai dari awal | Ya (untuk operasi massal) |
| **Skip step** | Menandai langkah saat ini selesai dan lanjut | Ya |
| **Retry now** | Mencoba ulang langkah saat ini seketika | Tidak |

**Kiat.** Tab **State Machine** di details pane menunjukkan dengan jelas pada langkah mana skenario berada.

## 7.8. Mengikat ke sandbox

**Tujuan.** Cadangkan lingkungan terisolasi untuk sebuah akun, yang tanpanya ia tak bisa diluncurkan.

**Lokasi.** Menu konteks → **Bind sandbox…**, atau operasi massal **Bind sandbox**.

**Cara menggunakannya.** Pilih metode: round-robin, isi yang kosong dulu, atau sandbox tertentu.

**Batasan.** Satu akun, satu sandbox. Jika sandbox yang dipilih sudah dipakai, aplikasi menawarkan untuk membebaskannya dari akun sebelumnya.

## 7.9. Tata letak jendela

**Tujuan.** Tata jendela CS2 menggunakan tata letak siap pakai.

**Lokasi.** Layar **Layouts**.

**Cara menggunakannya.** Buat preset, tempatkan slot pada kanvas monitor, setel ikatan, dan klik **Apply**.

**Kiat.** Tombol **Revert layout** memulihkan posisi jendela sebelumnya dalam waktu satu menit, kalau-kalau sebuah tata letak tidak berhasil.

## 7.10. Pusat notifikasi

**Tujuan.** Satu tempat untuk semua notifikasi aplikasi.

**Lokasi.** Lencana notifikasi di bilah atas, atau `Ctrl+Shift+N`.

**Cara menggunakannya.** Panel terbuka di kanan. Beralih antara tab **All**, **Errors**, **Warnings**, dan **Info**. Untuk setiap entri Anda bisa pergi ke sumber, coba ulang, atau tutup. Tombol **Clear all** mengosongkan daftar.

**Batasan.** 200 entri terakhir disimpan; yang lebih tua dihapus.

---

# 8. Status dan indikator

Setiap status punya warna, glif, dan label. Berikut arti masing-masing dan apakah Anda perlu bertindak.

| Status | Glif | Artinya | Perlu tindakan |
|---|---|---|---|
| **OK / Success** | ✓ (hijau) | Akun daring, login berhasil | Tidak |
| **Running** | ▶ (biru) | Akun atau alur kerja sedang berjalan | Tidak |
| **Starting** | ◐ (ungu) | Peluncuran berlangsung, keadaan transisi | Tunggu hingga selesai |
| **Queued** | ⏱ (abu-abu) | Menunggu di antrean | Tidak |
| **Stopped** | ■ (abu-abu) | Berhenti, menganggur | Opsional — Anda bisa memulainya |
| **Paused** | ⏸ (kuning) | Skenario dijeda | Klik **Resume** untuk melanjutkan |
| **Warning** | △ (kuning) | Anomali non-kritis | Periksa detailnya; sering kali Anda bisa lanjut |
| **Error** | ✕ (merah) | Kegagalan yang dapat dipulihkan | Klik **Retry** atau selidiki penyebabnya |
| **Crashed** | ☠ (merah gelap, berdenyut) | Proses keluar tak terduga | Klik **Restart** |
| **Match Found** | ◎ (hijau, berdenyut) | Pertandingan CS2 ditemukan | Tak ada — aplikasi mengonfirmasi kesiapan otomatis |
| **Desync** | ⛓ (oranye) | Anggota party tak sinkron | Jalankan **Re-sync** |
| **Info** | ⓘ (biru) | Pesan netral | Tidak |

**Indikator tambahan:**

- **Recovering** — indikator biru di bilah status selama aplikasi menyala: proses dari sesi sebelumnya sedang diambil kembali ke pengelolaan. Tunggu hingga selesai.
- **Reattached** — penanda sementara pada baris akun: proses berhasil diambil alih setelah pemulaian ulang.
- **Frozen at HH:mm:ss** — di layar **Monitoring**, berarti tampilan data dibekukan (bukan mode **Live**). Untuk mengembalikan data langsung, beralih ke **Live** atau matikan **Freeze**.

**Cara melihat detail.** Arahkan kursor ke sebuah glif status untuk memperoleh tooltip: sejak kapan keadaan berlangsung, pada langkah mana akun berada, dan apa peristiwa terakhirnya.

![contoh status di tabel akun](../images/status-badges.png)

---

# 9. Notifikasi

Aplikasi melaporkan peristiwa dalam tiga cara: **toast** (muncul di sudut dan menghilang), **bilah status** (ringkasan tetap di bawah), dan **banner sebaris** (terikat ke layar tertentu).

## Toast

Mereka muncul di sudut kanan bawah.

| Notifikasi | Mengapa muncul | Artinya | Apa yang dilakukan | Bisakah diabaikan |
|---|---|---|---|---|
| **Saved** | Anda mengubah suatu pengaturan | Perubahan tersimpan | Tak ada | Ya, menghilang sendiri |
| Sukses operasi (hijau) | Sebuah tindakan selesai dengan sukses | Semuanya baik | Tak ada | Ya, menghilang setelah ~5 detik |
| Peringatan (kuning) | Anomali non-kritis diketahui | Layak dilihat | Secara opsional lihat detailnya | Biasanya ya, menghilang setelah ~10 detik |
| Kesalahan (merah) | Sebuah operasi gagal | Tindakan diperlukan | Klik **View** atau **Retry** | Tidak, tetap sampai ditutup |
| Mogok | Sebuah klien menutup tak terduga | Sebuah akun mogok | Klik **Restart** atau buka dump | Tidak, tetap sampai diakui |

**Perlu diketahui.**
- Mengarahkan kursor ke sebuah notifikasi menghentikan penghitung auto-tutup — Anda bisa membacanya dengan tenang.
- Notifikasi identik diciutkan menjadi satu dengan penghitung, misalnya `… failed (×4)`.

## Bilah status

Di sisi kanan bilah status, notifikasi belum dibaca yang paling penting ditampilkan, misalnya `● 3 errors`. Mengekliknya membuka pusat notifikasi.

## Banner sebaris

Mereka muncul di bagian atas layar dan berlaku untuk keseluruhannya. Contoh: `⚠ Steam network degraded — 12 accounts retrying login`. Sebuah banner bisa ditutup dengan tombol **Dismiss** jika ia tidak memblokir. Banner yang memblokir (misalnya, saat sebuah layanan tak tersedia) tetap sampai masalahnya teratasi.

## Peringatan suara

Suara mati secara bawaan. Anda bisa mengaktifkannya untuk peristiwa tertentu (misalnya, **Match found** atau **Crash**) di **Settings → Notifications**. Suara untuk **Match found** berguna untuk tahu pertandingan ditemukan tanpa menatap layar — penerimaan pertandingan itu sendiri terjadi otomatis.

![toast kesalahan dengan tombol View dan Retry](../images/notification-error-toast.png)

---

# 10. Kesalahan dan pemecahan masalah

Kesalahan saat menjalankan farm itu lumrah, dan aplikasi membantu Anda menyelesaikannya. Berikut situasi umum dalam format “Masalah → Kemungkinan penyebab → Solusi → Hasil yang diharapkan”.

## Tidak bisa mengaktifkan lisensi

**Masalah.** Saat memasukkan kunci, aplikasi tak membiarkan Anda lanjut.

| Pesan | Kemungkinan penyebab | Solusi |
|---|---|---|
| “License key invalid” | Kunci dimasukkan dengan salah ketik | Periksa ejaannya. Lebih mudah menempel kunci dengan **Paste from clipboard** |
| “Used on max devices” | Lisensi sudah dipakai pada jumlah perangkat maksimum | Bebaskan lisensi pada perangkat lain, lalu coba lagi. Tombol **Manage devices** menuju pengelolaan perangkat |
| “Cannot reach license server” | Tak ada koneksi ke server lisensi | Periksa koneksi internet Anda dan klik **Retry** |

**Hasil yang diharapkan.** Dengan kunci yang benar dan koneksi ke server, jendela aktivasi menutup dan **Dashboard** terbuka.

## Sebuah akun tak mau diluncurkan

**Masalah.** Anda mengeklik **Start**, tetapi akun tak berpindah ke **Running**.

- **Kemungkinan penyebab.** Akun tak terikat ke sandbox.
  **Solusi.** Buka menu konteks akun → **Bind sandbox…** dan tetapkan sebuah sandbox.
- **Kemungkinan penyebab.** Autentikasi ulang diperlukan (detail login basi); penanda “Reauth required” ada di sebelah baris.
  **Solusi.** Menu konteks → **Re-auth (Steam Guard)**.
- **Kemungkinan penyebab.** Steam untuk sementara membatasi laju login.
  **Solusi.** Tunggu sekitar semenit dan klik **Retry**.

**Hasil yang diharapkan.** Status berpindah **Starting → Running**.

## Steam berlama-lama di Waiting/Starting

**Masalah.** Akun macet pada tahap login.

- **Kemungkinan penyebab.** Login lambat atau masalah jaringan Steam sementara.
  **Solusi.** Beri sedikit waktu. Jika status **Error** muncul, klik **Retry**. Jika jaringan Steam tak stabil, banner peringatan muncul di atas — tunggu hingga pulih.

**Hasil yang diharapkan.** Akun masuk dan berpindah ke **Running**.

## Sebuah klien mogok

**Masalah.** Akun mendapat status **Crashed**.

- **Kemungkinan penyebab.** Klien CS2 atau Steam keluar tak terduga.
  **Solusi.** Pada notifikasi yang muncul, klik **Restart**. Pemulihan sering sudah berlangsung otomatis. Detail mogok ada di layar **Monitoring** pada aliran **Crashes & Warnings**.

**Hasil yang diharapkan.** Akun dimulai ulang dan kembali ke **Running**.

## Sebuah party masuk Desync

**Masalah.** Party berada dalam keadaan **Desync** — anggota dalam keadaan tak konsisten.

- **Kemungkinan penyebab.** Satu anggota menerima pertandingan dan yang lain tak tepat waktu, atau seseorang keluar dari antrean.
  **Solusi.** Klik **Re-sync** untuk menjeda antrean dan menunggu konsistensi. Jika satu akun bermasalah, keluarkan dengan **Drop member** dan antrekan sisanya lagi.

**Hasil yang diharapkan.** Party kembali ke keadaan **Quorum** dan siap diantrekan lagi.

## Peluncuran massal selesai dengan kesalahan

**Masalah.** Setelah **Start** massal, beberapa akun tak jalan.

- **Solusi.** Pada ringkasan, klik **Filter to failed** — tabel hanya menampilkan akun bermasalah. Selesaikan masing-masing berdasarkan penyebab di atas dan luncurkan lagi.

**Hasil yang diharapkan.** Setelah penyebab teratasi, **Start** berulang memindahkan akun ke **Running**.

## Data sebuah layar tak mau memuat

**Masalah.** Alih-alih konten layar, ada banner atau pesan bahwa sebuah layanan tak tersedia.

- **Kemungkinan penyebab.** Sebuah layanan latar sementara tak tersedia.
  **Solusi.** Klik **Retry**. Jika tak membantu, klik **Open logs** untuk melihat detail, atau mulai ulang aplikasi.

**Hasil yang diharapkan.** Layar memuat dan menampilkan data terkini.

## Aplikasi melaporkan Orphan process

**Masalah.** Di pusat notifikasi, pesan seperti “Orphan process … — Adopt or Kill?”.

- **Kemungkinan penyebab.** Sebuah proses dari sesi sebelumnya tersisa yang tak bisa diikat otomatis ke sebuah akun.
  **Solusi.** Pilih **Adopt** (ambil ke pengelolaan) jika proses diperlukan, atau **Kill** (akhiri) jika tidak.

**Hasil yang diharapkan.** Daftar proses tertata rapi.

## Komputer lambat dan mogok makin sering

**Masalah.** Ketidakstabilan umum, kegagalan sering.

- **Kemungkinan penyebab.** Lebih banyak akun berjalan daripada yang bisa ditangani komputer.
  **Solusi.** Buka **Monitoring** dan lihat **CPU** dan **RAM**. Jika nilainya mendekati batas, hentikan beberapa akun dengan **Stop**.

**Hasil yang diharapkan.** Beban turun dan operasi menstabil.

> **Kode kesalahan.** Detail kesalahan menyertakan kode singkat seperti `[E-1042]`. Anda bisa menyalinnya dan memakainya saat menghubungi dukungan. Referensi lengkap kode tersedia melalui **Help → Error reference**.

![contoh layar kesalahan dengan tombol Retry / Open logs](../images/error-screen.png)

---

# 11. Praktik terbaik

## Menyiapkan akun

- Tambahkan akun sebagai daftar melalui **Import** — lebih cepat dan lebih sedikit salah ketik.
- Biarkan penetapan sandbox pada **Auto-assign** kecuali Anda butuh ikatan tertentu.
- Gunakan **Tags** untuk mengelompokkan akun dan memfilternya cepat.

## Meluncurkan banyak akun

- Luncurkan dalam batch: mulai dengan kelompok kecil, pastikan stabilitas, lalu tambahkan lagi.
- Jaga **Dashboard** atau **Monitoring** tetap terbuka untuk mengawasi beban secara waktu nyata.
- Targetkan yang disarankan 4–10 akun CS2 sekaligus; Anda bisa menjalankan lebih banyak di PC bertenaga dan lebih sedikit di mesin yang lemah.

## Bekerja dengan tata letak

- Siapkan lebih dulu beberapa preset untuk situasi berbeda (misalnya, “4-stack”, “single focused”).
- Setelah sebuah tata letak keliru, segera gunakan **Revert layout**, selama jendela pengembalian satu menit masih aktif.

## Menghentikan dengan aman

- Hentikan akun dengan tombol **Stop** (penutupan mulus) alih-alih menutup jendela dengan tangan.
- Sebelum keluar dari aplikasi, hentikan akun aktif. Jika Anda mencoba menutup aplikasi saat skenario berjalan, ia memperingatkan Anda.

## Menghindari gangguan

- Sebelum mengantre, pastikan party berada dalam keadaan **Quorum**.
- Awasi banner tentang keadaan jaringan Steam — saat tak stabil, lebih baik menunggu.

## Menjaga operasi tetap stabil

- Periksa **Dashboard** secara berkala — ia menampilkan keadaan keseluruhan dalam hitungan detik.
- Jaga jumlah akun yang berjalan bersamaan dalam kapasitas komputer Anda.
- Biarkan pemulihan otomatis bekerja beberapa detik sebelum Anda turun tangan sendiri.

---

# 12. Pertanyaan yang sering diajukan

**Mengapa saya tak bisa meluncurkan sebuah akun?**
Kemungkinan besar akun tak terikat ke sandbox — tanpanya ia tak bisa diluncurkan. Ikat satu melalui menu konteks → **Bind sandbox…**. Peluncuran juga bisa terhalang oleh keperluan autentikasi ulang (penanda “Reauth required”) — dalam kasus itu jalankan **Re-auth**.

**Mengapa Steam berlama-lama dalam keadaan menunggu?**
Ini biasanya login lambat atau tundaan jaringan Steam sementara. Beri sedikit waktu. Jika status **Error** muncul, klik **Retry**.

**Bagaimana saya memulai ulang alur kerja?**
Pilih akun atau instance yang Anda butuhkan dan klik **Restart** (atau `Ctrl+Shift+R`). Untuk operasi massal, aplikasi meminta konfirmasi.

**Apa yang terjadi jika aplikasi menutup?**
Akun dan pengaturan Anda tersimpan. Pada peluncuran berikutnya, aplikasi mencoba mengambil kembali proses sesi sebelumnya ke pengelolaan — indikator **Recovering** muncul di bilah status. Jika skenario aktif saat menutup, aplikasi memperingatkan Anda lebih dahulu.

**Bagaimana saya tahu semuanya bekerja?**
Periksa bilah status di bawah dan **Dashboard**. Tanda operasi normal: akun dalam status **Running**, tak ada penanda merah di kartu **Errors** atau tabel **Failures & Crashes**, serta beban **CPU** dan **RAM** dalam rentang normal.

**Di mana kata sandi saya disimpan?**
Hanya di komputer Anda. Semua dienkripsi dengan proteksi bawaan Windows, tak pernah disimpan sebagai teks biasa, dan tak pernah dikirim ke mana pun.

**Apakah FarmPanel bermain untuk saya?**
Tidak. Ia bukan bot atau auto-farmer. Aplikasi mengelola peluncuran, pemantauan, pembangunan lobi, dan pemulihan, sementara semua tindakan di dalam gim dilakukan oleh Anda.

**Apakah saya harus memasukkan kunci lisensi setiap kali?**
Tidak. Kunci dimasukkan sekali, saat aktivasi pertama. Setelah itu aplikasi terbuka langsung ke **Dashboard**.

**Bagaimana saya cepat menemukan sebuah tindakan kalau lupa letak tombolnya?**
Tekan `Ctrl+K` untuk membuka palet perintah. Mulai mengetik nama sebuah tindakan, layar, atau nama pengguna akun, lalu pilih yang Anda butuhkan dari daftar.

**Bisakah saya memindahkan monitoring ke monitor kedua?**
Bisa. Di layar **Monitoring**, klik tombol lepas — layar terbuka sebagai jendela terpisah yang bisa Anda letakkan di monitor kedua. Posisinya diingat.

**Bagaimana saya mengatur ulang pengaturan ke bawaan?**
Di **Settings → Advanced** ada **Reset to defaults**. Untuk melindungi dari klik tak sengaja, aplikasi meminta Anda mengonfirmasi dengan mengetik teks.

---

*Akhir Panduan Pengguna FarmPanel.*

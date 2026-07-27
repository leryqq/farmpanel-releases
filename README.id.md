<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Aplikasi desktop FarmPanel, layar Akun: navigasi samping (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) dan tabel akun dengan kolom status, login, nama panggilan, workflow, sandbox, dan login terakhir"/>

<br/>

# FARMPANEL

**Panel farm akun Steam & CS2 — orkestrasi multi-akun untuk Windows**

`jalankan · isolasi · pantau · pulihkan`

FarmPanel adalah panel desktop Windows untuk menjalankan **farm akun Steam**
dalam skala besar. FarmPanel meluncurkan, mengisolasi dalam sandbox,
memantau, dan memulai ulang secara otomatis setiap **akun CS2** di farm
Anda — dari lima akun hingga ratusan — dari satu jendela, tanpa autofarm dan
tanpa bot.

[**Unduh untuk Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Situs web](https://farmpanel.cc) ·
[Produk](https://farmpanel.cc/id/product) ·
[Telegram](https://t.me/farmpanel_id)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__id-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_id)

Juga tersedia dalam: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Tiếng Việt](./README.vi.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## Apa itu FarmPanel

Jika Anda menjalankan lebih dari satu akun Steam, Anda pasti kenal rutinitas
ini: belasan jendela terbuka sekaligus, klien CS2 yang macet dan harus Anda
sadari lalu jalankan ulang secara manual, serta tidak ada cara mudah untuk
tahu siapa yang tersangkut di layar loading dan siapa yang sudah dalam
pertandingan. Semakin banyak akun di farm, semakin berat pekerjaannya.

**FarmPanel adalah panel farm akun Steam dan CS2 yang dibuat khusus untuk
menghilangkan rutinitas itu.** Ini adalah aplikasi desktop Windows yang
meluncurkan, mengisolasi, dan memantau seluruh farm multi-akun dari satu
jendela — alternatif nyata untuk mengelola multi-akun Steam secara manual,
atau menyulap tumpukan skrip dan mesin virtual.

FarmPanel **bukan bot autofarm**. Ia tidak bermain untuk Anda dan tidak
meniru tindakan dalam game — ia mengelola semua yang terjadi *di sekitar*
game: menjalankan klien, mengirim undangan lobi, memulihkan sesi yang macet,
dan memberi Anda visibilitas langsung atas setiap akun. Setiap tindakan
dalam game tetap di tangan orang sungguhan, sehingga farm Anda berperilaku —
dan terlihat — seperti pemain sungguhan, karena memang begitu.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Mengapa pemilik farm memilih FarmPanel

**01 — Tidak ada autofarm, sama sekali.**
FarmPanel tidak pernah bermain untuk Anda. Setiap tindakan dalam game
dilakukan secara manual, jadi akun tampak seperti manusia, karena memang
begitu.

**02 — Atur sekali saja.**
Setiap peluncuran dan login menjalankan urutan deterministik yang sama. Yang
berhasil kemarin akan berhasil besok, tanpa kejutan.

**03 — Kerusakan pulih sendiri.**
Jika Steam atau CS2 mati, FarmPanel menyadarinya dan mengembalikannya dalam
hitungan detik, tanpa pengawasan.

**04 — Isolasi sandbox yang sesungguhnya.**
Setiap akun berjalan di lingkungannya sendiri yang terisolasi — tanpa sesi
bersama, tanpa berkas bersama, tanpa percampuran sidik jari antar-akun.

**05 — Kata sandi tidak pernah keluar dari PC Anda.**
Kredensial dienkripsi dengan keamanan bawaan Windows dan disimpan hanya di
komputer Anda, tidak pernah dikirim ke mana pun.

**06 — Visibilitas langsung atas setiap akun.**
Dasbor waktu nyata per akun: status, keadaan pertandingan, waktu aktif. Tidak
perlu menebak-nebak apa yang sedang dilakukan farm.

**07 — Perutean jaringan per akun.**
Pilih region server terbaik untuk setiap akun; FarmPanel mengatur jaringannya
untuk Anda.

**08 — Tumbuh bersama farm Anda.**
Mulai dengan lima akun, kembangkan hingga ratusan. Panel yang sama, alur
kerja yang sama, dari awal hingga akhir.

## Cara memulai

1. Unduh pemasang — **[Unduh untuk Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   di atas, atau dari halaman [Releases](https://github.com/leryqq/farmpanel-releases/releases) repositori ini.
2. Jalankan `Setup.exe`. FarmPanel memeriksa sistem Anda dan memandu penyiapan langkah demi langkah.
3. Tambahkan akun Steam Anda dan jalankan farm pertama Anda.

```
persyaratan:   Windows 10/11 (64-bit) · .NET 8
disarankan:    RAM 32 GB · SSD · 16-32 akun CS2 bersamaan
pembaruan:     otomatis, dari repositori ini
```

## Pertanyaan umum

**Apakah FarmPanel bermain game untuk saya?**
Tidak — itulah intinya. Tidak ada bot dan tidak ada autofarm. FarmPanel
mengelola akun: meluncurkan, memantau, menyusun lobi, memperbaiki kerusakan.
Semua yang di dalam game dilakukan oleh Anda, sehingga akun Anda berperilaku
seperti pemain sungguhan, karena memang begitu.

**Di mana kata sandi saya disimpan?**
Hanya di komputer Anda. Kata sandi dienkripsi dengan keamanan bawaan Windows,
tidak pernah disimpan sebagai teks biasa, dan tidak pernah dikirim ke mana
pun.

**Apakah hanya mendukung CS2?**
CS2 memiliki dukungan terdalam saat ini, termasuk telemetri pertandingan
waktu nyata. Game lain sedang dalam perjalanan.

**Berapa biayanya?**
Harga bergantung pada ukuran farm. [Hubungi kami di Telegram](https://t.me/farmpanel_id)
dan kami akan menyesuaikan paket dengan konfigurasi Anda — dari setup kecil
hingga ratusan akun.

Jawaban lain ada di [FAQ produk](https://farmpanel.cc/id/product#faq).

## Panduan & sumber daya

- [Cara menjalankan banyak akun Steam dengan aman](https://farmpanel.cc/id/guides/run-multiple-steam-accounts-safely)
- [Sandboxing akun Steam, dijelaskan](https://farmpanel.cc/id/guides/steam-account-sandboxing)
- [Berapa banyak akun CS2 yang bisa dijalankan satu PC?](https://farmpanel.cc/id/guides/how-many-cs2-accounts-per-pc)
- [Drop mingguan CS2, dijelaskan](https://farmpanel.cc/id/guides/cs2-weekly-drop-explained)
- [Risiko ban multi-akun CS2](https://farmpanel.cc/id/guides/cs2-multi-account-ban-risks)
- [Apakah Anda butuh akun Prime untuk farming CS2?](https://farmpanel.cc/id/guides/prime-accounts-for-cs2-farming)
- [Ekonomi farming case CS2](https://farmpanel.cc/id/guides/cs2-case-farming-economics)
- [Menjual drop CS2 dan mencairkan uang](https://farmpanel.cc/id/guides/sell-cs2-drops-steam-market)
- [Farm CS2: manual vs. dengan panel](https://farmpanel.cc/id/compare/manual-multi-accounting)

## Tautan

| | |
| --- | --- |
| Situs web | [farmpanel.cc](https://farmpanel.cc) |
| Produk | [farmpanel.cc/id/product](https://farmpanel.cc/id/product) |
| Changelog | [farmpanel.cc/id/changelog](https://farmpanel.cc/id/changelog) |
| Telegram | [t.me/farmpanel_id](https://t.me/farmpanel_id) |

---

<div align="center">

Repositori ini hanya mendistribusikan biner FarmPanel yang ditandatangani.
Kode sumber aplikasi bersifat proprietary dan tertutup.

`status sistem · semua sistem beroperasi`

**FarmPanel Systems** · Semua hak dilindungi

</div>

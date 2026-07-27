<div align="center">

<img src="assets/dashboard-banner.svg" width="100%" alt="Ứng dụng máy tính FarmPanel, màn hình Tài khoản: thanh điều hướng bên (Dashboard, Accounts, Workflows, Monitoring, Sandboxes, Servers, Matchmaking, Lobby, Logs) và bảng tài khoản với các cột trạng thái, đăng nhập, biệt danh, workflow, sandbox và lần đăng nhập gần nhất"/>

<br/>

# FARMPANEL

**Bảng điều khiển farm tài khoản Steam & CS2 — điều phối đa tài khoản trên Windows**

`khởi chạy · cô lập · giám sát · phục hồi`

FarmPanel là bảng điều khiển desktop Windows để vận hành một **farm tài khoản
Steam** ở quy mô lớn. Nó khởi chạy, cô lập trong sandbox, theo dõi và tự động
khởi động lại từng **tài khoản CS2** trong farm của bạn — từ năm tài khoản
đến vài trăm — chỉ từ một cửa sổ, không autofarm và không bot.

[**Tải cho Windows**](https://github.com/leryqq/farmpanel-releases/releases/latest) ·
[Trang web](https://farmpanel.cc) ·
[Sản phẩm](https://farmpanel.cc/vi/product) ·
[Telegram](https://t.me/farmpanel_vn)

[![release](https://img.shields.io/github/v/release/leryqq/farmpanel-releases?label=release&color=c9c9d2&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases/latest)
[![windows](https://img.shields.io/badge/windows-10%20%2F%2011-0078D6?labelColor=07070a&style=flat-square)](https://farmpanel.cc)
[![downloads](https://img.shields.io/github/downloads/leryqq/farmpanel-releases/total?label=downloads&color=b6f0c9&labelColor=07070a&style=flat-square)](https://github.com/leryqq/farmpanel-releases/releases)
[![telegram](https://img.shields.io/badge/telegram-farmpanel__vn-d9b8f0?labelColor=07070a&style=flat-square)](https://t.me/farmpanel_vn)

Cũng có sẵn bằng: [English](./README.md) · [Русский](./README.ru.md) · [Español](./README.es.md) · [Português](./README.pt.md) · [Français](./README.fr.md) · [Türkçe](./README.tr.md) · [Bahasa Indonesia](./README.id.md) · [हिन्दी](./README.hi.md) · [中文](./README.zh.md) · [العربية](./README.ar.md)

</div>

---

## FarmPanel là gì

Nếu bạn chạy nhiều hơn một tài khoản Steam, bạn đã quá quen với cảnh này:
cả chục cửa sổ mở cùng lúc, một client CS2 bị treo mà bạn phải để ý rồi mở
lại bằng tay, và không có cách nào gọn gàng để biết ai đang kẹt ở màn hình
tải và ai đã vào trận. Càng thêm tài khoản vào farm, công việc càng nặng.

**FarmPanel là bảng điều khiển farm tài khoản Steam và CS2 được tạo ra chính
để xóa bỏ công việc nhàm chán đó.** Đây là ứng dụng desktop Windows khởi
chạy, cô lập và giám sát toàn bộ farm đa tài khoản chỉ từ một cửa sổ — một
giải pháp thay thế thực sự cho việc quản lý đa tài khoản Steam bằng tay, hay
chắp vá một mớ script và máy ảo.

FarmPanel **không phải bot autofarm**. Nó không chơi thay bạn và không mô
phỏng thao tác trong game — nó quản lý mọi thứ *xung quanh* game: khởi chạy
client, gửi lời mời lobby, phục hồi các phiên bị treo, và cho bạn khả năng
theo dõi trực tiếp từng tài khoản. Mọi thao tác trong game vẫn nằm trong tay
người thật, nên farm của bạn hành xử — và trông — như người chơi thật, bởi
vì đúng là như vậy.

```
orchestrator: launch sandbox#42
steam:        client ready (acct_2418)
cs2:          lobby created · slot 1/5
gsi:          match_state = warmup
recovery:     ok · health 1.00
```

## Vì sao các chủ farm chọn FarmPanel

**01 — Không autofarm, không bao giờ.**
FarmPanel không bao giờ chơi thay bạn. Mọi thao tác trong game đều làm bằng
tay, nên tài khoản trông giống người thật, bởi vì đúng là như vậy.

**02 — Thiết lập một lần.**
Mỗi lần khởi chạy và đăng nhập đều theo cùng một trình tự xác định. Cái gì
chạy được hôm qua thì mai vẫn chạy được, không bất ngờ.

**03 — Sự cố tự khắc phục.**
Nếu Steam hoặc CS2 sập, FarmPanel nhận ra và đưa nó trở lại trong vài giây,
không cần bạn can thiệp.

**04 — Cô lập sandbox thực sự.**
Mỗi tài khoản chạy trong môi trường cô lập riêng — không phiên chung, không
tệp chung, không trộn lẫn dấu vân tay giữa các tài khoản.

**05 — Mật khẩu không bao giờ rời khỏi PC của bạn.**
Thông tin đăng nhập được mã hóa bằng bảo mật tích hợp của Windows và chỉ lưu
trên máy của bạn, không bao giờ gửi đi đâu.

**06 — Theo dõi trực tiếp từng tài khoản.**
Một bảng điều khiển thời gian thực cho mỗi tài khoản: trạng thái, tình trạng
trận đấu, thời gian hoạt động. Không phải đoán xem farm đang làm gì.

**07 — Định tuyến mạng theo từng tài khoản.**
Chọn khu vực máy chủ tốt nhất cho mỗi tài khoản; FarmPanel cấu hình mạng
giúp bạn.

**08 — Lớn lên cùng farm của bạn.**
Bắt đầu với năm tài khoản, mở rộng đến hàng trăm. Vẫn cùng một bảng điều
khiển, cùng một quy trình, từ đầu đến cuối.

## Bắt đầu

1. Tải trình cài đặt — **[Tải cho Windows](https://github.com/leryqq/farmpanel-releases/releases/latest)**
   ở trên, hoặc từ trang [Releases](https://github.com/leryqq/farmpanel-releases/releases) của kho này.
2. Chạy `Setup.exe`. FarmPanel kiểm tra hệ thống của bạn và hướng dẫn cài đặt từng bước.
3. Thêm các tài khoản Steam của bạn và khởi chạy farm đầu tiên.

```
yêu cầu:       Windows 10/11 (64-bit) · .NET 8
khuyến nghị:   32 GB RAM · SSD · 16-32 tài khoản CS2 đồng thời
cập nhật:      tự động, từ kho này
```

## Câu hỏi thường gặp

**FarmPanel có chơi game thay tôi không?**
Không — đó chính là điểm mấu chốt. Không có bot và không có autofarm.
FarmPanel quản lý tài khoản: khởi chạy, giám sát, dựng lobby, khắc phục sự
cố. Mọi thứ trong game do bạn làm, nên tài khoản của bạn hành xử như người
chơi thật, bởi vì đúng là như vậy.

**Mật khẩu của tôi được lưu ở đâu?**
Chỉ trên máy của bạn. Chúng được mã hóa bằng bảo mật tích hợp của Windows,
không bao giờ lưu ở dạng văn bản thuần và không bao giờ gửi đi đâu.

**Nó chỉ hỗ trợ CS2 thôi sao?**
Hiện tại CS2 được hỗ trợ sâu nhất, bao gồm cả telemetry trận đấu thời gian
thực. Các game khác đang trên đường tới.

**Chi phí bao nhiêu?**
Giá phụ thuộc vào quy mô farm. [Nhắn cho chúng tôi trên Telegram](https://t.me/farmpanel_vn)
và chúng tôi sẽ chọn gói phù hợp với cấu hình của bạn — từ thiết lập nhỏ đến
hàng trăm tài khoản.

Thêm câu trả lời tại [FAQ sản phẩm](https://farmpanel.cc/vi/product#faq).

## Hướng dẫn & tài nguyên

- [Cách chạy nhiều tài khoản Steam an toàn](https://farmpanel.cc/vi/guides/run-multiple-steam-accounts-safely)
- [Sandbox tài khoản Steam, giải thích](https://farmpanel.cc/vi/guides/steam-account-sandboxing)
- [Một PC chạy được bao nhiêu tài khoản CS2?](https://farmpanel.cc/vi/guides/how-many-cs2-accounts-per-pc)
- [Drop hằng tuần của CS2, giải thích](https://farmpanel.cc/vi/guides/cs2-weekly-drop-explained)
- [Rủi ro khóa tài khoản khi đa tài khoản CS2](https://farmpanel.cc/vi/guides/cs2-multi-account-ban-risks)
- [Bạn có cần tài khoản Prime để farm CS2 không?](https://farmpanel.cc/vi/guides/prime-accounts-for-cs2-farming)
- [Kinh tế của việc farm hòm CS2](https://farmpanel.cc/vi/guides/cs2-case-farming-economics)
- [Bán drop CS2 và rút tiền](https://farmpanel.cc/vi/guides/sell-cs2-drops-steam-market)
- [Farm CS2: bằng tay vs. bằng bảng điều khiển](https://farmpanel.cc/vi/compare/manual-multi-accounting)

## Liên kết

| | |
| --- | --- |
| Trang web | [farmpanel.cc](https://farmpanel.cc) |
| Sản phẩm | [farmpanel.cc/vi/product](https://farmpanel.cc/vi/product) |
| Changelog | [farmpanel.cc/vi/changelog](https://farmpanel.cc/vi/changelog) |
| Telegram | [t.me/farmpanel_vn](https://t.me/farmpanel_vn) |

---

<div align="center">

Kho này chỉ phân phối các tệp nhị phân FarmPanel đã được ký.
Mã nguồn của ứng dụng là độc quyền và đóng.

`trạng thái hệ thống · mọi hệ thống hoạt động bình thường`

**FarmPanel Systems** · Bảo lưu mọi quyền

</div>

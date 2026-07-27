# Hướng dẫn sử dụng FarmPanel

**Bảng điều khiển cho trang trại tài khoản Steam và CS2 của bạn trên Windows**

Phiên bản tài liệu: 1.0

🌐 [English](USER-GUIDE.md) · [Русский](USER-GUIDE.ru.md) · [Español](USER-GUIDE.es.md) · [Português](USER-GUIDE.pt.md) · [Français](USER-GUIDE.fr.md) · [Türkçe](USER-GUIDE.tr.md) · [Bahasa Indonesia](USER-GUIDE.id.md) · **Tiếng Việt** · [हिन्दी](USER-GUIDE.hi.md) · [中文](USER-GUIDE.zh.md) · [العربية](USER-GUIDE.ar.md)

---

> **Cách đọc hướng dẫn này.** Các nút, tab và trạng thái xuất hiện trong ứng dụng đúng như được viết **in đậm** (ví dụ: **Add Account**, **Start**, **Running**), để bạn luôn nhấp đúng chỗ. Mỗi quy trình cho bạn biết cần nhấp gì, điều gì xảy ra tiếp theo và cách xác nhận thành công.

## Mục lục

1. [Giới thiệu](#1-giới-thiệu)
2. [Trước khi bắt đầu](#2-trước-khi-bắt-đầu)
3. [Lần khởi chạy đầu tiên](#3-lần-khởi-chạy-đầu-tiên)
4. [Tổng quan giao diện](#4-tổng-quan-giao-diện)
5. [Các quy trình cốt lõi](#5-các-quy-trình-cốt-lõi)
6. [Tác vụ thường gặp («Tôi muốn…»)](#6-tác-vụ-thường-gặp-tôi-muốn)
7. [Tham chiếu tính năng](#7-tham-chiếu-tính-năng)
8. [Trạng thái và chỉ báo](#8-trạng-thái-và-chỉ-báo)
9. [Thông báo](#9-thông-báo)
10. [Lỗi và khắc phục sự cố](#10-lỗi-và-khắc-phục-sự-cố)
11. [Thực hành tốt nhất](#11-thực-hành-tốt-nhất)
12. [Câu hỏi thường gặp](#12-câu-hỏi-thường-gặp)

---

# 1. Giới thiệu

## FarmPanel là gì

**FarmPanel** là một ứng dụng máy tính để bàn trên Windows giúp bạn quản lý nhiều tài khoản Steam và máy khách Counter-Strike 2 từ một cửa sổ duy nhất. Thay vì mở hàng chục cửa sổ Steam bằng tay, canh chừng từng cái và khởi động lại những cái bị treo, bạn quản lý toàn bộ trang trại tài khoản một cách tập trung — từ một bảng điều khiển rõ ràng.

FarmPanel khởi chạy máy khách, cô lập các tài khoản với nhau, theo dõi trạng thái của chúng theo thời gian thực và tự động phục hồi chúng sau sự cố.

> **Quan trọng.** FarmPanel **không phải bot và không phải công cụ auto-farm**. Nó không chơi thay bạn và không mô phỏng các hành động trong game. Nó quản lý mọi thứ diễn ra *xung quanh* game: khởi chạy máy khách, mời vào sảnh, phục hồi sau sự cố và hiển thị trực tiếp cho từng tài khoản. Mọi hành động trong game đều do người thật thực hiện.

## Nó giải quyết vấn đề gì

Nếu bạn có nhiều hơn một tài khoản, thói quen này hẳn quen thuộc:

- bạn phải khởi chạy hàng chục máy khách Steam và CS2;
- mỗi tài khoản phải chạy riêng, không can thiệp lẫn nhau;
- xây sảnh và gửi lời mời bằng tay thì chậm và mệt;
- một CS2 bị treo phải được nhận ra và khởi động lại kịp thời;
- khó biết ai đã vào trận và ai đang kẹt ở màn tải.

FarmPanel loại bỏ thói quen này và đưa mọi thao tác vào một ứng dụng duy nhất.

## Dành cho ai

Ứng dụng được xây dựng cho bất kỳ ai cần quản lý tập trung nhiều tài khoản Steam và CS2 — từ vài cái đến vài trăm — với khởi chạy tự động, giám sát trực tiếp và phục hồi đáng tin cậy sau sự cố.

## Bạn có thể làm gì

- Giữ tất cả tài khoản ở một nơi và nhanh chóng tìm cái bạn cần.
- Khởi động và dừng tài khoản từng cái một hoặc tất cả cùng lúc.
- Cô lập từng tài khoản trong môi trường được bảo vệ riêng (một sandbox).
- Lập các party gồm nhiều tài khoản và cho chúng vào hàng chờ ghép trận cùng nhau.
- Theo dõi tải máy tính, tình trạng tiến trình và sự cố treo theo thời gian thực.
- Tự động phục hồi tài khoản sau khi treo hoặc sau khi ứng dụng bị đóng.
- Sắp xếp các cửa sổ CS2 trên các màn hình bằng một bố cục dựng sẵn.

![Màn hình chính của FarmPanel (Dashboard)](../images/dashboard-overview.png)

---

# 2. Trước khi bắt đầu

## Yêu cầu hệ thống

| Mục | Tối thiểu | Khuyến nghị |
|---|---|---|
| Hệ điều hành | Windows 10 hoặc 11 (64-bit) | Windows 10 / 11 (64-bit) |
| Bộ nhớ | 8 GB | 32 GB |
| Ổ đĩa | Bất kỳ | SSD |
| Tài khoản đồng thời | 2 | 4–10 tài khoản CS2 |
| Độ phân giải màn hình | Vùng làm việc rộng ít nhất 1280 pixel | Full HD (1920×1080) trở lên |

## Cần chuẩn bị trước

- **Trình cài đặt FarmPanel** — một tệp tên `Setup.exe` mà bạn tải từ trang tải xuống chính thức.
- **Một khóa bản quyền** — bạn nhận được khi mua. Nó trông như thế này: `XXXX-XXXX-XXXX-XXXX-XXXX` (năm nhóm, mỗi nhóm bốn ký tự).
- **Thông tin tài khoản Steam của bạn** — tên đăng nhập và mật khẩu, cùng mã Steam Guard nếu bạn dùng. Bạn có thể nhập từng cái hoặc nhập một danh sách từ tệp.
- **Kết nối internet** — cần cho lần khởi chạy đầu tiên để kích hoạt bản quyền, và sau đó để Steam và CS2 hoạt động.

## Quyền hạn

- Việc cài đặt **không yêu cầu quyền quản trị viên** — ứng dụng chỉ cài cho tài khoản người dùng của bạn.
- Lần đầu chạy trình cài đặt, Windows có thể hiện cửa sổ **SmartScreen** màu xanh (“Windows protected your PC”) — đây là cảnh báo thường lệ cho chương trình mới. Nhấp **More info**, rồi **Run anyway**.
- Ứng dụng có thể cần truy cập mạng (cho Steam) và truy cập các quy tắc Windows Firewall. Nếu xuất hiện lời nhắc từ tường lửa, hãy cho phép truy cập.

## Dữ liệu của bạn được lưu ở đâu

Tên đăng nhập và mật khẩu được mã hóa bằng cơ chế bảo vệ tích hợp của Windows và được lưu **chỉ trên máy tính của bạn**. Chúng không bao giờ được lưu dưới dạng văn bản thuần và không bao giờ được gửi đi đâu.

---

# 3. Lần khởi chạy đầu tiên

Dưới đây là lộ trình từ cài đặt đến một bảng điều khiển sẵn sàng sử dụng. Hãy làm theo các bước theo thứ tự.

## Bước 1. Cài đặt ứng dụng

1. Tải trình cài đặt `Setup.exe` từ trang tải xuống.
2. Nhấp đúp vào tệp `Setup.exe`.
3. Nếu xuất hiện cửa sổ **SmartScreen** màu xanh (“Windows protected your PC”), hãy nhấp **More info**, rồi **Run anyway**. Đây là cảnh báo thường lệ cho chương trình mới, không phải lỗi.
4. Chờ quá trình cài đặt hoàn tất. Không cần quyền quản trị viên — trình cài đặt kiểm tra hệ thống của bạn và chuẩn bị mọi thứ.

**Điều gì xảy ra tiếp theo.** Một biểu tượng FarmPanel xuất hiện trên màn hình nền và trong menu Start.

![cửa sổ trình cài đặt Setup.exe](../images/setup-installer.png)

## Bước 2. Mở ứng dụng

Nhấp đúp vào biểu tượng **FarmPanel** trên màn hình nền.

**Bạn sẽ thấy gì.** Trong lần khởi chạy đầu tiên, khi bản quyền chưa được kích hoạt, **Activation Wizard** (trình hướng dẫn kích hoạt) sẽ mở ra. Màn hình chính chỉ xuất hiện sau khi kích hoạt thành công.

## Bước 3. Kích hoạt bản quyền của bạn

Cửa sổ kích hoạt dẫn bạn từng bước.

1. Gõ hoặc dán khóa bản quyền của bạn vào ô nhập. Để dán từ bộ nhớ tạm, nhấp **Paste from clipboard**.
2. Ứng dụng kiểm tra định dạng khóa khi bạn gõ. Khi định dạng đúng, nút kích hoạt sẽ khả dụng.
3. Nhấp **Activate**.

**Điều gì xảy ra tiếp theo.** Ứng dụng liên hệ máy chủ bản quyền và xác minh khóa. Việc này mất vài giây — bạn sẽ thấy trạng thái **Activating**.

**Dấu hiệu thành công.** Cửa sổ kích hoạt đóng lại và màn hình chính của ứng dụng (**Dashboard**) mở ra. Bản quyền của bạn đã kích hoạt — bạn sẽ không cần nhập lại khóa ở những lần chạy sau.

> **Nếu kích hoạt thất bại**, ứng dụng hiện một thông báo rõ ràng và cho biết bạn cần làm gì. Các trường hợp thường gặp được đề cập ở [10. Lỗi và khắc phục sự cố](#10-lỗi-và-khắc-phục-sự-cố).

![cửa sổ kích hoạt bản quyền](../images/license-activation.png)

## Bước 4. Kiểm tra các thiết lập cơ bản

Trước khi khởi chạy tài khoản lần đầu, bạn nên kiểm tra các thiết lập của mình.

1. Nhấp **Settings** ở bảng bên trái, hoặc nhấn `Ctrl+,`.
2. Mở mục **Sandboxes** và, nếu cần, chọn một thư mục cho các sandbox.
3. Tùy chọn mở **Appearance** và chọn một chủ đề (**System / Dark / Light**) cùng mật độ giao diện.

Các thiết lập tự lưu: sau mỗi thay đổi, một thông báo ngắn **Saved** xuất hiện.

## Bước 5. Sẵn sàng khởi động

Giờ bạn có thể thêm tài khoản và khởi chạy trang trại đầu tiên. Xem [5. Các quy trình cốt lõi](#5-các-quy-trình-cốt-lõi) để biết cách làm.

**Dấu hiệu mọi thứ hoạt động.** Thanh dưới cùng của cửa sổ (thanh trạng thái) hiện một bản tóm tắt: số tài khoản, các tiến trình đang hoạt động và phiên bản ứng dụng hiện tại.

---

# 4. Tổng quan giao diện

Ứng dụng chạy trong một cửa sổ chính duy nhất. Nó gồm các phần tử cố định luôn ở đúng vị trí và một vùng màn hình thay đổi tùy theo mục bạn chọn.

```
┌────────────────────────────────────────────────────────────┐
│  Command Bar                                                │
├──────────┬─────────────────────────────────────────────────┤
│          │                                                 │
│ Sidebar  │   Vùng làm việc của màn hình đã chọn            │
│          │                                                 │
│          │                                                 │
├──────────┴─────────────────────────────────────────────────┤
│  Status Bar                                                 │
└────────────────────────────────────────────────────────────┘
```

![cấu trúc cửa sổ tổng thể với các vùng được gắn nhãn](../images/window-layout.png)

## 4.1. Command Bar (thanh trên cùng)

**Mục đích.** Một dải cố định chạy ngang phía trên cửa sổ. Nó chứa điều hướng, tìm kiếm toàn cục và thông báo.

**Vị trí.** Hàng trên cùng của cửa sổ.

**Các phần tử chính (từ trái sang phải):**

- **Nút hamburger (☰)** — thu gọn và mở rộng thanh bên. Phím tắt `Ctrl+B`.
- **Logo** — nhấp vào sẽ đưa bạn về màn hình chính (**Dashboard**).
- **Breadcrumbs (đường dẫn)** — cho biết bạn đang ở đâu, ví dụ `Accounts › alex_42 › Events`. Nhấp bất kỳ đoạn nào để nhảy tới đó.
- **Tìm kiếm / bảng lệnh** — ở giữa. Nhấn `Ctrl+K` để mở bảng lệnh (xem bên dưới).
- **Huy hiệu thông báo** — một biểu tượng có bộ đếm (ví dụ, `⚠ 3`). Nhấp vào sẽ mở trung tâm thông báo.

**Khi nào dùng.** Command Bar luôn trong tầm tay: để nhảy nhanh giữa các màn hình, tìm một tài khoản theo tên đăng nhập, hoặc chạy một lệnh mà không cần chuột.

### Command Palette

Nhấn `Ctrl+K` bất cứ lúc nào để mở bảng lệnh — một ô tìm kiếm cho mọi hành động và đối tượng trong ứng dụng.

1. Bắt đầu gõ tên của một lệnh, màn hình, tên đăng nhập tài khoản hoặc quy trình.
2. Danh sách thu hẹp về các kết quả khớp. Di chuyển giữa chúng bằng `↑` `↓`.
3. Nhấn `Enter` để chạy mục đã chọn.

**Vì sao hữu ích.** Bảng lệnh là cách nhanh nhất để tìm bất cứ thứ gì mà không cần nhớ vị trí các nút.

![bảng lệnh đang mở](../images/command-palette.png)

## 4.2. Sidebar (thanh bên)

**Mục đích.** Điều hướng chính của ứng dụng.

**Vị trí.** Ở bên trái, cao hết chiều cao cửa sổ.

**Các mục (từ trên xuống dưới):**

| Biểu tượng | Mục | Hiển thị gì |
|---|---|---|
| ▤ | **Dashboard** | Tổng quan toàn bộ trang trại |
| 👥 | **Accounts** | Danh sách tất cả tài khoản (màn hình làm việc chính) |
| ⚙ | **Workflows** | Kịch bản khởi chạy tự động và tiến độ của chúng |
| ⚔ | **Matchmaking** | Party và tìm trận |
| 📈 | **Monitoring** | Tải máy tính và tình trạng tiến trình |
| 📜 | **Logs** | Nhật ký sự kiện |
| ▣ | **Layouts** | Sắp xếp cửa sổ CS2 trên các màn hình |
| ▦ | **Sandboxes** | Sandbox (môi trường cô lập) |
| ⚙ | **Settings** | Thiết lập ứng dụng |
| ? | **Help** | Trợ giúp |

Một số mục hiển thị bộ đếm (ví dụ, số tài khoản) hoặc một chấm trực tiếp khi có hoạt động.

**Các hành động chính:**

- Nhấp một mục để mở nó. Bạn cũng có thể dùng `Ctrl+1`…`Ctrl+8`.
- Nút thu gọn (hoặc `Ctrl+B`) thu nhỏ bảng thành các biểu tượng để dành chỗ.

**Mẹo.** Chuyển giữa các mục vẫn giữ nguyên trạng thái của bạn — bộ lọc, lựa chọn và vị trí cuộn. Khi quay lại một màn hình, bạn thấy nó y như lúc rời đi.

![thanh bên với tất cả các mục](../images/sidebar.png)

## 4.3. Status Bar (thanh trạng thái)

**Mục đích.** Một thanh mỏng ở dưới cùng cửa sổ với bản tóm tắt nhanh về trạng thái của toàn bộ trang trại.

**Vị trí.** Hàng dưới cùng của cửa sổ.

**Hiển thị gì (ví dụ):**

```
[env: PROD] | ● 412 accounts (238 running) | ▶ 18 workflows | ◎ 7 matches | CPU 42% RAM 71% | ⚠ 3 errors | 14:32:08 | v1.0.1
```

- có bao nhiêu tài khoản và hiện bao nhiêu đang chạy;
- có bao nhiêu quy trình và trận đấu đang diễn ra;
- tải bộ xử lý và bộ nhớ;
- số lỗi (nhấp để mở trung tâm thông báo);
- thời gian và phiên bản ứng dụng.

**Khi nào dùng.** Liếc qua thanh trạng thái để trong một giây biết mọi thứ có ổn không.

## 4.4. Màn hình Dashboard

**Mục đích.** Một màn hình tổng quan duy nhất. Trong vài giây, nó trả lời: bao nhiêu tài khoản đang trực tuyến, bao nhiêu quy trình đang chạy hay thất bại, có hoạt động ghép trận không, có sự cố treo nào không, và máy tính tải nặng đến đâu.

**Vị trí.** Mục đầu tiên trong thanh bên. Nó mở ngay sau khi khởi chạy.

**Các vùng chính:**

- **KPI strip** — năm thẻ ở trên cùng: **Accounts**, **Workflows**, **Matches**, **Errors**, **System**. Mỗi thẻ hiện một con số chủ đạo và một biểu đồ nhỏ. Nhấp một thẻ sẽ đưa bạn tới màn hình tương ứng.
- **Live Activity Feed** — một luồng thời gian thực của các sự kiện vận hành. Dùng nút tạm dừng (hoặc phím `Space`) để dừng cuộn.
- **Account State Heatmap** — một lưới trong đó mỗi tài khoản là một ô màu. Màu phản ánh trạng thái của nó. Rê chuột để xem tên đăng nhập và trạng thái; nhấp để nhảy tới tài khoản.
- **Active Workflows / Matchmaking Queue / Sandboxes** — ba ô tóm tắt các quy trình, hàng chờ trận và các sandbox.
- **Failures & Crashes** — một bảng các lỗi và sự cố treo gần đây trong một giờ qua.

**Cách dùng điển hình.** Buổi sáng, mở **Dashboard** để nắm bắt trang trại trong nháy mắt, rồi đi tới nơi cần chú ý.

**Mẹo.**
- Các chỉ số tự làm mới. Để buộc làm mới toàn bộ, nhấn `F5`.
- Nếu có bất cứ thứ gì được tô đỏ ở thẻ **Errors** hoặc bảng lỗi, hãy bắt đầu điều tra từ đó.

![Dashboard với KPI strip và activity feed](../images/dashboard-screen.png)

## 4.5. Màn hình Accounts

**Mục đích.** Màn hình làm việc chính. Ở đây bạn lưu trữ tài khoản, tìm cái cần và khởi động, dừng chúng.

**Vị trí.** Mục thứ hai trong thanh bên (`Ctrl+2`).

**Các vùng chính:**

- **Thanh công cụ** — các nút **Add Account**, **Import**, **Export** và **Refresh**, ô tìm kiếm, bộ lọc và các nút điều khiển hiển thị.
- **Bảng tài khoản** — danh sách tất cả tài khoản với các cột: trạng thái, tên đăng nhập, biệt danh, hạng, quy trình, sandbox, thẻ, thời gian đăng nhập gần nhất, và các cột khác.
- **Details Pane (ngăn chi tiết)** — ở bên phải. Hiển thị chi tiết của tài khoản đã chọn. Hiện hoặc ẩn bằng `Ctrl+\`.

**Bạn có thể làm gì:**

- Thêm tài khoản từng cái hoặc nhập một danh sách.
- Tìm kiếm và lọc tài khoản.
- Khởi động, dừng và khởi động lại một tài khoản hoặc nhiều cái cùng lúc.
- Gắn tài khoản với các sandbox và gán quy trình.
- Xem thẻ tài khoản chi tiết: dữ liệu, lịch sử, sự kiện và nhật ký.

**Cách dùng điển hình.** Chọn các tài khoản bạn cần trong bảng, rồi thực hiện một hành động lên chúng — qua thanh công cụ, menu ngữ cảnh (nhấp chuột phải), hoặc phím tắt.

Hướng dẫn từng bước chi tiết có ở [5. Các quy trình cốt lõi](#5-các-quy-trình-cốt-lõi).

![màn hình Accounts với bảng và ngăn chi tiết](../images/accounts-screen.png)

### Ngăn chi tiết tài khoản (Details Pane)

Bên phải bảng, một thẻ cho tài khoản đã chọn xuất hiện với các tab sau:

| Tab | Hiển thị gì |
|---|---|
| **Overview** | Dữ liệu cốt lõi, liên kết sandbox, quy trình được gán, thẻ, các ngày then chốt và các nút hành động |
| **Inventory** | Kho đồ của tài khoản: số lượng và giá trị vật phẩm |
| **Workflow** | Trạng thái hiện tại của kịch bản được gán và bước hiện tại của nó |
| **Events** | Các sự kiện gần đây cho tài khoản này |
| **Logs** | Nhật ký sự kiện được lọc theo tài khoản này |
| **History** | Lịch sử thay đổi: tạo, chỉnh sửa, đổi tên, gắn lại sandbox |

Ở dưới cùng tab **Overview** là một khối nút: **Start**, **Stop**, **Restart**, **Pause**, cùng **Edit account** và **Delete**. Hành động phù hợp nhất được làm nổi bật: **Start** khi tài khoản đã dừng, và **Stop** khi nó đang chạy.

## 4.6. Màn hình Workflows

**Mục đích.** Quản lý các kịch bản khởi chạy tự động và theo dõi chúng chạy.

**Vị trí.** Mục thứ ba trong thanh bên (`Ctrl+3`).

**Quy trình là gì.** Một quy trình là một chuỗi bước định sẵn mà ứng dụng thực hiện cho một tài khoản: đăng nhập Steam, khởi chạy CS2, v.v. Cùng một kịch bản luôn chạy theo cùng một cách, nên kết quả có thể dự đoán được.

- **Definition** — mẫu kịch bản: một tập hợp các bước.
- **Instance** — một lần chạy của một definition cho một tài khoản cụ thể.

**Các vùng chính:**

- **Bên trái** — danh sách các definition (mẫu) và các phiên bản của chúng.
- **Ở giữa** — bảng các instance đang chạy: kịch bản nào, cho tài khoản nào, ở bước nào, thử lại bao nhiêu lần, bắt đầu khi nào.
- **Bên phải** — chi tiết của instance đã chọn (các tab **Overview**, **State Machine**, **Steps**, **Logs**, **Retries**).
- **Dưới cùng** — một dòng thời gian sự kiện có thể thu gọn cho các instance đang hiển thị (`Ctrl+T`).

**Khi nào dùng.** Vào đây để xem việc khởi chạy của từng tài khoản đang ở bước nào, tạm dừng hoặc khởi động lại một kịch bản, hoặc tìm hiểu vì sao có gì đó không hoàn tất.

![màn hình Workflows với ba ngăn](../images/workflows-screen.png)

## 4.7. Màn hình Matchmaking

**Mục đích.** Lập các party gồm nhiều tài khoản và cho chúng vào hàng chờ ghép trận cùng nhau.

**Vị trí.** Mục thứ tư trong thanh bên (`Ctrl+4`).

**Khái niệm then chốt:**

| Thuật ngữ | Ý nghĩa |
|---|---|
| **Party** | Một nhóm tài khoản cùng tìm trận với nhau |
| **Quorum** | Tất cả thành viên party đã đăng nhập, đang trong hàng chờ và không trong trận |
| **Queue** | Chờ trận: vị trí, khu vực, chế độ |
| **Match Found** | Steam đã tìm được trận. Ứng dụng tự động xác nhận sẵn sàng cho tất cả thành viên — bạn không cần làm gì |
| **Desync** | Các thành viên ở trạng thái không nhất quán (ví dụ, ai đó rớt khỏi hàng chờ) |

**Các vùng chính:**

- **Bên trái** — danh sách các party với trạng thái của chúng (quorum, desync, match found, nhàn rỗi).
- **Bên phải** — chi tiết của party đã chọn: thành viên, trạng thái của họ, vị trí hàng chờ, độ trễ mạng, sandbox.
- **Dưới cùng** — một dòng thời gian các sự kiện ghép trận gần đây.

**Khi nào dùng.** Ở đây bạn lập các party gồm 2–5 tài khoản và đưa chúng vào hàng chờ. Khi tìm được trận, ứng dụng tự động xác nhận sẵn sàng cho tất cả thành viên.

![màn hình Matchmaking với các party và chi tiết](../images/matchmaking-screen.png)

## 4.8. Màn hình Monitoring

**Mục đích.** Theo dõi tải máy tính, tình trạng tiến trình và sự cố treo theo thời gian thực.

**Vị trí.** Mục thứ năm trong thanh bên (`Ctrl+5`).

**Các vùng chính:**

- **Đồng hồ tài nguyên** — các thẻ **CPU**, **RAM**, **Disk**, **Net**, và, nơi có sẵn, **GPU** với giá trị hiện tại và biểu đồ nhỏ.
- **Process Explorer** — bảng tất cả các tiến trình Steam và CS2 đang chạy: mỗi cái thuộc tài khoản nào, tiêu tốn bao nhiêu, đã chạy bao lâu.
- **Crashes & Warnings** — một luồng các sự cố gần đây.
- **Logs panel** — một nhật ký ở dưới cùng màn hình, có thể thu gọn.

**Điều khiển thời gian.** Ở trên cùng bạn có thể chuyển giữa **Live** (thời gian thực), **Last 1h / 24h** và **Custom** (một khoảng tùy chỉnh). Nút **Freeze** (`Ctrl+Space`) đóng băng hình ảnh để bạn có thể nghiên cứu nó thong thả.

**Khi nào dùng.** Nếu máy tính bắt đầu chậm hoặc sự cố treo trở nên thường xuyên, hãy mở **Monitoring** để xem tiến trình nào đang ngốn tài nguyên và chính xác cái gì đã treo.

> **Mẹo.** Bạn có thể mở màn hình **Monitoring** ở một cửa sổ riêng bằng nút tách và đặt nó lên màn hình thứ hai.

![màn hình Monitoring với các đồng hồ và danh sách tiến trình](../images/monitoring-screen.png)

## 4.9. Màn hình Logs

**Mục đích.** Một nhật ký chi tiết về tất cả các sự kiện của ứng dụng — như một dòng chảy trực tiếp về những gì đang diễn ra.

**Vị trí.** Mục thứ sáu trong thanh bên (`Ctrl+6`).

**Tính năng chính:**

- **Bộ lọc mức** — các công tắc **Error**, **Warn**, **Info**, **Debug**. Theo mặc định, các thông báo lỗi, cảnh báo và thông tin được hiển thị.
- **Bộ lọc nguồn** — bạn có thể thu hẹp nhật ký về một tài khoản, quy trình hoặc sandbox duy nhất.
- **Tìm kiếm** — `Ctrl+F`, với nhảy giữa các kết quả (`F3` / `Shift+F3`).
- **Follow** — nhật ký tự cuộn tới các dòng mới. Phím `Space` bật và tắt chế độ theo dõi. Nếu bạn cuộn lên, việc theo dõi tạm dừng và một nút nhảy-xuống-đáy xuất hiện.
- **Export** — lưu các dòng đang hiển thị vào một tệp.

**Khi nào dùng.** Khi bạn cần chi tiết: chính xác điều gì đã xảy ra với một tài khoản cụ thể và theo thứ tự nào.

![màn hình Logs với một nhật ký sự kiện](../images/logs-screen.png)

## 4.10. Màn hình Layouts

**Mục đích.** Sắp xếp các cửa sổ CS2 trên một hoặc nhiều màn hình bằng một bố cục dựng sẵn.

**Vị trí.** Mục thứ bảy trong thanh bên (`Ctrl+7`).

**Khái niệm then chốt:**

- **Preset** — một cách sắp xếp cửa sổ đã lưu.
- **Slot** — một vùng hình chữ nhật trên màn hình nơi một cửa sổ sẽ được đặt vào.
- **Snap** — lệnh sắp xếp các cửa sổ đang chạy vào các slot.

**Các vùng chính:**

- **Bên trái** — danh sách các preset đã lưu.
- **Bên phải** — một khung vẽ thể hiện các màn hình của bạn, nơi bạn đặt các slot.
- **Dưới cùng** — một bảng liên kết: slot nào ứng với tài khoản hoặc vai trò nào.

**Cách dùng.**
1. Tạo một preset bằng nút **New Preset**.
2. Đặt các slot lên khung vẽ.
3. Đặt tài khoản nào vào slot nào.
4. Nhấp **Apply** hoặc **Snap windows** — ứng dụng sắp xếp các cửa sổ CS2 đang chạy vào các vị trí đã định.

> **Lưới an toàn.** Trước khi sắp xếp, ứng dụng ghi nhớ vị trí cửa sổ hiện tại. Nút **Revert layout** khôi phục các vị trí trước đó trong vòng một phút.

![màn hình Layouts với khung vẽ màn hình](../images/layouts-screen.png)

## 4.11. Màn hình Sandboxes

**Mục đích.** Quản lý các sandbox — những môi trường cô lập nơi các máy khách Steam chạy.

**Vị trí.** Mục thứ tám trong thanh bên (`Ctrl+8`).

**Sandbox là gì.** Một sandbox là một môi trường riêng biệt, được bảo vệ cho một máy khách Steam. Các tài khoản ở các sandbox khác nhau không bao giờ chồng lấn: chúng không chia sẻ phiên, tệp hay dấu vết. Một tài khoản gắn với một sandbox.

**Khi nào dùng.** Ở đây bạn tạo các sandbox và theo dõi trạng thái của chúng. Trong hầu hết trường hợp, sandbox được gán tự động khi bạn thêm tài khoản, nên bạn hiếm khi cần chủ động vào đây.

## 4.12. Màn hình Settings

**Mục đích.** Điều chỉnh ứng dụng theo sở thích của bạn.

**Vị trí.** Mục **Settings** ở dưới cùng thanh bên (`Ctrl+,`).

**Bố cục.** Bên trái là danh sách các mục thiết lập; bên phải là chính các thiết lập. Thay đổi lưu ngay lập tức: một thông báo ngắn **Saved** xuất hiện sau mỗi lần.

**Các mục thiết lập:**

| Mục | Cấu hình gì |
|---|---|
| **General** | Khởi chạy cùng Windows, thu nhỏ xuống khay, kênh cập nhật |
| **Appearance** | Chủ đề (**System / Dark / Light**), mật độ, tỷ lệ phông, giảm chuyển động |
| **Accounts** | Hành vi khi tạo tài khoản, lưu giữ các tài khoản đã xóa |
| **Workflows** | Chính sách thử lại, giới hạn số lần chạy đồng thời |
| **Sandboxes** | Thư mục sandbox, phục hồi tự động |
| **Monitoring** | Tốc độ làm mới dữ liệu, ngưỡng cảnh báo |
| **Notifications** | Thông báo và âm thanh theo mức độ nghiêm trọng |
| **Layouts** | Bố cục mặc định, hành vi đa màn hình |
| **Hotkeys** | Phím tắt — có thể gán lại |
| **Advanced** | Mức ghi nhật ký, chẩn đoán, chọn môi trường, đặt lại về mặc định |
| **About** | Phiên bản ứng dụng, các nút mở thư mục dữ liệu và nhật ký |

> **Lưu ý.** Một số thiết lập (ví dụ, thư mục sandbox hoặc môi trường) chỉ áp dụng sau khi khởi động lại. Những thiết lập như vậy hiển thị một huy hiệu “Requires restart” bên cạnh.

![màn hình Settings](../images/settings-screen.png)

---

# 5. Các quy trình cốt lõi

Đây là phần quan trọng nhất. Nó chứa hướng dẫn từng bước đầy đủ cho các tác vụ chính. Mỗi bước mô tả bạn sẽ thấy gì và cách xác nhận thành công.

## 5.1. Thêm một tài khoản đơn lẻ

**Mục tiêu.** Thêm một tài khoản Steam mới vào ứng dụng.

**Bạn cần gì.** Tên đăng nhập và mật khẩu của tài khoản. Một mã Steam Guard nếu có.

### Bước 1 — Mở biểu mẫu thêm

Vào màn hình **Accounts** và nhấp **Add Account** trên thanh công cụ. Bạn cũng có thể nhấn `Ctrl+N`.

**Kết quả mong đợi.** Một biểu mẫu với các trường cho tài khoản mới mở ra.

### Bước 2 — Điền thông tin

Điền các trường:

- **Login** — bắt buộc, phải là duy nhất.
- **Password** — bắt buộc.
- **Steam Guard secret** — mã Steam Guard, nếu bạn có (tùy chọn).
- **Nickname** — tùy chọn; có thể được lấy tự động ở lần đăng nhập đầu tiên.
- **Tags** — thẻ tùy chọn để nhóm.
- **Sandbox binding** — chọn **Auto-assign**, một sandbox cụ thể, hoặc **None**.
- **Workflow** — kịch bản khởi chạy, nếu bạn muốn gán ngay.

**Kết quả mong đợi.** Nếu tên đăng nhập đã bị dùng, trường sẽ được tô đỏ kèm giải thích. Mật khẩu yếu được tô hổ phách — đây là cảnh báo và không ngăn việc lưu.

### Bước 3 — Lưu tài khoản

Nhấp nút lưu trong biểu mẫu.

**Kết quả mong đợi.** Biểu mẫu đóng lại và tài khoản mới xuất hiện trong bảng với trạng thái **Draft** hoặc, nếu đã gắn với một sandbox, sẵn sàng khởi chạy.

**Dấu hiệu thành công.** Tài khoản hiển thị trong bảng ở màn hình **Accounts**.

### Mẹo

- Nếu bạn bật **Validate immediately** trong biểu mẫu, ứng dụng kiểm tra tên đăng nhập ở nền và hiển thị kết quả dưới dạng một thông báo.
- Để một tài khoản có thể khởi chạy được, nó phải được gắn với một sandbox. Lựa chọn đơn giản nhất là **Auto-assign**.

### Lỗi thường gặp và cách sửa

- **“Login already in use.”** Tên đăng nhập này đã tồn tại trong ứng dụng. Kiểm tra danh sách tài khoản của bạn — có thể bạn đã thêm nó rồi.
- **Quên sandbox.** Một tài khoản không có sandbox thì không thể khởi chạy. Gắn một cái sau qua menu ngữ cảnh → **Bind sandbox**.

![biểu mẫu thêm tài khoản](../images/accounts-add-form.png)

## 5.2. Nhập một danh sách tài khoản từ tệp

**Mục tiêu.** Thêm nhanh nhiều tài khoản cùng lúc từ một tệp.

**Bạn cần gì.** Một tệp chứa danh sách tài khoản (TXT, CSV hoặc TSV). Định dạng dòng TXT đơn giản nhất là `login:password` (bạn cũng có thể dùng `login:password:steamguard:nickname`).

### Bước 1 — Khởi động trình hướng dẫn nhập

Ở màn hình **Accounts**, nhấp mũi tên cạnh nút **Import** và chọn một nguồn — ví dụ, **From file…**. Bạn cũng có thể nhấn `Ctrl+I`.

**Kết quả mong đợi.** Một trình hướng dẫn nhập từng bước mở ra.

### Bước 2 — Chọn nguồn và cách gán sandbox

Trỏ tới tệp bằng nút **Browse…**. Ở dưới cùng, chọn cách gán các sandbox:

- **Auto-assign (round-robin)** — phân bổ theo vòng (khuyến nghị);
- **Bind to specific sandbox** — gắn tất cả vào một sandbox;
- **Leave unbound** — để chúng không gắn sandbox.

Nhấp Next.

### Bước 3 — Kiểm tra dữ liệu được nhận diện thế nào

Trình hướng dẫn hiển thị các dòng đầu của tệp dưới dạng một bảng. Hãy chắc dữ liệu được tách thành các cột đúng cách. Nếu ký tự phân cách bị phát hiện sai, hãy đặt nó thủ công.

**Kết quả mong đợi.** Trong bản xem trước, tên đăng nhập và mật khẩu nằm ở các cột riêng của chúng.

### Bước 4 — Ánh xạ các trường

Kéo tiêu đề cột vào các ô cần thiết: **Login**, **Password**, **SteamGuard**, **Nickname**.

### Bước 5 — Kiểm tra các dòng có hợp lệ

Trình hướng dẫn đánh dấu mỗi dòng: ✓ hợp lệ, ⚠ cảnh báo, ✕ lỗi. Các dòng có lỗi có thể được sửa ngay tại đây hoặc bỏ qua.

**Kết quả mong đợi.** Bạn thấy sẽ thêm bao nhiêu tài khoản, bao nhiêu là trùng lặp, và bao nhiêu có lỗi.

### Bước 6 — Xác nhận nhập

Nhấp **Import N accounts**.

**Kết quả mong đợi.** Một thanh tiến trình với trạng thái theo từng dòng xuất hiện. Khi hoàn tất, các tài khoản xuất hiện trong bảng.

**Dấu hiệu thành công.** Số tài khoản trong bảng đã tăng thêm đúng bằng số đã nhập.

### Cách hủy và khôi phục

Nếu bạn hủy việc nhập khi nó đang chạy, ứng dụng đề nghị hoàn tác lô đã thêm. Xác nhận hoàn tác để trở về trạng thái ban đầu.

![trình hướng dẫn nhập, bước xác thực dòng](../images/import-wizard-validation.png)

## 5.3. Khởi chạy nhiều tài khoản

**Mục tiêu.** Khởi động vài tài khoản cùng một lúc.

**Bạn cần gì.** Các tài khoản đã được thêm và gắn với sandbox.

### Bước 1 — Chọn các tài khoản

Ở màn hình **Accounts**, tích các tài khoản bạn muốn ở cột đầu tiên. Để chọn tất cả những cái đang hiển thị, nhấn `Ctrl+A`.

**Kết quả mong đợi.** Thanh công cụ chuyển sang chế độ hàng loạt và hiển thị có bao nhiêu dòng được chọn, ví dụ `12 selected`.

### Bước 2 — Khởi động các tài khoản đã chọn

Nhấp **Start** trên thanh công cụ hàng loạt. Bạn cũng có thể nhấn `Ctrl+R`.

**Kết quả mong đợi.** Trạng thái các tài khoản đã chọn đổi thành **Starting**. Ứng dụng chuẩn bị từng tài khoản và bắt đầu khởi chạy. Việc khởi chạy diễn ra theo từng lô để máy tính không bị quá tải.

### Bước 3 — Chờ khởi chạy

Theo dõi cột trạng thái. Chờ cho tới khi các tài khoản chuyển sang trạng thái **Running**.

**Kết quả mong đợi.** Các tài khoản đã khởi chạy hiển thị **Running**, kèm một bộ đếm thời gian hoạt động bên cạnh.

**Dấu hiệu thành công.** Tất cả tài khoản đã chọn hiển thị **Running**. Số lượng đang hoạt động ở thanh trạng thái đã tăng.

### Mẹo

- Bạn không nhất thiết phải khởi chạy mọi tài khoản cùng lúc. Bắt đầu với một lô nhỏ, chắc chắn mọi thứ ổn định, rồi thêm nữa.
- Để khởi chạy một tài khoản đơn lẻ: chọn một dòng và nhấp **Start**, hoặc dùng nút **Start** ở ngăn chi tiết bên phải.

### Lỗi thường gặp và khôi phục

- **Một tài khoản ở Starting quá lâu.** Việc đăng nhập có thể chậm. Hãy chờ; nếu trạng thái đổi thành **Error**, dùng nút **Retry**.
- **Một số tài khoản không khởi động.** Sau một lần khởi chạy hàng loạt, một bản tóm tắt cho biết bao nhiêu cái thành công và thất bại. Nhấp **Filter to failed** để chỉ xử lý những cái đó.

![khởi chạy hàng loạt tài khoản, trạng thái Starting/Running](../images/accounts-bulk-start.png)

## 5.4. Dừng tất cả các tài khoản đang chạy

**Mục tiêu.** Tắt sạch sẽ tất cả các tài khoản đang hoạt động.

### Bước 1 — Chọn các tài khoản

Chọn các tài khoản đang chạy. Để chọn tất cả những cái đang hiển thị, nhấn `Ctrl+A`.

### Bước 2 — Dừng chúng

Nhấp **Stop** trên thanh công cụ hàng loạt, hoặc nhấn `Ctrl+.` (Ctrl và dấu chấm).

**Kết quả mong đợi.** Ứng dụng tắt sạch sẽ từng tài khoản. Trạng thái đổi thành **Stopped**. Nếu một tài khoản không phản hồi, sau một lúc ứng dụng đóng nó bằng cách cưỡng bức.

**Dấu hiệu thành công.** Tất cả tài khoản hiển thị **Stopped**. Số lượng đang hoạt động ở thanh trạng thái đã giảm.

### Mẹo

- **Stop** là một cách tắt nhẹ nhàng. Ứng dụng trước tiên cố đóng các máy khách một cách đúng đắn.
- Nếu một tài khoản đang trong trận, hãy hoàn tất các hành động trong game trước, rồi mới dừng nó.

## 5.5. Tạo một party và cho vào hàng chờ

**Mục tiêu.** Lập một party gồm vài tài khoản và cho chúng vào hàng chờ ghép trận cùng nhau.

**Bạn cần gì.** Vài tài khoản đang chạy (**Running**) đã đăng nhập.

### Bước 1 — Tạo một party

Vào màn hình **Matchmaking** và nhấp **Create Party**. Bạn cũng có thể nhấn `Ctrl+N`.

**Kết quả mong đợi.** Một cửa sổ mở ra nơi bạn có thể thêm tài khoản vào party và đặt tên cho nó.

### Bước 2 — Thêm thành viên và lưu

Thêm 2 đến 5 tài khoản vào party, đặt một cái tên, và lưu.

**Kết quả mong đợi.** Party mới xuất hiện trong danh sách bên trái.

### Bước 3 — Kiểm tra quorum

Chọn party và nhìn các thành viên của nó ở bên phải. Hãy chắc party đang ở trạng thái **Quorum** — tức là tất cả thành viên đã đăng nhập và sẵn sàng.

**Kết quả mong đợi.** Party hiển thị một huy hiệu **✓ Quorum**. Nếu một thành viên gặp sự cố (ví dụ, đăng nhập chậm), nó được hiển thị dưới dạng một dòng riêng.

### Bước 4 — Cho party vào hàng chờ

Nhấp **Queue** cho party đã chọn (hoặc `Ctrl+Q`). Để cho tất cả party vào hàng chờ cùng lúc, dùng **Queue All** trên thanh công cụ.

**Kết quả mong đợi.** Trước khi vào hàng chờ, ứng dụng chạy các bước kiểm tra của nó. Sau đó tất cả thành viên vào hàng chờ, với vị trí và độ trễ mạng được hiển thị.

**Dấu hiệu thành công.** Các thành viên ở trạng thái đang chờ, với một bộ đếm thời gian chờ đang chạy.

### Mẹo

- Chọn khu vực và chế độ trên thanh công cụ (ví dụ, `EU` và `Premier`) trước khi vào hàng chờ.
- Nếu party rơi vào trạng thái **Desync**, dùng hành động **Re-sync** để tạm dừng hàng chờ và chờ một trạng thái nhất quán.

![một party trong hàng chờ với vị trí các thành viên](../images/matchmaking-party-queue.png)

## 5.6. Điều gì xảy ra khi tìm được trận

**Mục tiêu.** Hiểu ứng dụng làm gì tại thời điểm tìm được một trận.

**Bạn cần gì.** Một party đang trong hàng chờ.

### Chấp nhận trận là tự động

Khi Steam tìm được một trận, một biểu ngữ **MATCH FOUND** nổi bật xuất hiện cho party. **Bạn không cần nhấp bất cứ thứ gì** — ứng dụng xác nhận sẵn sàng cho tất cả thành viên party trong khoảng thời gian được cho. Không cần hành động nào từ phía bạn.

**Kết quả mong đợi.** Các thành viên party chấp nhận trận tự động; trạng thái của họ đổi thành **✓ Accepted**.

**Dấu hiệu thành công.** Tất cả thành viên hiển thị **Accepted**, và trận bắt đầu.

> **Mẹo.** Muốn biết đã tìm được trận mà không phải nhìn màn hình? Bật một cảnh báo âm thanh cho **Match found** trong **Settings → Notifications**. Việc chấp nhận vẫn diễn ra tự động — âm thanh chỉ để giữ cho bạn được thông báo.

### Làm gì nếu party bị desync

Đôi khi một trận không thể được xác nhận cho tất cả mọi người — ví dụ, nếu một thành viên rớt khỏi hàng chờ. Party khi đó rơi vào trạng thái **Desync**. Dùng hành động **Re-sync**, và nếu cần loại thành viên gặp sự cố bằng **Drop member**, rồi cho những cái còn lại vào hàng chờ lại.

![biểu ngữ Match Found](../images/matchmaking-match-found.png)

## 5.7. Phục hồi sau sự cố treo hoặc khởi động lại ứng dụng

**Mục tiêu.** Đưa trang trại trở về trạng thái hoạt động sau khi một máy khách bị treo, hoặc sau khi ứng dụng bị đóng và mở lại.

**Bạn cần gì.** Không cần gì thêm — việc phục hồi phần lớn diễn ra tự động.

### Điều gì xảy ra tự động

- **Sau khi một máy khách treo.** Nếu Steam hoặc CS2 đóng bất ngờ, ứng dụng nhận ra, đánh dấu tài khoản với trạng thái **Crashed**, và hiển thị một thông báo có nút **Restart**. Việc phục hồi thường tự diễn ra trong vài giây.
- **Sau khi khởi động lại ứng dụng.** Khi khởi động, ứng dụng tìm các tiến trình Steam và CS2 còn sót lại từ phiên trước và đưa chúng trở lại dưới sự quản lý. Trong lúc đó, một chỉ báo **Recovering** xuất hiện ở thanh trạng thái. Các tài khoản được gắn lại được đánh dấu “Reattached” trong chốc lát.

### Làm gì thủ công

1. Mở **Dashboard** và nhìn bảng **Failures & Crashes**.
2. Với một tài khoản bị treo, nhấp **Restart** trong thông báo, trong dòng tài khoản, hoặc trong ngăn chi tiết.
3. Nếu ứng dụng báo một **Orphan process** ở trung tâm thông báo, chọn **Adopt** hoặc **Kill**.

**Dấu hiệu thành công.** Các tài khoản lại ở trạng thái **Running**, các dấu treo màu đỏ biến mất, và không có chỉ báo **Recovering** đang hoạt động ở thanh trạng thái.

### Mẹo

- Đừng khởi chạy lại mọi thứ bằng tay ngay sau một sự cố treo — hãy cho việc phục hồi tự động vài giây trước đã.
- Nếu sự cố treo tái diễn, mở **Monitoring** để xem tải: có thể bạn đang chạy nhiều tài khoản hơn mức máy tính này chịu được.

![chỉ báo Recovering ở thanh trạng thái](../images/status-recovering.png)

---

# 6. Tác vụ thường gặp («Tôi muốn…»)

Các câu trả lời ngắn cho những mục tiêu thường gặp. Để có hướng dẫn đầy đủ, theo các liên kết tới mục 5.

## «Tôi muốn thêm tài khoản mới»

- **Khi nào cần.** Bạn có các tài khoản Steam mới.
- **Làm gì.** Với một tài khoản, dùng nút **Add Account** ở màn hình **Accounts**. Với nhiều cái cùng lúc, dùng nút **Import** và trình hướng dẫn nhập.
- **Điều gì xảy ra.** Các tài khoản xuất hiện trong bảng và sẵn sàng khởi chạy (một khi chúng có sandbox).
- Thêm: [5.1](#51-thêm-một-tài-khoản-đơn-lẻ), [5.2](#52-nhập-một-danh-sách-tài-khoản-từ-tệp).

## «Tôi muốn khởi chạy Steam»

- **Khi nào cần.** Bạn cần một tài khoản đăng nhập Steam.
- **Làm gì.** Chọn tài khoản ở màn hình **Accounts** và nhấp **Start**.
- **Điều gì xảy ra.** Ứng dụng khởi chạy Steam trong sandbox của tài khoản và đăng nhập. Trạng thái chuyển **Starting → Running**.

## «Tôi muốn khởi chạy CS2»

- **Khi nào cần.** Steam đã chạy và bạn cần khởi động game.
- **Làm gì.** Khởi chạy tài khoản bằng **Start** sẽ đưa nó qua toàn bộ kịch bản, bao gồm khởi động CS2 (nếu quy trình được gán có bao gồm điều đó).
- **Điều gì xảy ra.** Sau khi đăng nhập Steam, ứng dụng khởi chạy CS2. Bạn có thể theo dõi các bước ở màn hình **Workflows**.

## «Tôi muốn tạo một sảnh»

- **Khi nào cần.** Bạn cần gom các tài khoản vào một sảnh trong game.
- **Làm gì.** Lập một party ở màn hình **Matchmaking** bằng **Create Party** và thêm thành viên.
- **Điều gì xảy ra.** Ứng dụng gộp các tài khoản đã chọn vào một party và giúp đưa chúng về một trạng thái nhất quán (quorum).
- Thêm: [5.5](#55-tạo-một-party-và-cho-vào-hàng-chờ).

## «Tôi muốn bắt đầu ghép trận»

- **Khi nào cần.** Party đã lập và sẵn sàng.
- **Làm gì.** Chọn party và nhấp **Queue** (hoặc **Queue All** cho tất cả).
- **Điều gì xảy ra.** Các thành viên vào hàng chờ; bạn thấy vị trí và thời gian chờ của họ.

## «Tôi muốn dừng tất cả các phiên đang chạy»

- **Khi nào cần.** Đã đến lúc kết thúc.
- **Làm gì.** Chọn các tài khoản (`Ctrl+A`) và nhấp **Stop**.
- **Điều gì xảy ra.** Ứng dụng đóng sạch sẽ các máy khách, và trạng thái trở thành **Stopped**.
- Thêm: [5.4](#54-dừng-tất-cả-các-tài-khoản-đang-chạy).

## «Tôi muốn phục hồi sau sự cố treo»

- **Khi nào cần.** Một máy khách bị treo hoặc ứng dụng đã khởi động lại.
- **Làm gì.** Cho việc phục hồi tự động vài giây; nếu cần, nhấp **Restart** cho tài khoản bị treo.
- **Điều gì xảy ra.** Ứng dụng đưa các tài khoản trở lại làm việc.
- Thêm: [5.7](#57-phục-hồi-sau-sự-cố-treo-hoặc-khởi-động-lại-ứng-dụng).

## «Tôi muốn sắp xếp các cửa sổ trên màn hình»

- **Khi nào cần.** Bạn muốn bố trí các cửa sổ CS2 gọn gàng trên màn hình.
- **Làm gì.** Ở màn hình **Layouts**, tạo một preset và nhấp **Apply** / **Snap windows**.
- **Điều gì xảy ra.** Các cửa sổ đang chạy di chuyển vào các vị trí đã định.

---

# 7. Tham chiếu tính năng

Phần này đề cập từng tính năng riêng lẻ cùng mục đích, vị trí và điểm đặc thù của nó.

## 7.1. Tìm kiếm tài khoản và bộ lọc

**Mục đích.** Nhanh chóng tìm các tài khoản bạn cần trong một danh sách lớn.

**Vị trí.** Thanh công cụ màn hình **Accounts**: ô tìm kiếm và nút **Filters**.

**Cách dùng.**
- Gõ vào ô tìm kiếm (`Ctrl+F`). Bạn có thể tìm theo phần: `login:alex`, `status:running`, `rank:>=gold`, `tag:prime`.
- Nhấp **Filters** (`Ctrl+K` ở màn hình này mở cửa sổ bộ lọc), đặt điều kiện theo trạng thái, hạng, sandbox, quy trình hoặc thẻ, và lưu bộ đó thành một preset.

**Hành vi mong đợi.** Bảng lập tức chỉ hiển thị các tài khoản khớp. Các bộ lọc đang hoạt động xuất hiện thành một hàng chip bên dưới thanh công cụ.

**Mẹo.** Lưu các bộ điều kiện thường dùng thành preset — chúng có sẵn từ menu thả xuống trên thanh công cụ.

## 7.2. Nhóm và thiết lập cột

**Mục đích.** Sắp xếp bảng cho phù hợp với công việc của bạn.

**Vị trí.** Thanh công cụ màn hình **Accounts**: các nút **Density**, **Columns** và **Group**.

**Cách dùng.**
- **Group** cho phép bạn nhóm các tài khoản theo trạng thái, quy trình, sandbox, thẻ hoặc hạng. Các nhóm hiển thị bộ đếm, ví dụ `Running (24)`.
- **Columns** — bộ các cột hiển thị. Có sẵn các bộ dựng sẵn: **Operational**, **Identity**, **Audit**, **Compact**. Bạn có thể lưu bộ của riêng mình.
- **Density** — chiều cao dòng (gọn hơn hoặc thoáng hơn).

## 7.3. Menu ngữ cảnh của tài khoản

**Mục đích.** Truy cập nhanh mọi hành động cho một tài khoản.

**Vị trí.** Nhấp chuột phải vào một dòng tài khoản.

**Có gì.** Chỉnh sửa, sao chép tên đăng nhập hoặc Steam ID, khởi động/dừng/khởi động lại, gắn và gỡ gắn sandbox, gán quy trình, xác thực lại (**Re-auth**), dò đăng nhập (**Probe login now**), làm việc với thẻ, xuất, nhân bản và xóa.

## 7.4. Thao tác hàng loạt

**Mục đích.** Thực hiện một hành động lên nhiều tài khoản cùng lúc.

**Vị trí.** Thanh công cụ màn hình **Accounts** ở chế độ lựa chọn (khi có ít nhất một dòng được tích).

**Cách dùng.** Tích các tài khoản, rồi nhấp nút bạn cần: **Start**, **Stop**, **Restart**, **Bind sandbox**, **Workflow…**, **Tag…**, **Export**, hoặc **Delete**.

**Hành vi mong đợi.** Một cửa sổ xuất hiện với chế độ xem tiến trình theo từng tài khoản. Bạn có thể hủy thao tác khi nó đang chạy.

**Giới hạn.** Khi xóa từ năm tài khoản trở lên, ứng dụng yêu cầu bạn xác nhận bằng cách gõ từ `DELETE`.

## 7.5. Xuất tài khoản

**Mục đích.** Lưu dữ liệu tài khoản vào một tệp.

**Vị trí.** Nút **Export** trên thanh công cụ hoặc trong menu ngữ cảnh.

**Cách dùng.** Chọn một định dạng: **TXT** (login:password), **CSV** (tất cả các trường), hoặc **JSON** (bản ghi đầy đủ).

> **Cảnh báo.** Xuất mật khẩu đòi hỏi sự đồng ý riêng — ứng dụng yêu cầu bạn đánh dấu vào một hộp kiểm. Hãy xử lý các tệp như vậy một cách cẩn thận.

## 7.6. Nhân bản một tài khoản

**Mục đích.** Nhanh chóng tạo một bản sao của một tài khoản làm điểm khởi đầu.

**Vị trí.** Menu ngữ cảnh của dòng → **Clone…**.

**Hành vi mong đợi.** Một biểu mẫu mở ra với các trường đã điền sẵn (tên đăng nhập trở thành `original_copy`), ngoại trừ mã Steam Guard và liên kết sandbox — bạn đặt lại chúng.

## 7.7. Workflow: khởi động, tạm dừng, dừng

**Mục đích.** Quản lý các kịch bản tự động.

**Vị trí.** Màn hình **Workflows**.

**Cách dùng.**

| Hành động | Làm gì | Hỏi xác nhận? |
|---|---|---|
| **Start** | Chạy kịch bản cho các tài khoản đã chọn | Khi khởi chạy hơn 10 tài khoản |
| **Pause** | Tạm dừng nhẹ nhàng sau bước hiện tại | Không |
| **Resume** | Tiếp tục từ điểm hiện tại | Không |
| **Stop** | Kết thúc kịch bản kèm dọn dẹp | Có |
| **Restart** | Dừng và bắt đầu lại từ đầu | Có (với thao tác hàng loạt) |
| **Skip step** | Đánh dấu bước hiện tại đã xong và đi tiếp | Có |
| **Retry now** | Thử lại bước hiện tại ngay lập tức | Không |

**Mẹo.** Tab **State Machine** trong ngăn chi tiết cho thấy rõ một kịch bản đang ở bước nào.

## 7.8. Gắn với một sandbox

**Mục đích.** Dành riêng một môi trường cô lập cho một tài khoản, mà không có nó thì tài khoản không thể khởi chạy.

**Vị trí.** Menu ngữ cảnh → **Bind sandbox…**, hoặc thao tác hàng loạt **Bind sandbox**.

**Cách dùng.** Chọn một phương thức: round-robin, lấp những cái trống trước, hoặc một sandbox cụ thể.

**Giới hạn.** Một tài khoản, một sandbox. Nếu sandbox được chọn đã đang được dùng, ứng dụng đề nghị giải phóng nó khỏi tài khoản trước đó.

## 7.9. Bố cục cửa sổ

**Mục đích.** Sắp xếp các cửa sổ CS2 bằng một bố cục dựng sẵn.

**Vị trí.** Màn hình **Layouts**.

**Cách dùng.** Tạo một preset, đặt các slot lên khung vẽ màn hình, đặt các liên kết, và nhấp **Apply**.

**Mẹo.** Nút **Revert layout** khôi phục các vị trí cửa sổ trước đó trong vòng một phút, phòng khi một bố cục không ưng ý.

## 7.10. Trung tâm thông báo

**Mục đích.** Một nơi duy nhất cho tất cả các thông báo của ứng dụng.

**Vị trí.** Huy hiệu thông báo ở thanh trên cùng, hoặc `Ctrl+Shift+N`.

**Cách dùng.** Bảng mở ra ở bên phải. Chuyển giữa các tab **All**, **Errors**, **Warnings** và **Info**. Với mỗi mục, bạn có thể đi tới nguồn, thử lại, hoặc bỏ qua. Nút **Clear all** làm trống danh sách.

**Giới hạn.** 200 mục gần nhất được giữ lại; các mục cũ hơn bị loại bỏ.

---

# 8. Trạng thái và chỉ báo

Mỗi trạng thái có một màu, một ký hiệu và một nhãn. Dưới đây là ý nghĩa của từng cái và liệu bạn có cần hành động.

| Trạng thái | Ký hiệu | Ý nghĩa | Cần hành động |
|---|---|---|---|
| **OK / Success** | ✓ (xanh lá) | Tài khoản trực tuyến, đăng nhập thành công | Không |
| **Running** | ▶ (xanh dương) | Tài khoản hoặc quy trình đang chạy | Không |
| **Starting** | ◐ (tím) | Đang khởi chạy, một trạng thái chuyển tiếp | Chờ nó hoàn tất |
| **Queued** | ⏱ (xám) | Đang chờ trong hàng chờ | Không |
| **Stopped** | ■ (xám) | Đã dừng, nhàn rỗi | Tùy chọn — bạn có thể khởi động nó |
| **Paused** | ⏸ (hổ phách) | Kịch bản bị tạm dừng | Nhấp **Resume** để tiếp tục |
| **Warning** | △ (hổ phách) | Một bất thường không nghiêm trọng | Kiểm tra chi tiết; thường bạn có thể tiếp tục |
| **Error** | ✕ (đỏ) | Một sự cố có thể phục hồi | Nhấp **Retry** hoặc điều tra nguyên nhân |
| **Crashed** | ☠ (đỏ sẫm, nhấp nháy) | Tiến trình thoát bất ngờ | Nhấp **Restart** |
| **Match Found** | ◎ (xanh lá, nhấp nháy) | Đã tìm được một trận CS2 | Không gì cả — ứng dụng tự xác nhận sẵn sàng |
| **Desync** | ⛓ (cam) | Các thành viên party không đồng bộ | Chạy **Re-sync** |
| **Info** | ⓘ (xanh dương) | Một thông báo trung tính | Không |

**Chỉ báo bổ sung:**

- **Recovering** — một chỉ báo màu xanh dương ở thanh trạng thái trong lúc ứng dụng khởi động: các tiến trình từ phiên trước đang được đưa trở lại dưới sự quản lý. Chờ nó hoàn tất.
- **Reattached** — một dấu tạm thời trên dòng tài khoản: tiến trình đã được tiếp quản thành công sau khi khởi động lại.
- **Frozen at HH:mm:ss** — ở màn hình **Monitoring**, nghĩa là hiển thị dữ liệu đang bị đóng băng (không ở chế độ **Live**). Để đưa dữ liệu trực tiếp trở lại, chuyển sang **Live** hoặc tắt **Freeze**.

**Cách xem chi tiết.** Rê chuột lên một ký hiệu trạng thái để có một chú giải: trạng thái đã kéo dài từ khi nào, tài khoản đang ở bước nào, và sự kiện gần nhất là gì.

![ví dụ về các trạng thái trong bảng tài khoản](../images/status-badges.png)

---

# 9. Thông báo

Ứng dụng báo cáo sự kiện theo ba cách: **toast** (bật lên ở góc rồi biến mất), **thanh trạng thái** (một bản tóm tắt cố định ở dưới cùng), và **biểu ngữ nội tuyến** (gắn với một màn hình cụ thể).

## Toast

Chúng xuất hiện ở góc dưới bên phải.

| Thông báo | Vì sao xuất hiện | Ý nghĩa | Làm gì | Có thể bỏ qua |
|---|---|---|---|---|
| **Saved** | Bạn đã đổi một thiết lập | Thay đổi đã được lưu | Không gì | Có, tự biến mất |
| Thao tác thành công (xanh lá) | Một hành động hoàn tất thành công | Mọi thứ ổn | Không gì | Có, biến mất sau ~5 giây |
| Cảnh báo (hổ phách) | Một bất thường không nghiêm trọng được nhận ra | Đáng xem qua | Tùy chọn xem chi tiết | Thường là có, biến mất sau ~10 giây |
| Lỗi (đỏ) | Một thao tác thất bại | Cần hành động | Nhấp **View** hoặc **Retry** | Không, còn cho tới khi bị đóng |
| Treo | Một máy khách đóng bất ngờ | Một tài khoản đã treo | Nhấp **Restart** hoặc mở dump | Không, còn cho tới khi được xác nhận |

**Cần biết.**
- Rê chuột lên một thông báo sẽ dừng bộ đếm tự đóng — bạn có thể đọc nó thong thả.
- Các thông báo giống nhau gộp thành một kèm bộ đếm, ví dụ `… failed (×4)`.

## Thanh trạng thái

Ở phía bên phải thanh trạng thái, thông báo chưa đọc quan trọng nhất được hiển thị, ví dụ `● 3 errors`. Nhấp vào sẽ mở trung tâm thông báo.

## Biểu ngữ nội tuyến

Chúng xuất hiện ở phía trên một màn hình và áp dụng cho toàn bộ màn hình đó. Ví dụ: `⚠ Steam network degraded — 12 accounts retrying login`. Một biểu ngữ có thể được đóng bằng nút **Dismiss** nếu nó không chặn. Các biểu ngữ chặn (ví dụ, khi một dịch vụ không khả dụng) còn cho tới khi vấn đề được giải quyết.

## Cảnh báo âm thanh

Âm thanh tắt theo mặc định. Bạn có thể bật nó cho các sự kiện cụ thể (ví dụ, **Match found** hoặc **Crash**) trong **Settings → Notifications**. Một âm thanh cho **Match found** rất tiện để biết đã tìm được trận mà không phải nhìn màn hình — việc chấp nhận trận thì tự diễn ra.

![một toast lỗi với các nút View và Retry](../images/notification-error-toast.png)

---

# 10. Lỗi và khắc phục sự cố

Lỗi khi vận hành một trang trại là chuyện thường, và ứng dụng giúp bạn giải quyết chúng. Dưới đây là các tình huống thường gặp theo định dạng “Vấn đề → Nguyên nhân có thể → Giải pháp → Kết quả mong đợi”.

## Không thể kích hoạt bản quyền

**Vấn đề.** Khi nhập khóa, ứng dụng không cho bạn tiếp tục.

| Thông báo | Nguyên nhân có thể | Giải pháp |
|---|---|---|
| “License key invalid” | Khóa được nhập bị gõ sai | Kiểm tra chính tả. Dán khóa bằng **Paste from clipboard** thì dễ hơn |
| “Used on max devices” | Bản quyền đã được dùng trên số thiết bị tối đa | Giải phóng bản quyền trên một thiết bị khác, rồi thử lại. Nút **Manage devices** dẫn tới quản lý thiết bị |
| “Cannot reach license server” | Không có kết nối tới máy chủ bản quyền | Kiểm tra kết nối internet của bạn và nhấp **Retry** |

**Kết quả mong đợi.** Với một khóa đúng và kết nối tới máy chủ, cửa sổ kích hoạt đóng lại và **Dashboard** mở ra.

## Một tài khoản không chịu khởi chạy

**Vấn đề.** Bạn đã nhấp **Start**, nhưng tài khoản không chuyển sang **Running**.

- **Nguyên nhân có thể.** Tài khoản không được gắn với một sandbox.
  **Giải pháp.** Mở menu ngữ cảnh của tài khoản → **Bind sandbox…** và gán một sandbox.
- **Nguyên nhân có thể.** Cần xác thực lại (thông tin đăng nhập đã cũ); một dấu “Reauth required” nằm cạnh dòng.
  **Giải pháp.** Menu ngữ cảnh → **Re-auth (Steam Guard)**.
- **Nguyên nhân có thể.** Steam tạm thời giới hạn tần suất đăng nhập.
  **Giải pháp.** Chờ khoảng một phút và nhấp **Retry**.

**Kết quả mong đợi.** Trạng thái chuyển **Starting → Running**.

## Steam ở Waiting/Starting quá lâu

**Vấn đề.** Tài khoản kẹt ở giai đoạn đăng nhập.

- **Nguyên nhân có thể.** Đăng nhập chậm hoặc vấn đề mạng Steam tạm thời.
  **Giải pháp.** Cho nó một chút thời gian. Nếu một trạng thái **Error** xuất hiện, nhấp **Retry**. Nếu mạng Steam không ổn định, một biểu ngữ cảnh báo xuất hiện ở trên — chờ cho tới khi nó phục hồi.

**Kết quả mong đợi.** Tài khoản đăng nhập và chuyển sang **Running**.

## Một máy khách bị treo

**Vấn đề.** Tài khoản nhận trạng thái **Crashed**.

- **Nguyên nhân có thể.** Máy khách CS2 hoặc Steam thoát bất ngờ.
  **Giải pháp.** Trong thông báo xuất hiện, nhấp **Restart**. Việc phục hồi thường đã đang diễn ra tự động. Chi tiết sự cố treo có ở màn hình **Monitoring** trong luồng **Crashes & Warnings**.

**Kết quả mong đợi.** Tài khoản khởi động lại và trở về **Running**.

## Một party rơi vào Desync

**Vấn đề.** Party ở trạng thái **Desync** — các thành viên ở trạng thái không nhất quán.

- **Nguyên nhân có thể.** Một thành viên chấp nhận trận còn một thành viên khác không kịp, hoặc ai đó rớt khỏi hàng chờ.
  **Giải pháp.** Nhấp **Re-sync** để tạm dừng hàng chờ và chờ sự nhất quán. Nếu một tài khoản gây rắc rối, loại nó bằng **Drop member** và cho những cái còn lại vào hàng chờ lại.

**Kết quả mong đợi.** Party trở về trạng thái **Quorum** và sẵn sàng vào hàng chờ lại.

## Một lần khởi chạy hàng loạt kết thúc với lỗi

**Vấn đề.** Sau một lần **Start** hàng loạt, một số tài khoản không khởi chạy.

- **Giải pháp.** Trong bản tóm tắt, nhấp **Filter to failed** — bảng chỉ hiển thị các tài khoản gặp sự cố. Giải quyết từng cái theo các nguyên nhân ở trên và khởi chạy lại.

**Kết quả mong đợi.** Sau khi các nguyên nhân được giải quyết, một lần **Start** lặp lại đưa các tài khoản sang **Running**.

## Dữ liệu của một màn hình không chịu tải

**Vấn đề.** Thay vì nội dung của màn hình, có một biểu ngữ hoặc một thông báo rằng một dịch vụ không khả dụng.

- **Nguyên nhân có thể.** Một dịch vụ nền tạm thời không khả dụng.
  **Giải pháp.** Nhấp **Retry**. Nếu không giúp được, nhấp **Open logs** để xem chi tiết, hoặc khởi động lại ứng dụng.

**Kết quả mong đợi.** Màn hình tải và hiển thị dữ liệu hiện tại.

## Ứng dụng báo một Orphan process

**Vấn đề.** Ở trung tâm thông báo, một thông báo như “Orphan process … — Adopt or Kill?”.

- **Nguyên nhân có thể.** Một tiến trình từ phiên trước còn sót lại mà không thể tự gắn với một tài khoản.
  **Giải pháp.** Chọn **Adopt** (đưa vào quản lý) nếu tiến trình cần thiết, hoặc **Kill** (kết thúc) nếu không.

**Kết quả mong đợi.** Danh sách tiến trình được sắp xếp gọn gàng.

## Máy tính chậm và sự cố treo tăng lên

**Vấn đề.** Bất ổn định nói chung, sự cố thường xuyên.

- **Nguyên nhân có thể.** Nhiều tài khoản đang chạy hơn mức máy tính chịu được.
  **Giải pháp.** Mở **Monitoring** và nhìn **CPU** và **RAM**. Nếu các giá trị gần đến giới hạn, dừng bớt vài tài khoản bằng **Stop**.

**Kết quả mong đợi.** Tải giảm và hoạt động ổn định lại.

> **Mã lỗi.** Chi tiết lỗi bao gồm một mã ngắn như `[E-1042]`. Bạn có thể sao chép nó và dùng khi liên hệ hỗ trợ. Một tham chiếu đầy đủ các mã có sẵn qua **Help → Error reference**.

![một màn hình lỗi ví dụ với các nút Retry / Open logs](../images/error-screen.png)

---

# 11. Thực hành tốt nhất

## Chuẩn bị tài khoản

- Thêm tài khoản dưới dạng một danh sách qua **Import** — nhanh hơn và ít gõ sai hơn.
- Để việc gán sandbox ở **Auto-assign** trừ khi bạn cần một liên kết cụ thể.
- Dùng **Tags** để nhóm các tài khoản và lọc chúng nhanh.

## Khởi chạy nhiều tài khoản

- Khởi chạy theo lô: bắt đầu với một nhóm nhỏ, xác nhận độ ổn định, rồi thêm nữa.
- Giữ **Dashboard** hoặc **Monitoring** mở để theo dõi tải theo thời gian thực.
- Nhắm tới mức khuyến nghị 4–10 tài khoản CS2 cùng lúc; bạn có thể chạy nhiều hơn trên một PC mạnh và ít hơn trên các máy yếu.

## Làm việc với các bố cục

- Chuẩn bị trước vài preset cho các tình huống khác nhau (ví dụ, “4-stack”, “single focused”).
- Sau khi một bố cục bị hỏng, dùng **Revert layout** ngay, trong khi cửa sổ hoàn tác một phút còn hiệu lực.

## Dừng an toàn

- Dừng các tài khoản bằng nút **Stop** (một cách tắt nhẹ nhàng) thay vì đóng cửa sổ bằng tay.
- Trước khi thoát ứng dụng, hãy dừng các tài khoản đang hoạt động. Nếu bạn cố đóng ứng dụng khi các kịch bản đang chạy, nó cảnh báo bạn.

## Tránh gián đoạn

- Trước khi vào hàng chờ, hãy chắc party ở trạng thái **Quorum**.
- Theo dõi các biểu ngữ về trạng thái mạng Steam — khi nó không ổn định, tốt hơn là chờ.

## Duy trì hoạt động ổn định

- Kiểm tra **Dashboard** thường xuyên — nó cho thấy trạng thái tổng thể trong vài giây.
- Giữ số tài khoản chạy đồng thời trong khả năng của máy tính bạn.
- Hãy để việc phục hồi tự động chạy vài giây trước khi bạn tự can thiệp.

---

# 12. Câu hỏi thường gặp

**Vì sao tôi không thể khởi chạy một tài khoản?**
Nhiều khả năng tài khoản không được gắn với một sandbox — không có nó thì không thể khởi chạy. Gắn một cái qua menu ngữ cảnh → **Bind sandbox…**. Một lần khởi chạy cũng có thể bị chặn bởi nhu cầu xác thực lại (một dấu “Reauth required”) — trong trường hợp đó hãy chạy **Re-auth**.

**Vì sao Steam ở trạng thái chờ lâu như vậy?**
Đây thường là đăng nhập chậm hoặc độ trễ mạng Steam tạm thời. Cho nó một chút thời gian. Nếu một trạng thái **Error** xuất hiện, nhấp **Retry**.

**Làm sao tôi khởi động lại một quy trình?**
Chọn các tài khoản hoặc instance bạn cần và nhấp **Restart** (hoặc `Ctrl+Shift+R`). Với một thao tác hàng loạt, ứng dụng hỏi xác nhận.

**Điều gì xảy ra nếu ứng dụng đóng?**
Các tài khoản và thiết lập của bạn được lưu. Ở lần khởi chạy tiếp theo, ứng dụng cố đưa các tiến trình của phiên trước trở lại quản lý — một chỉ báo **Recovering** xuất hiện ở thanh trạng thái. Nếu các kịch bản đang hoạt động khi đóng, ứng dụng cảnh báo bạn trước.

**Làm sao tôi biết mọi thứ đang hoạt động?**
Kiểm tra thanh trạng thái ở dưới cùng và **Dashboard**. Dấu hiệu hoạt động bình thường: các tài khoản ở trạng thái **Running**, không có dấu đỏ ở thẻ **Errors** hoặc bảng **Failures & Crashes**, và tải **CPU** và **RAM** trong phạm vi bình thường.

**Mật khẩu của tôi được lưu ở đâu?**
Chỉ trên máy tính của bạn. Chúng được mã hóa bằng cơ chế bảo vệ tích hợp của Windows, không bao giờ được lưu dưới dạng văn bản thuần, và không bao giờ được gửi đi đâu.

**FarmPanel có chơi thay tôi không?**
Không. Nó không phải bot hay công cụ auto-farm. Ứng dụng quản lý việc khởi chạy, giám sát, lập sảnh và phục hồi, còn mọi hành động trong game đều do bạn thực hiện.

**Tôi có phải nhập khóa bản quyền mỗi lần không?**
Không. Khóa được nhập một lần, trong lần kích hoạt đầu tiên. Sau đó ứng dụng mở thẳng vào **Dashboard**.

**Làm sao tôi tìm nhanh một hành động nếu quên nút nằm ở đâu?**
Nhấn `Ctrl+K` để mở bảng lệnh. Bắt đầu gõ tên một hành động, màn hình, hoặc tên đăng nhập tài khoản, và chọn cái bạn cần từ danh sách.

**Tôi có thể chuyển monitoring sang màn hình thứ hai không?**
Được. Ở màn hình **Monitoring**, nhấp nút tách — màn hình mở ra dưới dạng một cửa sổ riêng mà bạn có thể đặt lên màn hình thứ hai. Vị trí của nó được ghi nhớ.

**Làm sao tôi đặt lại các thiết lập về mặc định?**
Trong **Settings → Advanced** có **Reset to defaults**. Để bảo vệ khỏi các cú nhấp vô ý, ứng dụng yêu cầu bạn xác nhận bằng cách gõ văn bản.

---

*Kết thúc Hướng dẫn sử dụng FarmPanel.*

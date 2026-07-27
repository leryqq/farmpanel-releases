# Cài đặt Sandboxie-Plus

**Hướng dẫn cài đặt từng bước cho Windows**

Phiên bản tài liệu: 1.0 · Phiên bản Sandboxie-Plus: **1.17.5**

🌐 [English](INSTALL-SANDBOXIE-PLUS.md) · [Русский](INSTALL-SANDBOXIE-PLUS.ru.md) · [Español](INSTALL-SANDBOXIE-PLUS.es.md) · [Português](INSTALL-SANDBOXIE-PLUS.pt.md) · [Français](INSTALL-SANDBOXIE-PLUS.fr.md) · [Türkçe](INSTALL-SANDBOXIE-PLUS.tr.md) · [Bahasa Indonesia](INSTALL-SANDBOXIE-PLUS.id.md) · **Tiếng Việt** · [हिन्दी](INSTALL-SANDBOXIE-PLUS.hi.md) · [中文](INSTALL-SANDBOXIE-PLUS.zh.md) · [العربية](INSTALL-SANDBOXIE-PLUS.ar.md)

---

FarmPanel giữ mỗi tài khoản trong **sandbox** riêng của nó — một môi trường cô lập nơi Steam và CS2 không lẫn với các tài khoản khác. Việc cô lập này do một chương trình miễn phí tên là **Sandboxie-Plus** đảm nhận. Bạn cài nó một lần, trước khi bắt đầu khởi chạy tài khoản trong FarmPanel.

Hướng dẫn này đưa bạn qua quá trình cài đặt từng bước. Không có gì phức tạp — chỉ mất vài phút.

> **Tóm tắt.** Tải trình cài đặt **Sandboxie-Plus 1.17.5** → chạy nó → chấp nhận các thiết lập mặc định → cho phép cài đặt (cần quyền quản trị) → xong.

> **Quan trọng.** Khác với chính FarmPanel, Sandboxie-Plus **cần quyền quản trị** để cài đặt — điều này là bình thường, vì chương trình tích hợp sâu vào Windows để cô lập các ứng dụng một cách đáng tin cậy.

## Mục lục

1. [Những thứ bạn cần](#những-thứ-bạn-cần)
2. [Bước 1. Tải trình cài đặt](#bước-1-tải-trình-cài-đặt)
3. [Bước 2. Chạy quá trình cài đặt](#bước-2-chạy-quá-trình-cài-đặt)
4. [Bước 3. Đi qua trình hướng dẫn cài đặt](#bước-3-đi-qua-trình-hướng-dẫn-cài-đặt)
5. [Bước 4. Lần chạy đầu tiên của Sandboxie-Plus](#bước-4-lần-chạy-đầu-tiên-của-sandboxie-plus)
6. [Bước 5. Kiểm tra mọi thứ hoạt động](#bước-5-kiểm-tra-mọi-thứ-hoạt-động)
7. [Bước 6. Kết nối với FarmPanel](#bước-6-kết-nối-với-farmpanel)
8. [Cách gỡ cài đặt Sandboxie-Plus](#cách-gỡ-cài-đặt-sandboxie-plus)
9. [Khắc phục sự cố](#khắc-phục-sự-cố)
10. [Câu hỏi thường gặp](#câu-hỏi-thường-gặp)

---

# Những thứ bạn cần

- **Một máy tính chạy Windows 10 hoặc 11** (64-bit).
- **Quyền quản trị** trên máy tính này (một hộp thoại xuất hiện khi cài đặt — bạn cần nhấp **Có**).
- **Kết nối internet** — để tải chương trình.
- **Khoảng 5 phút của bạn.**

> Sandboxie-Plus miễn phí. Một số tính năng bổ sung dành cho người ủng hộ dự án, nhưng bạn **không cần** chúng để làm việc với FarmPanel — bản miễn phí thông thường là đủ.

---

# Bước 1. Tải trình cài đặt

1. Mở trang chính thức của phiên bản bạn cần:
   **[Sandboxie-Plus 1.17.5 trên GitHub](https://github.com/sandboxie-plus/Sandboxie/releases/tag/v1.17.5)**
2. Cuộn xuống mục **Assets**.
3. Tìm và tải tệp có tên kiểu như **`Sandboxie-Plus-x64-v1.17.5.exe`** — đây là trình cài đặt cho Windows 64-bit thông thường.

**Cách chọn đúng tệp:**

| Tệp | Dành cho ai |
|---|---|
| **`Sandboxie-Plus-x64-v1.17.5.exe`** | **Đa số người dùng** — Windows thông thường trên CPU Intel hoặc AMD. Tải tệp này. |
| `Sandboxie-Plus-arm64-v1.17.5.exe` | Chỉ dành cho máy tính chạy CPU ARM (hiếm). |
| `Sandboxie-Classic-…` | Biến thể giao diện cũ. **Không cần** cho FarmPanel — hãy chọn **Plus**. |
| Tệp `.7z` | Bản portable dành cho người dùng nâng cao. **Không cần** để cài đặt. |

**Điều gì xảy ra tiếp theo.** Tệp xuất hiện trong thư mục **Tải xuống** (Downloads) của bạn.

> **Mẹo.** Chỉ tải trình cài đặt từ trang GitHub chính thức được liên kết ở trên. Như vậy bạn nhận được phiên bản chính hãng, đã được xác minh.

![trang phát hành 1.17.5 với mục Assets](../images/sandboxie/github-release-assets.png)

---

# Bước 2. Chạy quá trình cài đặt

1. Mở thư mục **Tải xuống** và nhấp đúp vào tệp **`Sandboxie-Plus-x64-v1.17.5.exe`** đã tải.
2. Windows hiển thị hộp thoại **“Bạn có muốn cho phép ứng dụng này thay đổi thiết bị của bạn không?”** — nhấp **Có**. Đây là hộp thoại quyền quản trị; không có nó, Sandboxie-Plus không thể cài đặt.

> **Nếu cửa sổ SmartScreen màu xanh xuất hiện** (“Windows đã bảo vệ PC của bạn”) — nhấp **Thông tin thêm**, rồi **Vẫn chạy**. Đây là cảnh báo thông thường cho chương trình đã tải, không phải lỗi.

**Điều gì xảy ra tiếp theo.** Cửa sổ trình hướng dẫn cài đặt mở ra.

---

# Bước 3. Đi qua trình hướng dẫn cài đặt

Trình hướng dẫn cài đặt đưa bạn qua vài màn hình đơn giản. Trong hầu hết trường hợp, bạn chỉ cần để mọi thứ ở giá trị mặc định và nhấp **Next**.

1. **Chọn ngôn ngữ.** Nếu cửa sổ chọn ngôn ngữ xuất hiện, chọn Tiếng Việt (hoặc ngôn ngữ của bạn) rồi nhấp **OK**.
2. **Thỏa thuận cấp phép.** Đọc rồi nhấp **I Agree** hoặc **Next**.
3. **Thư mục cài đặt.** Giữ thư mục mặc định (`C:\Program Files\Sandboxie-Plus`) rồi nhấp **Next**. Không cần thay đổi.
4. **Tùy chọn cài đặt.** Không cần thay đổi gì — chỉ cần nhấp **Next** / **Install**.
5. Đợi cho xong. Việc cài đặt mất chưa đến một phút.
6. Ở màn hình cuối, nhấp **Finish**. Giữ ô “khởi chạy Sandboxie-Plus” được chọn, nếu có.

**Điều gì xảy ra tiếp theo.** Sandboxie-Plus được cài đặt, và biểu tượng của nó xuất hiện trên màn hình nền và trong menu Start. Chương trình thường mở ngay sau khi cài đặt.

> **Có cần khởi động lại không?** Thường là không. Nhưng nếu trình hướng dẫn yêu cầu khởi động lại máy tính, hãy làm vậy để việc cô lập hoạt động đúng.

![màn hình trình hướng dẫn cài đặt với thư mục mặc định](../images/sandboxie/installer-wizard.png)

---

# Bước 4. Lần chạy đầu tiên của Sandboxie-Plus

Lần đầu bạn mở Sandboxie-Plus, nó hiển thị một **Setup Wizard** (trình hướng dẫn thiết lập). Hãy đi qua từng bước — chỉ cần lặp lại những gì mô tả dưới đây.

Nếu cửa sổ **chọn ngôn ngữ giao diện** xuất hiện trước trình hướng dẫn, hãy chọn ngôn ngữ của bạn rồi nhấp **OK**.

Sau đó trình hướng dẫn đưa bạn qua vài màn hình.

### Màn hình 1 — Introduction

Chọn **“Personally, for private non-commercial use”** (Cá nhân, dùng riêng phi thương mại) rồi nhấp **Next**.

![Setup Wizard — màn hình Introduction với “Personally, for private non-commercial use” được chọn](../images/sandboxie/wizard-1-introduction.png)

### Màn hình 2 — Support certificate

Để trống ô này rồi nhấp **Next**. Không cần chứng chỉ để làm việc với FarmPanel.

![Setup Wizard — màn hình Support certificate với ô để trống](../images/sandboxie/wizard-2-support-certificate.png)

### Màn hình 3 — Configure UI

Giữ các giá trị ở **mặc định** (**Advanced UI for experts** đã được chọn) rồi nhấp **Next**.

![Setup Wizard — màn hình cấu hình giao diện với các giá trị mặc định](../images/sandboxie/wizard-3-ui-configuration.png)

### Màn hình 4 — Shell integration

**Bỏ chọn tất cả các ô** rồi nhấp **Next**.

![Setup Wizard — màn hình Shell integration với tất cả các ô đã bỏ chọn](../images/sandboxie/wizard-4-shell-integration.png)

### Màn hình 5 — Updater

**Bỏ chọn tất cả các ô** rồi nhấp **Next**.

![Setup Wizard — màn hình Updater với tất cả các ô đã bỏ chọn](../images/sandboxie/wizard-5-updater.png)

### Màn hình 6 — Complete

Nhấp **Finish** để áp dụng thiết lập và đóng trình hướng dẫn.

![Setup Wizard — màn hình cuối với nút Finish](../images/sandboxie/wizard-6-complete.png)

> **Mẹo.** Nếu phân vân ở màn hình nào, hãy bỏ chọn các ô và nhấp **Next**. FarmPanel không cần các tích hợp bổ sung hay lời nhắc cập nhật.

**Điều gì xảy ra tiếp theo.** Cửa sổ chính của Sandboxie-Plus mở ra — danh sách sandbox và bảng điều khiển.

![cửa sổ chính của Sandboxie-Plus sau lần chạy đầu tiên](../images/sandboxie/main-window.png)

---

# Bước 5. Kiểm tra mọi thứ hoạt động

Hãy chắc chắn Sandboxie-Plus được cài đặt đúng:

1. Mở Sandboxie-Plus (biểu tượng trên màn hình nền hoặc trong menu Start).
2. Cửa sổ chính hiển thị một danh sách sandbox — thường có một sandbox mặc định tên kiểu như **DefaultBox**.
3. Chương trình mở ra và không hiển thị thông báo lỗi.

Nếu tất cả những điều này đều có — **Sandboxie-Plus đã được cài đặt và sẵn sàng sử dụng**.

---

# Bước 6. Kết nối với FarmPanel

Khi Sandboxie-Plus đã được cài đặt, FarmPanel có thể dùng nó để cô lập các tài khoản.

1. Mở **FarmPanel**.
2. Vào **Settings → Sandboxes**.
3. Chắc chắn đường dẫn thư mục sandbox đã được đặt. Nếu ô trống, hãy chọn một thư mục cho sandbox; nếu đã điền sẵn thì không cần thay đổi gì.
4. Quay lại màn hình **Accounts**. Bây giờ, khi thêm tài khoản, bạn có thể chọn cách gán sandbox (**Auto-assign** và các cách khác), và các tài khoản có thể được khởi chạy.

> **Cách nó kết nối.** Trong FarmPanel, mỗi tài khoản phải được gắn với một sandbox, nếu không sẽ không khởi chạy được. Chính Sandboxie-Plus tạo và duy trì các môi trường cô lập này “ở hậu trường”. Để biết thêm về sandbox và việc khởi chạy tài khoản, xem [Hướng dẫn sử dụng FarmPanel](../user-guide/USER-GUIDE.vi.md).

**Dấu hiệu thành công.** Một tài khoản trong FarmPanel khởi chạy và chuyển sang trạng thái **Running** — điều này có nghĩa việc cô lập qua Sandboxie-Plus đang hoạt động.

---

# Cách gỡ cài đặt Sandboxie-Plus

Nếu bạn cần gỡ chương trình:

1. Trước tiên, đóng tất cả chương trình đang chạy trong sandbox (trong FarmPanel, dừng các tài khoản bằng **Stop**).
2. Mở **Cài đặt Windows** → **Ứng dụng** → **Ứng dụng đã cài đặt**
   (hoặc “Control Panel” → “Programs and Features”).
3. Tìm **Sandboxie-Plus** trong danh sách.
4. Nhấp **Uninstall** và xác nhận. Việc gỡ cài đặt cũng cần quyền quản trị.

> **Lưu ý.** Sau khi Sandboxie-Plus bị gỡ, FarmPanel không thể khởi chạy tài khoản cho đến khi chương trình được cài lại.

---

# Khắc phục sự cố

## Windows không cho cài — không có quyền quản trị

**Nguyên nhân.** Sandboxie-Plus bắt buộc phải có quyền quản trị.

**Giải pháp.** Đăng nhập bằng tài khoản có quyền quản trị, hoặc nhờ quản trị viên máy tính cài chương trình. Khi hộp thoại **“Cho phép thay đổi?”** xuất hiện, nhấp **Có**.

## Cửa sổ SmartScreen xuất hiện

**Nguyên nhân.** Windows cảnh báo về các chương trình mới tải gần đây. Đó không phải lỗi.

**Giải pháp.** Nhấp **Thông tin thêm**, rồi **Vẫn chạy**.

## Phần mềm diệt virus chặn trình cài đặt

**Nguyên nhân.** Một số phần mềm diệt virus thận trọng với phần mềm tích hợp vào hệ thống.

**Giải pháp.**
1. Chắc chắn bạn đã tải tệp từ trang GitHub chính thức (liên kết ở [Bước 1](#bước-1-tải-trình-cài-đặt)).
2. Nếu cần, tạm thời thêm tệp vào danh sách ngoại lệ của phần mềm diệt virus và tải lại.

## Tải nhầm tệp

**Nguyên nhân.** Trang phát hành có nhiều tệp.

**Giải pháp.** Với Windows thông thường, bạn cần tệp tên **`Sandboxie-Plus-x64-v1.17.5.exe`**. Đừng lấy các biến thể **arm64**, **Classic** hay **.7z**. Quay lại [Bước 1](#bước-1-tải-trình-cài-đặt) và tải đúng tệp.

## FarmPanel không khởi chạy tài khoản sau khi cài đặt

**Giải pháp.**
1. Chắc chắn Sandboxie-Plus đã được cài và mở được (xem [Bước 5](#bước-5-kiểm-tra-mọi-thứ-hoạt-động)).
2. Trong FarmPanel, mở **Settings → Sandboxes** và kiểm tra đường dẫn thư mục sandbox đã được đặt.
3. Khởi động lại FarmPanel.
4. Nếu sự cố vẫn còn, hãy liên hệ hỗ trợ (xem [Câu hỏi thường gặp](#câu-hỏi-thường-gặp)).

## Máy tính yêu cầu khởi động lại sau khi cài đặt

**Giải pháp.** Khởi động lại máy tính — việc này hoàn tất cài đặt và bật tính năng cô lập. Sau khi khởi động lại, mở FarmPanel lần nữa.

---

# Câu hỏi thường gặp

**Cài Sandboxie-Plus có bắt buộc không?**
Có, nếu bạn muốn khởi chạy tài khoản trong FarmPanel. Chính Sandboxie-Plus cung cấp sự cô lập cho mỗi tài khoản trong một môi trường riêng.

**Sandboxie-Plus có tính phí không?**
Không, bản cơ bản miễn phí và đủ để làm việc với FarmPanel. Các tính năng bổ sung dành cho người ủng hộ dự án, nhưng không bắt buộc.

**Vì sao việc cài đặt cần quyền quản trị còn FarmPanel thì không?**
Sandboxie-Plus tích hợp sâu vào Windows để cô lập chương trình một cách đáng tin cậy, nên nó cần quyền quản trị. FarmPanel thì chỉ cài cho tài khoản người dùng của bạn và không cần quyền đó.

**Tôi có cần tự cấu hình các sandbox không?**
Không. Chỉ cần cài Sandboxie-Plus. FarmPanel tạo và cấu hình sandbox cho các tài khoản một cách tự động.

**Tôi có cần chứng chỉ ủng hộ (supporter certificate) không?**
Không. Bạn có thể bỏ qua màn hình đó ở lần chạy đầu tiên. Nó không cần cho FarmPanel.

**Tôi nên cài chính xác phiên bản nào?**
Phiên bản **1.17.5** — liên kết ở [Bước 1](#bước-1-tải-trình-cài-đặt). Hãy cài đúng phiên bản này để tương thích ổn định với FarmPanel.

**Tôi nên liên hệ ở đâu nếu có gì đó không hoạt động?**
Liên hệ hỗ trợ FarmPanel trên Telegram: [t.me/farmpanel_vn](https://t.me/farmpanel_vn). Mô tả vấn đề và kèm theo nội dung thông báo lỗi nếu có.

---

Sau khi cài Sandboxie-Plus, hãy quay lại [hướng dẫn cài đặt FarmPanel](../install-guide/INSTALL-GUIDE.vi.md) hoặc đi thẳng đến [Hướng dẫn sử dụng](../user-guide/USER-GUIDE.vi.md) để thêm tài khoản và khởi chạy farm đầu tiên của bạn.

*Kết thúc hướng dẫn cài đặt Sandboxie-Plus.*

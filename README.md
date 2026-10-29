# HoangAnh Auto Farm · v3.12.0 — Máy tính

Tool dành cho **Chrome hoặc Microsoft Edge trên máy tính Windows / MacBook**. Hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

**[⬇ BẤM VÀO ĐÂY ĐỂ TẢI TOOL CHO MÁY TÍNH](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.12.0/hoanganh-autofarm-resource-v3.12.0.zip)**

Đây là tiện ích trình duyệt. Bạn không cần cài Node.js, chạy lệnh hay tìm tệp `.exe`.

## 1. Tải và giải nén

1. Bấm nút tải ở trên. Tệp nhận được có tên `hoanganh-autofarm-resource-v3.12.0.zip`.
2. Mở thư mục **Downloads / Tải xuống** trên máy tính.
3. **Windows:** nhấp chuột phải vào tệp ZIP → **Extract All… / Giải nén tất cả…** → **Extract / Giải nén**. Nếu chưa thấy mục này, chọn **Show more options / Hiển thị thêm tùy chọn**.
4. **MacBook:** nhấp đúp vào tệp ZIP để giải nén bằng Finder.
5. Đặt thư mục đã giải nén ở nơi dễ tìm và giữ lâu dài, ví dụ `Documents/HoangAnh-AutoFarm`. Đừng xóa hoặc chuyển thư mục này sau khi cài.
6. Mở thư mục đó. Bạn cần nhìn thấy tệp **`manifest.json`**, cùng các tệp như `autofarm.js`, `popup.html` và thư mục `icons`.

**Nếu mở ra chỉ thấy thêm một thư mục, hãy mở tiếp vào trong cho đến khi thấy `manifest.json`.** Nếu máy ẩn đuôi tệp, tên có thể chỉ hiện là `manifest`.

```text
HoangAnh-AutoFarm/        ← Chọn thư mục này khi cài
├── manifest.json
├── autofarm.js
├── popup.html
└── icons/
```

## 2. Nạp tool vào Chrome hoặc Edge

1. Mở đúng trình duyệt bạn sẽ dùng để chơi game.
2. Bấm vào **thanh địa chỉ ở trên cùng**, xóa địa chỉ cũ rồi dán một trong hai dòng sau và nhấn Enter:
   - Chrome: `chrome://extensions`
   - Microsoft Edge: `edge://extensions`
3. Bật **Developer mode / Chế độ dành cho nhà phát triển**. Chrome thường đặt ở góc trên bên phải; Edge có thể đặt trong thanh bên.
4. Bấm **Load unpacked / Tải tiện ích đã giải nén**.
5. Trong cửa sổ chọn thư mục, tìm và chọn **thư mục chứa trực tiếp `manifest.json`** ở bước 1, rồi bấm **Select Folder / Chọn thư mục**. Bạn chọn cả thư mục, không chọn riêng tệp JSON và không chọn tệp ZIP.
6. Cài thành công khi trang tiện ích xuất hiện ô **hoanganh Auto Farm · Resource Pilot**, phiên bản **3.12.0**, với công tắc bật.

> Không thấy nút Load unpacked? Kiểm tra đã bật Developer mode chưa. MacBook cũng làm tương tự bằng Chrome hoặc Edge; hướng dẫn này không dùng cho Safari.

## 3. Mở game và bắt đầu farm

1. Trong **chính trình duyệt vừa cài tool**, mở [PokéSurvivor](https://pokesurvivor.com/) hoặc [Doofcraft](https://pokesurvivor.doofcraft.com/), rồi đăng nhập game.
2. Nếu game đã mở trước khi cài, bấm nút **tải lại trang ↻** cạnh thanh địa chỉ.
3. Khi tool nạp thành công, bạn sẽ thấy bảng **RESOURCE PILOT** nổi trên trang game. Nếu bảng bị thu gọn, bấm dấu **+** trên bảng.
4. Chọn Pokémon muốn chơi trong game. Trong tab **Build** của tool, chọn đúng Pokémon, nhập **4 chiêu khác nhau** rồi bấm **Lưu và áp dụng cấu hình**. Core được lưu riêng cho từng Pokémon. Nếu cần TM, hãy trang bị trong game trước.
5. Vào tab **Farm**, chọn mục tiêu:
   - **Farm:** ưu tiên tài nguyên. Nhập số vàng / lượt gacha cần kiếm **thêm**. Ví dụ vàng `10000`, gacha `10`; mục không cần đặt thì để `0` hoặc để trống.
   - **Sinh tồn:** ưu tiên sống và tăng sức mạnh; không dừng theo mục tiêu tài nguyên.
6. Muốn tool tự vào lượt mới sau khi kết thúc, bật **Tự chơi lại qua menu Solo**. Trong **Ngưỡng và giới hạn**, đặt giới hạn phút/lượt theo ý bạn; `0` là không giới hạn tương ứng.
7. Bấm **Lưu và áp dụng cấu hình**, sau đó bấm **Bắt đầu** trong bảng tool. Bạn có thể bắt đầu ở menu Solo hoặc khi đã vào trận.
8. Kiểm tra trạng thái chuyển sang **ĐANG FARM**. Nút **Tạm dừng** tạm ngưng điều khiển; nút **Dừng** kết thúc phiên điều khiển.

**Để vừa làm việc vừa farm:** có thể dùng nút **Tách game sang cửa sổ riêng** và bật **Giữ màn hình và máy thức khi đang farm**. Giữ cửa sổ game còn hiển thị; khi tab bị ẩn/thu nhỏ, trình duyệt có thể ngừng vẽ game. Tool không chạy khi máy đã tắt hoặc ngủ.

## 4. Auto Roll theo gen

1. Bấm **Dừng** phiên farm, rồi mở **Gacha** trong game.
2. Trong bảng tool, chọn tab **Auto Roll** → **Đọc danh sách gen**.
3. Chọn gen/khu vực muốn roll và nhập số lượt tối đa, ví dụ `20`.
4. Bấm **Bắt đầu roll**. Tool dừng khi đủ giới hạn hoặc không còn nút roll bằng vé phù hợp khả dụng. Bấm **Dừng roll** để ngừng sớm.

Giới hạn tính theo số Pokémon nhận được: hai gói ×10 là 20 lượt. Bản gốc dùng gói ×10 nên phần dư dưới 10 không được roll; Doofcraft có thể roll đơn. Tool không tự mua vé, dùng đá quý, vé rainbow hoặc Wish. Nếu bạn dừng lúc một lượt đã gửi đi, game vẫn có thể xử lý lượt đó.

## 5. Cập nhật khi đã cài bản cũ

**Để giữ cấu hình, hãy dùng lại đúng thư mục tiện ích đang cài:**

1. Bấm **Dừng** trong tool và đóng tab game.
2. Tải ZIP mới từ nút tải ở đầu trang, giải nén ra một thư mục tạm.
3. Mở thư mục mới đến khi thấy `manifest.json`. Sao chép **toàn bộ nội dung trong thư mục này** vào **thư mục tiện ích cũ**.
4. Khi máy hỏi có thay thế tệp trùng tên không, chọn **Replace / Thay thế**. Sau khi chép, `manifest.json` vẫn phải nằm trực tiếp trong thư mục cũ, không bị lồng thêm một thư mục mới.
5. Mở `chrome://extensions` hoặc `edge://extensions`. Tại ô **hoanganh Auto Farm**, bấm nút **Reload / Tải lại** có biểu tượng mũi tên vòng tròn.
6. Mở lại game hoặc tải lại trang. Kiểm tra phiên bản trên bảng tool.

Không cần bấm **Remove / Xóa** tiện ích để cập nhật. Nếu nạp từ một thư mục mới, trình duyệt có thể coi là tiện ích khác và cấu hình cũ không tự chuyển. Chỉ bật một bản tool để tránh hai bản cùng điều khiển.

## 6. Lỗi thường gặp

| Bạn gặp gì? | Cách xử lý |
| --- | --- |
| “Không thể tải tệp kê khai / Manifest missing” | Bạn có thể chọn sai thư mục hoặc chưa giải nén. Mở thư mục và tìm `manifest.json`, rồi Load unpacked đúng thư mục chứa tệp đó. |
| ZIP đã tải nhưng không biết mở tệp nào để cài | Giải nén rồi làm bước 2. Không mở riêng `autofarm.js` hay `manifest.json` để cài. |
| Không thấy bảng RESOURCE PILOT trong game | Kiểm tra tiện ích đang bật, mở game trong đúng trình duyệt/hồ sơ đã cài, rồi tải lại trang game. Nếu trình duyệt hỏi quyền truy cập trang game, cho phép trên website game. |
| Vẫn hiện bản cũ sau cập nhật | Kiểm tra đã thay tệp trong đúng thư mục cũ, bấm Reload tiện ích rồi tải lại trang game. Tắt các bản tool trùng. |
| Không tự chơi lượt tiếp theo | Kiểm tra Tự chơi lại, giới hạn phút/lượt, mục tiêu đã đủ hay chưa và dòng trạng thái của tool. |
| Tạm dừng hoặc đứng yên | Đọc dòng trạng thái và tab Nhật ký. Kiểm tra game có hộp thoại đang chờ chọn, kết nối bị ngắt hoặc tab game bị ẩn hay không. |
| Cần gửi thông tin để được hỗ trợ | Chụp toàn bộ bảng tool có phiên bản, dòng trạng thái và màn hình game; cho biết bạn dùng Chrome/Edge và bản game nào. |

## Hỗ trợ và Donate

[Liên hệ Facebook của Hoàng Anh](https://www.facebook.com/NguyenHoangAnh.Support).

Muốn ủng hộ phát triển tool, mở tab **Donate** trong bảng tool để xem QR. Sự ủng hộ của bạn là động lực để mình tiếp tục cải thiện tool. Cảm ơn bạn!

Tool đang thử nghiệm. Các kiểm thử mô phỏng không bảo đảm thắng mọi boss hoặc treo liên tục trong mọi điều kiện.

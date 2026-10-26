# hoanganh Auto Farm · v2.8.0

Auto farm và tự chọn nâng cấp cho [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/). Tự nhận bản game theo website đang mở.

- **Máy tính:** [⬇ Tải ZIP v2.8.0](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v2.8.0/hoanganh-autofarm-resource-v2.8.0.zip)
- **Android:** [⬇ Tải gói Mobile v2.8.0](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v2.8.0/hoanganh-autofarm-mobile-v2.8.0.zip)

## Cài trên máy tính

1. Tải và giải nén ZIP máy tính.
2. Mở `chrome://extensions` (Edge: `edge://extensions`), bật **Developer mode**.
3. Chọn **Load unpacked**, chọn thư mục có `manifest.json`.
4. Tắt/gỡ bản cũ, tải lại toàn bộ tab game, đăng nhập và vào trận.
5. Bấm **Bắt đầu** trong bảng nổi hoặc nhấn **F8**. Giữ tab game ở phía trước.

Bản 2.8.0 cần quyền chạy trên cả hai website. Nếu cập nhật extension đang cài, mở trang quản lý tiện ích và nhấn **Reload** trước khi tải lại game.

## Android

Tải ZIP Mobile, giải nén và nhập `hoanganh-autofarm-mobile.user.js` vào trình quản lý userscript hỗ trợ chạy trong trang, ví dụ Tampermonkey trên Firefox Android. Bật script cho cả hai website, tắt script phiên bản cũ rồi tải lại game. Xem `README-ANDROID.md` trong gói. Mobile đang thử nghiệm; nên giữ màn hình ngang.

## Chức năng

- Hồ sơ farm vàng/tài nguyên, vé gacha/boss và sinh tồn.
- Theo cổng boss, né vùng báo chiêu/đạn, đánh boss và thu phần thưởng quan sát được. Cổng mặc định có ưu tiên cao trong hai hồ sơ farm tài nguyên; có thể chọn theo ngưỡng HP/cấp hoặc tắt theo cổng.
- Giữ vị trí cạnh rương khóa đến khi mở; phân biệt rương thưởng nhặt trực tiếp ở Doofcraft.
- Doofcraft: đọc địa hình tường/nước từ canvas và tìm đường vòng qua tường đang nhìn thấy.
- Tự chọn nâng cấp, item và Bond; reroll bằng lượt có sẵn, chọn dự phòng khi hết lượt.
- Bộ chiêu tham khảo từ snapshot SurvivorTiers không TM. Dữ liệu này chưa được benchmark riêng cho cân bằng Doofcraft.
- Dùng orb theo tình huống ở bản gốc. Doofcraft hiện không có hotkey orb tương ứng nên tùy chọn này tự tắt theo khả năng của game.

**Phím tắt:** F8 bật/tạm dừng · F9 đường đi · F6 nhận diện. Tự bấm WASD, rời cửa sổ hoặc chuyển tab sẽ tạm dừng. Tự chơi lại mặc định tắt; nếu game về menu chọn trận nhiều bước, hãy vào trận rồi tiếp tục.

## Phạm vi kiểm tra

Đã kiểm tra logic, trình duyệt mô phỏng và các lệnh vẽ công khai của cả hai game: sprite/shiny, tọa độ canvas phóng theo mật độ điểm ảnh, cổng, loot, rương, vùng báo chiêu, tia chéo và đạn. Với Doofcraft đã kiểm tra thêm khóa hộp lựa chọn và địa hình map. Chưa chạy trận Doofcraft với tài khoản đăng nhập, chưa đo tỷ lệ thắng boss hoặc vàng/vé mỗi giờ; mobile chưa kiểm tra trên thiết bị thật.

Xem `TESTING.md`, `SOURCES.md`, `PRIVACY.md` và `THIRD_PARTY_NOTICES.txt` trong ZIP.

Cần hỗ trợ: liên hệ [Facebook Nguyen Hoang Anh Support](https://www.facebook.com/NguyenHoangAnh.Support).

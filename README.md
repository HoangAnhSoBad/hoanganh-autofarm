# hoanganh Auto Farm · v3.9.0

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.0/hoanganh-autofarm-resource-v3.9.0.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.0/hoanganh-autofarm-mobile-v3.9.0.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.0/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.9.0

- Chỉ dùng 4 chiêu core tự chọn, lưu riêng cho từng Pokémon. Bỏ build tham khảo, lựa chọn đánh xa/cận chiến và so sánh build TM.
- Giữ core tự chọn đã lưu từ bản trước; nạp lại khi mở tool lần sau. Pokémon Shadow và dạng thường được lưu riêng theo định danh.
- Ưu tiên cao nhất cho học, nâng cấp và tiến hóa chiêu thuộc core khi xuất hiện. Ưu tiên ghép 4 core thành Bond chính; giữ dùng Bond chính sau khi hoàn thành.
- Không tự dùng build tham khảo nếu chưa lưu core. Khi không có thẻ core, vẫn xử lý lựa chọn dự phòng/reroll theo cấu hình để tránh kẹt.
- Giữ các cải tiến Z-Move, chọn chiêu mạnh, di chuyển và auto farm từ bản trước.

## Cách dùng
1. Mở tab Build trong bảng tool ở game.
2. Chọn đúng Pokémon rồi nhập 4 tên chiêu khác nhau từ danh sách gợi ý.
3. Bấm **Lưu và áp dụng cấu hình**. Đổi Pokémon sẽ nạp core đã lưu của Pokémon đó.
4. Nếu cần TM, trang bị trong game trước. Dừng phiên trước khi thay core hoặc Pokémon.

Core lưu trên thiết bị/trình duyệt hiện tại; Android lưu riêng từng website. Giữ cùng ID tiện ích và dữ liệu trình duyệt khi cập nhật để giữ cấu hình.

Kiểm tra: toàn bộ bộ kiểm thử logic; giao diện lưu/tải lại trên cả hai website, hai Pokémon có core riêng, kiểm tra trùng chiêu và loại bỏ lựa chọn tham khảo; bootstrap mobile. Chưa kiểm chứng phiên chơi thật hoặc điện thoại thật.

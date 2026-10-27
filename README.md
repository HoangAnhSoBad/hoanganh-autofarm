# hoanganh Auto Farm · v3.8.0

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.0/hoanganh-autofarm-resource-v3.8.0.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.0/hoanganh-autofarm-mobile-v3.8.0.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.0/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# hoanganh Auto Farm v3.8.0

- Hộ tống: tính khoảng cách theo kích thước Pokémon dẫn đường và theo dõi NPC; đi vượt vòng xanh để NPC phía sau vào vùng cứu hộ. Chỉ chờ khi thấy NPC trong vùng; không tự nhận nhiệm vụ đã hoàn thành.
- Chọn chiêu trước Bond: xét cấp chiêu đã xác nhận, tầm đánh, dữ liệu sát thương/hồi chiêu tham khảo và mật độ quái. Cho phép tia tụ lực như Hyper Beam ở khoảng cách an toàn; tăng ưu tiên chiêu diện rộng khi quái áp sát. Giữ các chặn an toàn và ưu tiên Bond chính đã hoàn tất.
- Phá vòng vây: tìm hướng ít nguy hiểm với đường không xuyên vật cản, giữ hướng ngắn hạn để giảm đảo hướng. Né vùng đánh boss vẫn ưu tiên hơn phá vây; không bảo đảm thoát mọi vòng quái.
- Treo farm: thêm nút Tách game sang cửa sổ riêng, bảo vệ tab đang chạy khỏi tự discard, giữ thức theo tùy chọn. Khôi phục trạng thái discard trước đó khi dừng/tạm dừng hoặc mất heartbeat.

## Sử dụng khi làm công việc khác
Trong Farm, bật Giữ màn hình và máy thức, Lưu cấu hình, bấm Tách game sang cửa sổ riêng rồi Bắt đầu. Để cửa sổ game còn hiển thị bên cạnh cửa sổ làm việc; không thu nhỏ hoặc che kín. Tool vẫn dựa trên hình game: tab bị ẩn/ngừng vẽ sẽ không có dữ liệu mới. Không hỗ trợ bảo đảm farm khi máy ngủ, gập nắp hoặc trình duyệt đóng. Android cần tab game ở phía trước.

## Core tự chọn từ v3.7
Trong Build chọn Pokémon, bật Dùng 4 chiêu core tự chọn, nhập 4 chiêu khác nhau và Lưu cấu hình. Lưu riêng từng Pokémon; dừng phiên trước khi đổi core. TM cho bộ tự chọn cần trang bị trong game trước.

## Kiểm chứng và giới hạn
Đã chạy bộ kiểm tra hồi quy, mô phỏng hộ tống 3 kích thước, vòng vây và chọn chiêu, kiểm tra giao diện trên Chrome. Số liệu sức mạnh chỉ là ước tính từ catalog đã thu thập, không phải DPS trực tiếp theo toàn bộ buff của nhân vật. Chưa xác minh phiên farm qua đêm và thiết bị Android thật.

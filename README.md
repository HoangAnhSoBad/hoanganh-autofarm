# hoanganh Auto Farm · v3.9.1

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.1/hoanganh-autofarm-resource-v3.9.1.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.1/hoanganh-autofarm-mobile-v3.9.1.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.9.1/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.9.1

## Chọn và giữ Bond
- Lưu cấp chiêu đã đọc theo tên chiêu, giữ thông tin khi chuyển ô/ghép Bond. Không tự đoán cấp cao khi chưa đọc được.
- Bond tầm xa an toàn vẫn có thể được chọn trong lúc di chuyển hoặc né; giữ chặn khi chờ game, vào cổng, bị Choice Band khóa, ô không rõ hoặc chỉ gồm buff/chiêu không tới địch.
- Bond chính đủ 4 core vẫn được ưu tiên cao nhất.

## Địa hình và di chuyển
- Đọc địa hình Doofcraft theo ô 8 pixel thay vì 16 pixel để nhận diện vách mỏng chính xác hơn; gộp các ô liền nhau để giảm số vật cản cần xử lý.
- Nhớ tường tĩnh có biên dạng rõ tối đa 12 giây khi khuất, có giới hạn khoảng cách và số lượng; đặt lại khi đổi arena/dịch chuyển lớn.
- Loại hướng đi xuyên vật cản rắn ngay cả khi áp lực quái cao. Khi đã chạm biên, vẫn cho phép hướng đi ra khỏi vật cản.
- Đường vòng có thêm khoảng đệm và ưu tiên khoảng trống để hạn chế bám sát góc tường.

## Kiểm tra và cập nhật
Đã qua bộ hồi quy, renderer HUD Doofcraft với bố cục Hyper Beam / Hail / Bond Hex + Hyper Beam, giữ Bond sau xác nhận, vách 8 pixel, che khuất tường 3 giây và mô phỏng đường vòng quanh vật cản/góc chữ U. Kiểm tra bằng fixture Chrome; chưa đo hiệu quả farm trong trận thật hoặc bảo đảm không bao giờ kẹt.

Máy tính: thay tệp trong thư mục tiện ích cũ, Reload tiện ích rồi tải lại game. Android: nhập userscript mới và tải lại game. Giữ cấu hình 4 core đã lưu của v3.9.0.

Core: vào Build → chọn Pokémon → nhập 4 chiêu → Lưu và áp dụng cấu hình. Core lưu riêng từng Pokémon trên thiết bị; không dùng build tham khảo.

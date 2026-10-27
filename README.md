# hoanganh Auto Farm · v3.8.1

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.1/hoanganh-autofarm-resource-v3.8.1.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.1/hoanganh-autofarm-mobile-v3.8.1.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.1/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.8.1

## Sửa chọn chiêu Solar Beam / Hyper Beam
- Sửa trường hợp giữ Hyper Beam cấp 2 khi Solar Beam đã cấp 4: cho phép chuyển sang chiêu tụ lực cùng loại có cấp cao hơn dù quái ở gần, nếu đang dùng chiêu tụ lực. Không tự đổi từ chiêu an toàn sang tụ lực khi quái áp sát.
- Giảm độ ưu tiên giữ ô đang dùng khi chiêu cùng nhóm cao hơn ít nhất 2 cấp; vẫn tôn trọng chặn né nguy hiểm, HP thấp, Choice Band và Bond chính.
- Cập nhật số liệu nâng cấp Doofcraft theo dữ liệu công khai ngày 28/10/2026, phân biệt từng cấp thay vì dùng số cơ bản cho mọi cấp.
- Cho thử chọn lại sau khi thấy cấp chiêu mới nếu lần chuyển trước không được game xác nhận. Hiển thị tên/cấp và ô đang dùng đọc từ HUD trong tab Build.

## Sửa Pokémon Shadow / sự kiện
- Bổ sung sprite và định danh nội bộ cho 8 Pokémon Shadow cùng Bloodmoon Ursaluna từ catalog Doofcraft hiện tại.
- Phân biệt số Dex quốc gia và mã nội bộ: Shadow Mewtwo #150 · ID 10901; Shadow Lugia #249 · ID 10902.
- Khi Pokémon sự kiện cùng loài đang được chọn trong game, giữ đúng biến thể thay vì đổi về bản thường. TM và 4 chiêu core lưu riêng theo mã nội bộ.
- Sửa nhận diện dự phòng khi danh sách tên HUD rỗng nhưng vẫn đọc được tên từ chữ trong game.
- Giữ build Shadow đã có từ nguồn tham khảo. Biến thể mới chưa có build riêng được ghi rõ là tham khảo từ dạng gốc, không coi là meta đã kiểm chứng.

## Cập nhật
Máy tính: thay nội dung thư mục tiện ích đang dùng bằng ZIP mới, bấm Reload ở chrome://extensions hoặc edge://extensions rồi tải lại game. Tắt các bản cũ nếu cài thành tiện ích mới.
Android: nhập userscript v3.8.1 vào Tampermonkey rồi tải lại game.
Trong Build có thể để tự nhận diện hoặc chọn đúng tên Shadow; tên hiển thị kèm ID để phân biệt với bản thường.

Đã kiểm tra hồi quy, Solar4/Hyper2 ở cả hai bản game, nhận diện HUD ở 1x/2x, chọn đúng Shadow từ menu, kho TM tách biệt, sprite Shadow và điều khiển chuyển sang Solar Beam. Kiểm tra gameplay bằng mô phỏng Chrome; chưa xác minh trận thực tế trên tài khoản của bạn.

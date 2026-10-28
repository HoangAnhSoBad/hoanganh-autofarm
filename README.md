# hoanganh Auto Farm · v3.8.2

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.2/hoanganh-autofarm-resource-v3.8.2.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.2/hoanganh-autofarm-mobile-v3.8.2.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.8.2/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.8.2

## Chọn chiêu mạnh hơn
- Nhận diện riêng cấp chiêu, trạng thái tiến hóa (viền vàng) và ô đang dùng (tên chiêu phía trên).
- Sửa đọc biểu tượng Doofcraft khi game làm tròn kích thước theo pixel ở các mức phóng như 125%.
- Cho phép chuyển từ Hyper Beam cấp thấp sang Solar Beam cấp cao/tiến hóa cùng kiểu đánh, kể cả khi đang chạy tới Rift, rút lui hoặc giữ vị trí. Vẫn không tự chuyển sang chiêu lao người hay đưa chiêu tụ lực mới vào khi quái áp sát.
- Không khóa thử đổi chiêu vĩnh viễn sau hai lần game chưa xác nhận: chờ 15 giây rồi thử lại có giới hạn. Giữ Bond chính đủ 4 core và không đổi khi Choice Band khóa chiêu.

## Z-Move trên Doofcraft
- Nhận diện 18 loại Z-Crystal trong HUD và thẻ nâng cấp; phân biệt trạng thái sẵn sàng và hồi chiêu.
- Thêm tùy chọn “Dùng Z-Move khi gặp boss / đông quái” trong Farm, bật mặc định.
- Dùng phím F khi boss ở trong tầm, quái tụ đông hoặc cần phá vây. Kiểm tra HUD sau thao tác; không spam phím trong thời gian hồi hoặc khi chưa nhận diện chắc chắn.
- Ngừng sử dụng khi ô Z-Move biến mất. Chưa bật tính năng này cho bản gốc khi chưa xác minh cơ chế tương ứng.

## Cập nhật
Máy tính: tải ZIP máy tính, giải nén vào thư mục tiện ích đang dùng, bấm Reload ở chrome://extensions hoặc edge://extensions rồi tải lại game. Tắt bản cũ nếu cài thành tiện ích mới.
Android: nhập userscript mới vào Tampermonkey rồi tải lại game; cần giữ màn hình và tab game mở.

Kiểm tra: bộ hồi quy, điều khiển chọn chiêu/Z-Move, renderer HUD và bộ nhận phím hiện tại của Doofcraft, 18 crystal, giao diện cảm ứng và mức phóng 100%/125%/200%. Đây là kiểm tra bằng fixture trên Chrome, chưa xác minh trận thực tế trên tài khoản của bạn hoặc điện thoại thật.

Các sửa lỗi Shadow/biến thể sự kiện, core riêng từng Pokémon, mục tiêu tài nguyên và cửa sổ farm riêng từ bản trước được giữ lại. Khi treo farm, giữ cửa sổ game hiển thị; trình duyệt/hệ điều hành vẫn có thể hạn chế tab bị ẩn hoặc máy ngủ.

# hoanganh Auto Farm · v3.11.1

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.1/hoanganh-autofarm-resource-v3.11.1.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.1/hoanganh-autofarm-mobile-v3.11.1.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.11.1/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.11.1

## Sinh tồn: tăng sức mạnh qua Rift và rương
- Bỏ quy tắc cấm toàn bộ Rift và rương trong Sinh tồn.
- Khi core đã lưu chưa Bond đủ 4 chiêu, ưu tiên Rift đủ điều kiện hơn XP/vàng rơi lẻ. Không yêu cầu phải có Bond mới được vào cổng đầu tiên.
- Đánh giá chiêu sát thương thực sự đọc được trên HUD, HP, cấp hiện tại, nguy hiểm trên đường và thời gian còn lại của cổng. Chiêu buff đơn không được coi là đủ sức đánh boss.
- Mặc định: khi có chiêu sát thương cấp 3+ hoặc Bond có sát thương, cần ít nhất 75% HP và cấp 12; khi chỉ có chiêu sát thương cấp thấp, cần 90% HP và cấp 16. Ngưỡng HP/cấp đánh boss do bạn đặt cao hơn vẫn được tôn trọng. Đây là ngưỡng ước lượng, không bảo đảm thắng boss.
- Có hồi máu an toàn ở gần và HP dưới 85% thì hồi trước; gặp nguy hiểm mới thì đánh giá lại cả cổng đang theo.
- Khi đủ Bond 4 core, Rift vẫn là cơ hội tăng sức mạnh nhưng không còn được ưu tiên tuyệt đối trước XP/rương/boss.
- Mở rương khóa khi đủ HP, đường đi an toàn và không có quái/boss ở gần nơi cần đứng mở. Rương đang mở từ 65% được hoàn tất trước khi đổi sang cổng nếu vẫn an toàn. Nguy hiểm xuất hiện thì ngừng mở để né.
- Tính đường vòng qua địa hình khi xét hạn cổng; không coi đường tìm được một phần là đã có đường tới cổng. Giới hạn và lưu tạm kiểm tra địa hình để tránh tìm đường lại liên tục.
- Giữ lựa chọn tắt theo Rift/mở rương, core đã lưu và các quy tắc Bond, né boss, Revive của bản trước. Farm giữ chính sách riêng.

## Tải và cập nhật
- Máy tính: tải ZIP resource trong Assets, giải nén và thay tệp trong thư mục tiện ích cũ, Reload tại chrome://extensions hoặc edge://extensions, rồi tải lại game.
- Android: nhập hoanganh-autofarm-mobile.user.js mới vào Tampermonkey, tắt bản trùng và tải lại game.
- Trong Farm, chọn mục tiêu Sinh tồn; bật Theo cổng Rift và Mở rương khóa. Trong Build, lưu đúng 4 chiêu core cho Pokémon đang chơi.

Đã kiểm thử logic và mô phỏng Chrome trên cả hai tên miền: core chưa/đã Bond, HP/chiêu không đủ, hồi máu trước, hoàn tất/ngắt mở rương, đường vòng, hạn cổng và đường bị kín. Chưa đo tỷ lệ sống hay thắng boss bằng trận thực tế; Android chưa kiểm tra trên điện thoại thật.

# hoanganh Auto Farm · v3.10.0

Bot hỗ trợ [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/).

- [Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.10.0/hoanganh-autofarm-resource-v3.10.0.zip)
- [Tải ZIP Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.10.0/hoanganh-autofarm-mobile-v3.10.0.zip)
- [Tải userscript Android](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.10.0/hoanganh-autofarm-mobile.user.js)

Máy tính: giải nén, mở chrome://extensions (Edge: edge://extensions), bật Developer mode, chọn Load unpacked và chọn thư mục chứa manifest.json. Tắt bản cũ để tránh hai tool cùng điều khiển; tải lại game. Nếu cập nhật cùng thư mục, bấm Reload tiện ích. Cấu hình có thể không chuyển nếu trình duyệt cấp ID tiện ích mới.

Android: dùng Firefox và Tampermonkey, nhập hoanganh-autofarm-mobile.user.js qua Utilities → Import, xác nhận nhập, bật script rồi tải lại game. Bản thử nghiệm, cần giữ màn hình và tab game mở.

[Hỗ trợ qua Facebook](https://www.facebook.com/NguyenHoangAnh.Support)

# HoangAnh Auto Farm v3.10.0

## Hai mục tiêu
- **Farm**: ưu tiên tài nguyên, tăng trọng số loại còn thiếu trong mục tiêu; giữ rương/boss/Rift theo thiết lập. Cấu hình Vàng hoặc Vé cũ chuyển về Farm, giữ số tài nguyên đã đặt.
- **Sinh tồn**: ưu tiên XP, hồi phục và chiến đấu an toàn; bỏ đuổi tiền/vé, rương khóa và nhiệm vụ phụ. Không chủ động vào Rift. Khi gặp boss đã nhận diện, đủ HP/cấp/chiêu thì chủ động giữ cự ly đánh; né vùng báo chiêu và vật cản vẫn ưu tiên trước.
- Sinh tồn bắt đầu rút lui dưới ngưỡng ít nhất 55% HP, hồi tới 72% mới bỏ trạng thái rút lui để tránh đổi hướng liên tục. Hồi máu khẩn cấp và khả năng hồi sinh có thể ưu tiên hơn nâng core trong chế độ này.
- Sinh tồn không dừng vì đủ mục tiêu tài nguyên. Hiện thời gian tốt nhất trong phiên đọc từ đồng hồ HUD; lưu cùng phiên khi ghi kết quả. Giới hạn phút/lượt và nút Dừng vẫn có hiệu lực.

## Sửa chọn Bond
- Sửa Bond hỗn hợp Hail + Hyper Beam bị chặn khi di chuyển/né mặc dù còn chiêu đánh tới mục tiêu.
- Bond ngoài core không còn bị loại hoàn toàn; Bond chính đủ 4 core vẫn ưu tiên khi có thể sử dụng.
- Khôi phục nhóm Bond 2–4 chiêu từ lịch sử ghép đã xác nhận khi HUD chỉ nhận diện được một phần và chỉ có một nhóm phù hợp.
- Tab Build hiển thị lý do đang giữ/chọn ô để dễ kiểm tra, không chỉ hiện tên nâng cấp gần nhất.

## Cập nhật và kiểm tra
Thay tệp trong thư mục tiện ích cũ, Reload tiện ích rồi tải lại game; Android nhập userscript mới. Core tự chọn vẫn giữ nguyên.

Đã kiểm tra bằng renderer HUD Doofcraft với bố cục ảnh (Hyper Beam / Confusion / Hex / Bond Hail + Hyper Beam), các quyết định theo mục tiêu, ngưỡng hồi phục, lưu cấu hình/core và các kiểm thử hồi quy. Chưa đo tỷ lệ thắng hoặc thời gian sống trong trận thực tế. Chưa có tín hiệu xác minh riêng boss cuối/chiến thắng; chế độ xử lý boss đã nhận diện, không cam kết phá đảo hoặc đủ điều kiện thương mại.

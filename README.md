# hoanganh Auto Farm · v2.7.1

Tải và cài đặt nhanh:

- **Máy tính (Chrome/Edge):** [⬇️ Tải ZIP v2.7.1](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v2.7.1/hoanganh-autofarm-resource-v2.7.1.zip)
- **Android (Firefox):** [⬇️ Tải gói Mobile v2.7.1](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v2.7.1/hoanganh-autofarm-mobile-v2.7.1.zip)

**Cài trên máy tính:** tải và giải nén ZIP → mở `chrome://extensions` (Edge: `edge://extensions`) → bật **Developer mode** → chọn **Load unpacked** → chọn thư mục vừa giải nén có `manifest.json` → mở lại game. Nếu Chrome hỏi, cho phép tiện ích chạy trên `pokesurvivor.com`.

**Cài trên Android:** tải ZIP Mobile, giải nén và nhập file `.user.js` vào trình quản lý userscript trong Firefox Android. Xem `README-ANDROID.md` trong gói để làm theo từng bước. Bản mobile đang thử nghiệm.

---
# hoanganh Auto Farm · Resource Pilot 2.7.1

## Cài đặt máy tính
Giải nén ZIP, mở chrome://extensions, bật Developer mode và Load unpacked chính thư mục có manifest.json. Tắt bản cũ để tránh hai bộ điều khiển chạy đồng thời. Tải lại toàn bộ tab https://pokesurvivor.com/, vào trận rồi bắt đầu. Không cần Node/npm để dùng extension.

## Mặc định mới: Ép vào Rift
Ở chế độ Vàng hoặc Vé, tùy chọn Ưu tiên Rift mặc định là Ép vào Rift. Khi nhận diện cổng, tool bỏ rương, vàng, vé và mục tiêu thường để đi tới cổng; giữ mục tiêu cả khi HP thấp hoặc chưa đọc được HP, cấp còn thấp và thời gian còn lại ngắn. Không áp dụng ngưỡng HP/cấp hay từ chối chỉ vì ước tính không tới kịp. Cổng đã hết hạn không được chọn.

Đây là chế độ chấp nhận rủi ro trong game theo yêu cầu người dùng. Con số mong muốn 90% được hiểu là ưu tiên hành vi, không phải tỷ lệ vào cổng đã đo. Vẫn cần nhận diện được người chơi, dữ liệu mới và đường đi khả dụng. Tool không tạo cổng, kéo dài thời hạn hay dịch chuyển nhân vật. Bị kẹt nhiều lần hoặc không xác nhận chuyển cảnh vẫn có thể khiến tool tạm dừng.

Ngay cả khi đang dùng mẫu di chuyển vòng/quét, Ép vào Rift sẽ tạm dùng bộ di chuyển thích ứng để đến cổng và chiến đấu trong arena; trở lại map thì về mẫu đã chọn. Né đòn trên đường đi vẫn hoạt động và giữ mục tiêu Rift để tiếp tục sau khi né. Chế độ Sinh tồn không chủ động vào Rift; tắt Theo cổng Rift cũng ngăn tự vào.

## Đổi về Cân bằng
Trong Farm → Ưu tiên Rift, chọn Cân bằng rồi Lưu và áp dụng. Chế độ này dùng ngưỡng HP vào cổng mặc định 75%, cấp 12, rút lui dưới 45% HP và ước tính thời gian di chuyển. Các ô ngưỡng HP/cấp cổng chỉ chi phối chế độ Cân bằng. Ở Ép vào Rift chúng không ngăn tiếp cận.

## Các chức năng hiện có
- Rift: giữ mục tiêu, áp sát bằng bước ngắn, đứng trong vùng vào và chờ xác nhận arena. Trong arena ưu tiên đánh boss rồi thu phần thưởng quan sát được; hộp thoại item/Bond được xử lý trước di chuyển.
- Né boss: nhận vòng AoE và tia nhiều màu, tia xoay chéo, dấu đạn địch; theo dõi vận tốc để dự đoán va chạm, ưu tiên né hơn gây sát thương. Build tầm xa giữ cự ly rộng hơn; vẫn chưa bảo đảm thắng mọi boss.
- Rương khóa: tới cạnh, nhả toàn bộ phím và giữ vị trí khoảng 3,5 giây. Đọc vòng tiến độ khi có; chờ rương biến mất, không chạy sang loot thường. Rift được ưu tiên hơn mở rương.
- Build: snapshot SurvivorTiers không TM; chọn thẻ theo bộ chiêu, HP và mục tiêu. Có thể reroll bằng lượt hiện có; khi hết lượt chọn dự phòng để tiếp tục. Bond ưu tiên bộ chiêu và ghép buff với sát thương khi nhận diện được.
- Item: so sánh item đang có với món mới theo mục tiêu/HP/cấp, giữ item nếu chưa thấy lợi ích đủ rõ hoặc tên chưa nhận diện.
- Orb: đọc 4 ô phím 5–8, số lượng và cooldown. Dùng khống chế khi bị áp sát, tốc độ để né/tiếp cận, sát thương khi đánh boss; tránh dùng chồng buff.

F8 bật/tạm dừng, F9 overlay, F6 nhận diện. Tự bấm WASD, rời tab hoặc mất focus sẽ tạm dừng. Giữ game ở màn hình trước. Tự chơi lại mặc định tắt; nếu game về menu nhiều bước, tool có thể yêu cầu bạn vào trận.

## Phạm vi xác minh
Đã kiểm tra logic và trình duyệt mô phỏng, kèm bộ vẽ tham chiếu đã ghim của game cho các kiểu báo chiêu. Chưa đo tỷ lệ vào Rift, tỷ lệ thắng boss hoặc vàng/vé mỗi giờ trong trận thật. Mobile chưa được xác minh trên thiết bị thật. Game thay đổi hình vẽ/DOM có thể làm nhận diện sai. Xem TESTING.md, SOURCES.md, PRIVACY.md.

Cần hỗ trợ: liên hệ [Facebook Nguyen Hoang Anh Support](https://www.facebook.com/NguyenHoangAnh.Support).


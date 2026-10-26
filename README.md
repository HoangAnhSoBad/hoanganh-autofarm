# hoanganh Auto Farm · v3.0.0

Auto farm cho [PokéSurvivor](https://pokesurvivor.com/) và [Doofcraft](https://pokesurvivor.doofcraft.com/). Tự nhận bản game theo website đang mở.

- **Máy tính:** [⬇ Tải ZIP v3.0.0](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.0.0/hoanganh-autofarm-resource-v3.0.0.zip)
- **Android:** [⬇ Tải gói Mobile v3.0.0](https://github.com/HoangAnhSoBad/hoanganh-autofarm/releases/download/v3.0.0/hoanganh-autofarm-mobile-v3.0.0.zip)

## Cài trên máy tính

1. Tắt bản cũ và giải nén ZIP mới.
2. Mở `chrome://extensions` hoặc `edge://extensions`, bật **Developer mode**.
3. Chọn **Load unpacked**, chọn thư mục có `manifest.json`.
4. Tải lại toàn bộ tab game, đăng nhập rồi mở menu Solo hoặc vào trận.

Không cần Node/npm để sử dụng. Extension dùng quyền notifications để hiện thông báo hoàn thành; bảng thông báo trong game vẫn hoạt động nếu hệ thống chặn thông báo.

## Nhiệm vụ và thẻ mới ở 3.0.0

- **Trick-or-treat:** theo mũi tên cam và khoảng cách, chuyển sang dấu ?/vòng tiến độ khi tới gần; đứng cạnh cửa để tương tác.
- **Lồng Pokémon:** phân biệt lồng đang có nhiệm vụ và vật trang trí; đứng gần chờ mở, không đánh nhầm Pokémon bị nhốt.
- **Đèn nhiệm vụ:** phân biệt đèn chưa thắp và đèn đã sáng; theo dõi tiến độ thắp.
- **Hộ tống:** tiếp cận NPC, dẫn về vòng xanh, quay lại nếu NPC tụt xa và chờ nó vào điểm cứu hộ. Cải thiện này áp dụng cả bản gốc.
- Nhặt kẹo sự kiện, đá quý và vé; bí ngô là vật phá được. Chỉ cộng mục tiêu sau khi game xác nhận kết quả lượt.
- Chọn **Revive**, Mega/biến hình, plate cùng hệ; xét độ hiếm của buff. Chọn phần thưởng rương Waves và ô khóa Choice Band theo mục tiêu/build.
- Bổ sung 17 chiêu và 10 Pokémon mới của Doofcraft. Những Pokémon chưa có dữ liệu mô phỏng dùng build suy luận, có ghi rõ trong xem trước.

Bật **Làm nhiệm vụ bản đồ / hộ tống Pokémon** và chọn di chuyển **Thích ứng theo tài nguyên/sự kiện**. Khi hiện Rift, cổng vẫn có ưu tiên cao hơn nhiệm vụ. Bot tạm ngừng đứng tương tác để né nguy hiểm. Chỉ báo ngoài màn hình dùng để tìm đường, không tự coi là đã tương tác thành công. Revive ở đây là lựa chọn thẻ dự trữ; bản này chưa tự bấm xác nhận dùng hồi sinh khi bị hạ.

Xem [EVENTS.md](EVENTS.md) để biết tín hiệu nhận diện và giới hạn.

## Farm đến đủ tài nguyên

Trong tab **Farm**:

1. Bật **Tự chơi lại qua menu Solo**.
2. Nhập số cần kiếm thêm, ví dụ **Vàng: 10k**, **Lượt gacha: 10**; mục tiêu khác để trống hoặc 0.
3. Đặt **Tối đa phút/lượt = 0** nếu muốn farm đến đủ mà không bị hai giới hạn này chặn. Cấu hình giới hạn từ bản cũ vẫn có thể được giữ lại.
4. Nhấn **Lưu và áp dụng cấu hình**, rồi **Bắt đầu**.

Tool theo dõi phần thưởng của các lượt trong phiên, không tính số dư tài khoản sẵn có. Vé ×10 và ×25 được tính thành 10 và 25 lượt gacha. Nếu đặt cả vàng và vé, cần đạt cả hai mục tiêu. Doofcraft còn hỗ trợ mục tiêu đá quý và kẹo sự kiện khi xuất hiện trong bảng kết quả.

Sau mỗi lượt, tool đọc phần thưởng game đã xác nhận, lưu tiến độ, quay về menu rồi vào Solo tiếp. Khi đủ mục tiêu, tool dừng chơi lại, hiện **Hoàn thành**, phát âm báo nếu bật và gửi thông báo máy tính. Việc hoàn tất được xét sau khi lượt kết thúc và phần thưởng được ghi nhận; tool không tự bỏ dở trận để lấy mốc chính xác giữa lượt.

Tiến độ vẫn còn sau khi tải lại trang. Nhấn **Bắt đầu/Tiếp tục** để tiếp tục phiên chưa hoàn thành; dùng **Đặt lại tiến độ phiên** khi muốn tính lại từ 0. Nếu game báo lượt chưa được ghi nhận, tool tạm dừng và chưa cộng phần thưởng. Giới hạn phút/lượt, việc rời tab hoặc tự tiếp quản vẫn có thể dừng phiên trước mục tiêu.

## TM và build của Pokémon

Trong tab **Build**, bật **Chuẩn bị TM và chiêu khởi đầu trước lượt** và **Dùng TM đã có cho Pokémon này**.

- Tool đọc TM của đúng Pokémon, xét các build không TM và các ứng viên tối ưu trong snapshot SurvivorTiers. Chỉ dùng ứng viên TM khi các chiêu bắt buộc đã có và phù hợp danh sách game hiển thị.
- Doofcraft: bật TM đã học nếu build cần, chọn chiêu khởi đầu/repertoire khi ô này đã mở khóa.
- Bản gốc: có thể dùng một TM sẵn trong túi để dạy chiêu cần thiết cho Pokémon đã chọn. Đây là thao tác tiêu hao TM có sẵn; có thể tắt Dùng TM nếu muốn giữ lại.
- Tool trang bị chiêu qua giao diện game, không mua TM hoặc nâng cấp. Nature/Ability vẫn là dữ liệu gợi ý.
- Item nhặt trong trận được so sánh theo kiểu đánh cận/xa, bộ chiêu, HP, giai đoạn và mục tiêu farm. Trang bị của game tồn tại trong lượt; tool không tạo thêm ô item ban đầu.

Build và đánh giá item là phương án tham khảo có điều kiện, chưa phải kết quả benchmark riêng về lợi nhuận farm hay cân bằng Doofcraft.

## Các chức năng khác

Theo cổng boss, né báo chiêu/đạn, thu vé/vàng, mở rương khóa bằng giữ vị trí, tự chọn nâng cấp/Bond, reroll bằng lượt sẵn có và chọn dự phòng khi hết lượt. Doofcraft có đọc tường/nước để tìm đường vòng. Bản gốc hỗ trợ orb theo tình huống.

**F8** bật/tạm dừng · **F9** đường đi · **F6** nhận diện. Giữ tab game ở phía trước. Game có bước đăng nhập, phòng nhóm, hộp thoại không nhận diện hoặc lượt đang lưu cần xác nhận thủ công có thể làm tool tạm dừng.

## Android

Giải nén ZIP Mobile, nhập `hoanganh-autofarm-mobile.user.js` vào trình quản lý userscript hỗ trợ chạy trong trang trên Firefox Android, ví dụ Tampermonkey. Tắt script cũ, bật script mới cho cả hai website và tải lại game. Xem `README-ANDROID.md`. Tiến độ lưu riêng theo website trên thiết bị, không đồng bộ với Chrome extension. Bảng hoàn thành và âm báo có sẵn; thông báo hệ thống tùy quyền trình duyệt. Mobile chưa kiểm tra trên điện thoại thật.

## Kiểm tra

Đã qua kiểm tra logic và trình duyệt mô phỏng cho cả hai game: hai lượt liên tiếp, chuẩn bị TM/chiêu đã có, mục tiêu 10k vàng + 10 lượt gacha, đổi vé gói, tránh đếm trùng khi reload, dừng chơi lại và thông báo một lần; kiểm tra thêm trường hợp phần thưởng chưa được ghi nhận. Đã kiểm tra thêm bằng bộ vẽ sự kiện/HUD/hộp chọn thực tế công khai của Doofcraft ở zoom 2, và bộ vẽ hộ tống của bản gốc. Chưa xác minh các tính năng mới bằng tài khoản chơi thật hoặc trên điện thoại, chưa đo tỷ lệ thắng boss hay tài nguyên mỗi giờ.

Xem `TESTING.md`, `SOURCES.md`, `PRIVACY.md`, `THIRD_PARTY_NOTICES.txt` trong ZIP.

Cần hỗ trợ: [Facebook Nguyen Hoang Anh Support](https://www.facebook.com/NguyenHoangAnh.Support).

# HoangAnh Auto Farm v3.13.0 · Máy tính

- Item ưu tiên: chọn trong tab Farm, thay đổi và lưu ngay khi đang chơi. Khi game đưa bảng đổi item, ưu tiên item bạn chọn; để Tự chọn theo tình huống để dùng chính sách cũ. Không tạo/trang bị item mà game chưa cho chọn.
- Bond core: xác nhận ô Bond rồi chuyển sang ngay cả khi chưa có địch trong tầm; giữ Bond core thay vì quay về chiêu đơn. Vẫn tôn trọng Choice Band và không đoán ô khi dữ liệu không chắc chắn.
- Tầm đánh: dựa vào chiêu đang dùng và dữ liệu tầm/đạn hiện có, thay vì kiểu build chung. Chiêu xa giữ cự ly, lùi khi boss áp sát và ưu tiên chạy vòng; chiêu gần tiến vào tầm. Chặn hướng đi xuyên thân boss cả khi đang đi vòng tới mục tiêu khác.
- Dùng chiêu: bổ sung điểm tình huống cho khống chế, đẩy lùi khi bị vây và một số chiêu hồi máu khi HP thấp, bên cạnh cấp chiêu, sát thương và thời gian hồi đã có.
- Di chuyển: bỏ điểm trung gian không cần thiết trên đường vòng khi đoạn nối đã kiểm tra không xuyên vật cản. Giảm đổi hướng và đổi mục tiêu loot chỉ vì chênh lệch nhỏ; né đòn/hồi phục vẫn được ưu tiên ngay.
- Doofcraft: nhận đúng hình cột Obelisk của Eternatus và Mega Darkrai; ưu tiên phá cột quan sát được trước boss, giữ tầm và né nguy hiểm. Khi cột biến mất, đánh giá lại boss. Không áp dụng nhận diện này cho cột chưa xác minh ở bản gốc.

## Tải và cài
[Tải ZIP máy tính](https://github.com/HoangAnhSoBad/hoanganh-autofarm/raw/refs/heads/main/hoanganh-autofarm-resource-v3.13.0.zip) · [Hướng dẫn từng bước](https://github.com/HoangAnhSoBad/hoanganh-autofarm#readme)

Giải nén → Load unpacked → chọn thư mục màu vàng hoanganh-autofarm-resource-v3.13.0 → Chọn Cặp. Không chọn riêng manifest.json. Nếu đã cài, chép nội dung mới vào đúng thư mục cũ → Reload tiện ích → tải lại game.

Đã qua kiểm thử hồi quy và mô phỏng trình duyệt: đổi/lưu item trong trận, chọn/giữ Bond khi di chuyển, tầm gần/xa, va chạm boss và địa hình; nhận diện hình cột thật của renderer game ở scale 1/1.5/2. Chưa đo tỷ lệ thắng boss hoặc hiệu quả treo qua đêm trên trận thật; không bảo đảm điều khiển như người chơi hay né mọi đòn.

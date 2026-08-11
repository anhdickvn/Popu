# Popu / ChatApp

Bản iOS chat client Minecraft Java 1.12.x.

## Bản sửa này
- WASD + Jump bố trí dạng D-pad thẳng hàng, nút Jump riêng.
- Mini-map 48×48 lấy địa hình từ Chunk Data của server, không chỉ vẽ đường đi.
- Hiển thị X/Y/Z và trạng thái mặt đất.
- Giữ kết nối khi đưa app xuống nền bằng cơ chế background hiện có; iOS vẫn có thể dừng tiến trình trong một số trường hợp.
- Server/account có nút ✏️ sửa và 🗑️ xóa; sửa IP/port/username cập nhật hồ sơ hiện tại.
- GUI server hiển thị dạng danh sách item giống inventory list, có icon thật, tên, số lượng và menu `...`.
- Giữ login tự động, compass hotbar 5 và click Diamond Axe slot 23.
- Giữ Logs chỉ lưu chat server và mã màu.

## UI / movement / map update
- WASD is rendered as a fixed 3x2 D-pad with a separate Jump button.
- Mini-map parses Minecraft 1.12.x chunk-section bits/palette/data arrays and renders the highest non-air block per X/Z as a 48x48 height-map.
- Server and username records remain editable with pencil buttons and deletable with confirmation.
- Background connection is kept while iOS allows the app to run in the audio background mode; if the socket is lost, the client reconnects automatically when possible.

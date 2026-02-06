# Mạch đóng ngắt tải MKE-M05 1-Relay Module

## Giới thiệu sản phẩm
MKE-M05 1-Relay Module là mạch đóng ngắt tải bằng relay hoạt động như một công tắc 3 cực, bao gồm tiếp điểm **thường đóng (NC), thường mở (NO) và chân chung (COM)**. Relay được điều khiển thông qua tín hiệu kích hoạt từ mạch xử lý, cho phép đóng ngắt các tải một chiều (DC) hoặc xoay chiều (AC) một cách linh hoạt. Khi sử dụng với điện áp cao, người dùng cần đặc biệt chú ý đến các yêu cầu an toàn trong quá trình lắp đặt và vận hành.

Mạch đóng ngắt tải MKE-M05 1-Relay Module được ứng dụng rộng rãi trong nhiều tình huống thực tế như: điều khiển đèn chiếu sáng, quạt điện, máy bơm mini, chuông báo, khóa điện, các thiết bị gia dụng đơn giản, hệ thống nhà thông minh (Smart Home), cũng như các mạch tự động hóa cơ bản. Ngoài ra, mạch còn rất phù hợp cho các mô hình robot, dự án STEM, đồ án học tập và thực hành điện – điện tử, giúp người học dễ dàng tiếp cận nguyên lý điều khiển tải bằng relay.

Mạch đóng ngắt tải MKE-M05 1-Relay Module hỗ trợ điện áp điều khiển 3.3V và 5VDC, cho phép kết nối trực tiếp và an toàn với hầu hết các bo mạch điều khiển phổ biến hiện nay như Arduino, Raspberry Pi, Jetson Nano, Micro:bit và nhiều nền tảng khác. Sản phẩm đi kèm cáp kết nối 3P XH2.54 – Dupont, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

## Thông số kỹ thuật
- Điện áp cấp nguồn: 5VDC
- Chuẩn tín hiệu điều khiển: Digital
- Điện áp giao tiếp: TTL 3.3/5VDC
- Loại Relay: 5VDC
- Mạch bảo vệ:
  - Tích hợp transistor giúp giảm dòng tiêu thụ
  - Bảo vệ an toàn cho chân GPIO của vi điều khiển
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Ổn định, chống nhiễu
  - Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 3P XH2.54–Dupont

## Các chân tín hiệu
<table><thead>
  <tr>
    <th>MKE-M05</th>
    <th>Ghi chú</th>
  </tr></thead>
<tbody>
  <tr>
    <td>GND</td>
    <td>Chân cấp nguồn âm 0VDC</td>
  </tr>
  <tr>
    <td>5V</td>
    <td>Chân cấp nguồn dương 5VDC</td>
  </tr>
  <tr>
    <td>SIG</td>
    <td>Chân tín hiệu điều khiển Digital In</td>
  </tr>
  <tr>
    <td>NC</td>
    <td>Cổng kết nối chân tiếp điểm thường đóng của Relay (Normally Close)</td>
  </tr>
  <tr>
    <td>COM</td>
    <td>Cổng kết nối chân tiếp điểm chung của Relay (Common)</td>
  </tr>
  <tr>
    <td>NO</td>
    <td>Cổng kết nối chân tiếp điểm thường mở của Relay (Normally Open)</td>
  </tr>
</tbody>
</table>

## Hướng dẫn sử dụng
### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân GND và 5V.
- Điều khiển Relay qua chân tín hiệu SIG.
<table><thead>
  <tr>
    <th>SIG (Digital In)</th>
    <th>Trạng thái</th>
  </tr></thead>
<tbody>
  <tr>
    <td>TTL HIGH (3.3/5VDC)</td>
    <td>Không hoạt động (Off)</td>
  </tr>
  <tr>
    <td>TTL LOW (0VDC)</td>
    <td>Hoạt động (On)</td>
  </tr>
</tbody>
</table>

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu **"MKE_M05_Relay_Serial_XXX"** tại **File / Examples / MAKEREDU / Module / MKE_M05_Relay**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port** của mạch và nhấn **Upload** để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân SIG của module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import** chương trình theo đường link sau: `https://github.com/makereduvn/mke_m05_relay_microbit/`
- Kết nối mạch Micro:bit và **Download** chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân SIG của module với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT** trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT** sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-M05 Relay](/extras/MKE-M05_1.jpg)

## Hình ảnh sản phẩm
![MKE-M05 Relay](/extras/MKE-M05_2.png)
![MKE-M05 Relay](/extras/MKE-M05_3.png)




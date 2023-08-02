# Quy chuẩn đặt tên footprint linh kiện

Các footprint được đặt tên theo phạm vi từ tổng quát đến chi tiết, các thuộc tính sẽ được ngăn cách với nhau bằng dấu **-** với nhau, lý do sử dụng  **-** thay vì **_** vì nó cho phép thay đổi giá trị thuộc tính nhanh hơn bằng cách nhấn __*Ctrl + →*__ để di chuyển nhanh con trỏ giữa các thuộc tính

Ví dụ:
```
Header-Vert-THT-2.54mm-5P-Female_Header
```
Nếu con trỏ đang ở đầu vị trí chữ "Header", nếu muốn đổi chữ Vert (Vertical biểu thị linh kiện hướng thẳng đứng) thành Horz (Horizontal biểu thị linh kiện đặt nằm ngang) thì chỉ cần dùng __*Ctrl + →*__ thì sẽ di chuyển con trỏ tới đầu chữ __*Vert-*__ một cách nhanh chóng để thay đổi, tiết kiệm được thời gian sửa đổi thông số, cũng như copy sang một linh kiện giống nhau nhiều thuộc tính, ví dụ:

```
Header-Vert-THT-2.54mm-6P-Female_Header
```
## Một số phân nhóm linh kiện thông dụng
### 1. Phân nhóm Connector:
- Terminal(hoặc TerminalBlock): Đây là một loại connector được sử dụng để cấp nguồn cho thiết bị hoặc cho mạch điện, thường sử dụng cho đầu vào cấp nguồn hoặc đầu ra công suất(ví dụ như điều khiển động cơ, các thiết bị tải lớn).

- Header: Đây là connector sử dụng để truyền tín hiệu trong mạch điều khiển, nên kích thước thường nhỏ như một đường bus dây đi chung theo cụm.
- USB: Phân nhóm chung cho các cổng USB giao tiếp với máy tính, ví dụ như USB-C, USB-type A, mini USB, micro USB ...

- LED(Light Emitting Diode)
### 2. Phân nhóm linh kiện thụ động (passive components)
1. Điện trở

2. Tụ điện

- Capacitor Polarize: Loại tụ điện có phân cực như tụ nhôm (Aluminum), tụ Tantalum
- Capacitor Unpolar: như tụ gốm (Ceramic cap) hoặc tụ kẹo (Polyester cap)

2.Cuộn cảm
### 3. Phân nhóm socket

Có thể hiểu giống như một cái khuôn để đặt vật thể, hoặc đưa vật thể vào đó và giữ chặt nó

- BatteryHolder
- SD card
- MicroSIM, NanoSIM
...


### 4. Phân nhóm chuẩn đóng gói linh kiện (package components)
- Package: là tên đóng gói linh kiện khi sản xuất đại trà, ví dụ transistor BJT C1815 có package dạng cắm THT là TO-92, còn với dạng hàn SMD thì có package là SOT23-3

- Button và switch(có thể viết tắt là Btn và SW):Phân nhóm các nút nhấn tactile (switch tactile, đây là loại nút nhấn nhỏ, dùng cho điện áp thấp và dòng điện nhỏ và thường để hàn lên mạch PCB) và button và công tắc gạt (slide switch)
- MCU(Micro Controller Unit): các dạng kỹ thuật số IC có thể lập trình được
## Ý nghĩa các thuộc tính khi đặt tên linh kiện

Cách đặt tên cho footprint theo quy chuẩn sau:

__*Note*__ : Lưu ý rằng quy chuẩn này có thể thay đổi trong tương lai nếu không phù hợp để quản lý thư viện linh kiện ở một quy mô lớn hơn

```
Nhóm linh kiện - Phương đặt linh kiện trên board - Phương pháp hàn lên PCB - khoảng cách giữa 2 chân - số chân linh kiện - tên linh kiện 
```
1. Nhóm linh kiện: Đây là tên gọi chung cho tập hợp các linh kiện có cùng chức năng, mục đích sử dụng

2. Phương đặt linh kiện: phương nằm ngang (Horizontal, viết tắt thành Horz) hoặc phương thẳng đứng (Vertical, viết tắt thành Vert)

3. Phương pháp hàn linh kiện: hàn cắm THT (Through Hole Technology) hoặc SMD (Surface Mount Device)

4. Khoảng cách giữa 2 chân linh kiện(thường áp dụng đối với connector, hàng rào hoặc Terminal, ít áp dụng với package IC): khoảng cách tiêu chuẩn thường được sử dụng là 2.54mm (tương ứng với 100mil = 0.1inch), 1.27mm, 2.0mm, 3.96mm, 5.08mm

5. Số chân linh kiện (thường áp dụng đối với connector, hàng rào hoặc Terminal): Nếu là hàng rào đôi thì ghi <số hàng x số chân> , ví dụ như cổng DB có 14 chân 2 hàng thì sẽ là 2x7P

6. Đây là tên linh kiện, có thể dùng **_** để ngăn cách, ví dụ: S4B_XH_SM4_TB

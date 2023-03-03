# __*Hướng dẫn thêm thư viện IoTVision vào KICAD*__
1. Vào KICAD

2. Chọn **Preferences -> Configure Paths**

3. Nhấn vào biểu tượng **+** ở giữa trái

    - Thêm đường dẫn 3D: Gán alias (tên thay thế) vào mục **Name** (ví dụ **IOTVISION_3D**), trỏ đường dẫn đến thư mục 3D step và bỏ đường dẫn vào **PATH**
    
    - Thêm đường dẫn SYMBOL: Gán alias (tên thay thế) vào mục **Name** (ví dụ **IOTVISION_SYMBOL_DIR**), trỏ đường dẫn đến thư mục symbols và bỏ đường dẫn vào **PATH**
    
    - Thêm đường dẫn FOOTPRINT: Gán alias (tên thay thế) vào mục **Name** (ví dụ **IOTVISION_FOOTPRINT_DIR**), trỏ đường dẫn đến thư mục footprints và bỏ đường dẫn vào **PATH**
    

4. Nhấn OK

5. Chọn **Preferences -> Manage Symbol Libraries  -> Global Libraries**, nhấn vào biểu tượng **+** ở dưới trái

    - Nickname: **IVS_SYMBOLS**
    
    - Library Path: **${IOTVISION_SYMBOL_DIR}/Symbols.kicad_sym**
    
    - Nhấn OK
**Lưu ý**: Nếu mở **PCB Editor** hoặc **Footprint Editor** sẽ không thấy **Manage Symbol Libraries**

6. Chọn **Preferences -> Manage Footprint Libraries -> Global Libraries**, nhấn vào biểu tượng **+** ở dưới trái

    - Nickname: **IVS_FOOTPRINTS** __*(BẮT BUỘC)*__
    
    - Library Path: **${IOTVISION_FOOTPRINT_DIR}/IVSFootprint.pretty**
    
    - Nhấn OK
**Lưu ý**: Nếu mở **Schematic Editor** hoặc **Symbol Editor** sẽ không thấy **Manage Footprint Libraries**

# __*Hotkeys*__

## Thêm Hotkeys vào KICAD

Chọn **Preferences -> Preferences -> Hotkeys**, ở giữa dưới chọn **Import Hotkeys**


## PCB Editor

Chuyển qua Schematic: __*K*__

### Via

Đặt via xuyên lỗ : __*V*__ (áp dụng khi đang ở chế độ đi dây)

Giảm kích thước via: __*\*__

Tăng kích thước via: __*'*__

### Dây

Vẽ dây mới: __*X*__

Tăng bề rộng dây: __*W*__

Giảm bề rộng dây: __*Shift + W*__

Xoay hướng đi dây: __*/*__

Đổi chế độ đi dây (bo tròn 45 và 90 độ; vuông góc; 45 độ): __*Ctrl+/*__

Chọn mở rộng đường dây: __*Tab*__

Chọn mở rộng toàn bộ đường dây: __*U*__

### View

Phóng to: __*F1*__

Thu nhỏ: __*F2*__

Lật view board: __*Shift + F*__

Chuyển giữa 2 lớp đang làm việc: __*V*__ (khi không ở chế độ đi dây)


Hiển thị/ẩn ratnest: __*J*__

Hiển thị ratnest của footprint được chọn: __*Shift+J*__

Chỉnh độ mờ dây : __*Shift + [*__ và __*Shift + ]*__

Highlight dây: __*Ctrl + `*__

### Xếp linh kiện

Lật linh kiện: __*F*__

Căn lề trái: __*Alt+L*__

Căn lề phải: __*Alt+R*__

Căn lề Top: __*Alt+T*__

Căn lề Bot: __*Alt+B*__

Căn giữa dọc: __*Alt+V*__

Căn giữa ngang: __*Alt+H*__

Mirror: __*Shift + X*__

Phân bố đều khoảng cách linh kiện theo chiều ngang: __*Alt + X*__

Phân bố đều khoảng cách linh kiện theo chiều ngang: __*Alt + Y*__

Xoay linh kiện: __*R*__

Khóa/mở khóa linh kiện: __*L*__

### Nhóm linh kiện

Update footprint: __*F7*__

Chuyển sơ đồ nguyên lý sang pcb: __*F8*__

### Nhóm linh kiện

Tạo nhóm linh kiện: __*G*__

Vào nhóm linh kiện để chỉnh sửa: __*Shift + G*__

Hủy nhóm: __*Ctrl + G*__


### Phủ đồng polygon

Phủ đồng: __*B*__

Hủy phủ đồng: __*Ctrl + B*__

## 3D

Lật board: __*F*__

Hiển thị/ẩn linh kiện cắm: __*T*__

Hiển thị/ẩn linh kiện cắm: __*S*__

## Schematic

Thoát khối Hierarchical: __*Alt+backspace*__

Chuyển qua PCB: __*K*__

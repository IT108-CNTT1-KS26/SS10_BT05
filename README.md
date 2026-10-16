# Dự án Smart-Farm: Hệ Thống Tưới Lan Tự Động

*Dự án cung cấp giải pháp IoT toàn diện, giúp người nông dân theo dõi và tự động hóa quy trình chăm sóc vườn Lan dựa trên dữ liệu thời gian thực.*

![Sơ đồ kiến trúc hệ thống Smart Farm](https://via.placeholder.com/800x400.png?text=So+Do+Kien+Truc+Smart+Farm)

## 1. Tính năng cốt lõi

Dưới đây là danh sách các tính năng đã hoàn thiện và chuẩn bị cập nhật:
- [x] Tự động bơm nước khi độ ẩm đất xuống thấp.
- [x] Cảnh báo nhiệt độ vượt ngưỡng qua tin nhắn SMS.
- [x] Lưu trữ dữ liệu lịch sử chăm sóc lên Cloud.
- [ ] Bổ sung AI nhận diện sâu bệnh qua Camera.

## 2. Thông số kỹ thuật thiết bị

| Thiết bị / Module | Vai trò trong hệ thống | Giao thức kết nối | Nguồn cấp |
| :--- | :--- | :--- | :--- |
| **Cảm biến DHT22** | Đo nhiệt độ & độ ẩm không khí | Digital | 3.3V - 5V |
| **Mạch SoC ESP32** | Khối xử lý trung tâm (CPU + Wi-Fi) | Wi-Fi / Bluetooth | 5V |
| **Module Relay 5V** | Điều khiển máy bơm nước | Digital | 5V |

## 3. Hướng dẫn cài đặt

Để nạp mã nguồn vào mạch xử lý trung tâm, vui lòng thực hiện các lệnh sau trong Terminal:

```bash
# Clone kho lưu trữ về máy
git clone [https://github.com/your-repo/smart-farm-lan.git](https://github.com/your-repo/smart-farm-lan.git)

# Di chuyển vào thư mục dự án
cd smart-farm-lan

# Cài đặt các thư viện phụ thuộc
pip install -r requirements.txt

# Chạy script khởi động hệ thống
python main.py
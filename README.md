# 🌐 Hệ Thống Web Server & DNS Server Trên Linux (Nhóm 1)

![Ubuntu](https://img.shields.io/badge/OS-Ubuntu%20Server-E95420?style=flat-down&logo=ubuntu&logoColor=white)
![Apache](https://img.shields.io/badge/Web%20Server-Apache2-D22128?style=flat-down&logo=apache&logoColor=white)
![Bind9](https://img.shields.io/badge/DNS%20Server-Bind9-79919E?style=flat-down&logo=linux&logoColor=white)

Một dự án hạ tầng mạng giúp biến máy chủ Linux thành nơi vừa quản lý tên miền (DNS), vừa lưu trữ và vận hành cùng lúc nhiều trang web khác nhau trên một địa chỉ IP duy nhất.

---

### 🎯 Mục Đích Dự Án
* **Thay thế IP thô bằng Tên miền:** Giúp người dùng truy cập website bằng các tên miền dễ nhớ (như `web2.net`, `tuan.com`) thay vì phải gõ địa chỉ IP số phức tạp (`192.168.25.129`).
* **Tối ưu hóa tài nguyên máy chủ:** Chạy song song nhiều website độc lập (Multi-website) trên cùng một máy chủ duy nhất nhằm tiết kiệm chi phí và tài nguyên IP.

---

### 🛠️ Chức Năng Chính

1. **Phân giải tên miền (DNS Server - Bind9):**
   * **Phân giải xuôi:** Dịch từ tên miền người dùng gõ (`bi.com`, `an.net`, `hung.net`...) thành IP `192.168.25.129` để máy tính hiểu và kết nối.
   * **Phân giải ngược:** Dịch ngược từ IP `192.168.25.129` ra lại toàn bộ danh sách tên miền hệ thống đang sở hữu.

2. **Lưu trữ đa website (Web Server Virtual Hosts - Apache2):**
   * Tự động nhận diện tên miền người dùng đang gõ để hiển thị đúng thư mục mã nguồn và giao diện tương ứng (Truy cập `web1.local` ra trang web 1, truy cập `web2.net` ra trang web 2).

3. **Kết nối và phục vụ máy trạm (Client Support):**
   * Cho phép các máy tính khác trong mạng nội bộ (ví dụ: Windows 11) chỉ cần cấu hình DNS trỏ về Server là có thể lướt các trang web nội bộ này trực tiếp bằng trình duyệt (Chrome, Edge).

---

### 💻 Công Nghệ Sử Dụng
* **Hệ điều hành:** Ubuntu Server 24.04.4 LTS
* **Dịch vụ DNS:** Bind9
* **Dịch vụ Web:** Apache2 (Tính năng Virtual Hosts)
* **Môi trường:** Máy ảo VMware

---

### 👥 Thành Viên Thực Hiện
* **Sinh viên thực hiện (Nhóm 1):** Đoàn Quang Huy và các người cộng sự.

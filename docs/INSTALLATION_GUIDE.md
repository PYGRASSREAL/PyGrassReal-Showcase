# 💻 คู่มือการติดตั้งโปรแกรม PyGrassReal Desktop (Windows Installation Guide)

เอกสารนี้แนะนำขั้นตอนการติดตั้งโปรแกรม **PyGrassReal Desktop** สำหรับระบบปฏิบัติการ Windows ทีละขั้นตอนอย่างละเอียด

---

## ⚙️ สเปกคอมพิวเตอร์ที่แนะนำ (System Requirements)

| รายการ | สเปกขั้นต่ำ (Minimum) | สเปกที่แนะนำ (Recommended) |
| :--- | :--- | :--- |
| **ระบบปฏิบัติการ** | Windows 10 / 11 (64-bit) | Windows 11 (64-bit) |
| **หน่วยประมวลผล (CPU)** | Intel Core i5 / AMD Ryzen 5 | Intel Core i7 / AMD Ryzen 7 ขึ้นไป |
| **หน่วยความจำ (RAM)** | 8 GB | 16 GB หรือ 32 GB |
| **การ์ดจอ (GPU)** | การ์ดจอรองรับ WebGL 2.0 / DirectX 12 | NVIDIA GeForce RTX 3060 ขึ้นไป (สำหรับ Gaussian Splats) |
| **พื้นที่ว่างบนดิสก์** | 2 GB (SSD) | 10 GB (NVMe SSD) |

---

## 📥 ขั้นตอนการติดตั้ง (Step-by-Step Installation)

### 1. ดาวน์โหลดตัวติดตั้ง
* ไปที่หน้า **[Releases](https://github.com/OWNER/pygrassreal-showcase/releases/latest)** บน GitHub
* คลิกดาวน์โหลดไฟล์ **`pygrassreal-windows-setup.exe`**

### 2. รันตัวติดตั้งบนเครื่อง
1. ดับเบิลคลิกที่ไฟล์ `pygrassreal-windows-setup.exe`
2. หากมีหน้าต่างเตือนความปลอดภัยของ Windows (SmartScreen) ปรากฏขึ้น ให้คลิก **More info** -> เลือก **Run anyway**
3. เลือกตำแหน่งโฟลเดอร์ปลายทางที่ต้องการติดตั้ง (หรือใช้ค่าเริ่มต้นที่ระบบกำหนด)
4. เลือกสร้างไอคอนบน Desktop (Create Desktop Shortcut)
5. กดปุ่ม **Install** และรอให้ระบบคัดลอกไฟล์จนเสร็จสมบูรณ์

### 3. เริ่มต้นใช้งานครั้งแรก
1. เปิดโปรแกรมจาก Shortcut **PyGrassReal** บน Desktop
2. ล็อกอินด้วยบัญชี PyGrassReal ของคุณ (หรือสมัครสมาชิกใหม่ผ่านหน้าโปรแกรม)
3. เริ่มต้นสร้างชิ้นงาน 3D Parametric และเรียกใช้งานทีม AI ได้ทันที!

---

## ❓ การแก้ปัญหาเบื้องต้น (Troubleshooting)

* **เปิดโปรแกรมแล้วจอดำหรือไม่โหลด:**
  - ตรวจสอบว่าได้ติดตั้ง Driver การ์ดจอรุ่นล่าสุดแล้ว
  - ตรวจสอบการเชื่อมต่ออินเทอร์เน็ตในการโหลดชุดข้อมูล 3D ครั้งแรก
* **ต้องการติดต่อทีมซัพพอร์ต:**
  - อีเมล: support@pygrassreal.com

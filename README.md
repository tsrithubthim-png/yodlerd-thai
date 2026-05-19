# ⚔ สยามศึก (Sayam Suek)
## Thai Historical Fighting Game — PWA

เกมต่อสู้บุคคลสำคัญในประวัติศาสตร์ไทย สไตล์ Street Fighter

---

## 🎮 Features

- **10 ตัวละคร** จากประวัติศาสตร์ไทย พร้อมสกิลเฉพาะตัว
- **3 โหมดเกม**: ผู้เล่น VS ผู้เล่น, ผู้เล่น VS บอท, ตะลุยด่าน Arcade
- **Arcade Mode**: 8 ด่าน มีเนื้อเรื่อง ฉากสัมพันธ์กับตัวละคร
- **ประวัติตัวละคร**: กดดูประวัติละเอียดของแต่ละตัวละคร
- **Bot AI** 4 ระดับ: ง่าย / ปกติ / ยาก / นรก
- **PWA**: ติดตั้งได้ เล่น Offline ได้
- **Mobile Support**: ปุ่มควบคุมบนหน้าจอ รองรับ touch

---

## 🚀 Deploy to GitHub Pages

### วิธีที่ 1 — GitHub Web UI
1. สร้าง repository ใหม่ใน GitHub
2. อัปโหลดไฟล์ทั้งหมดใน folder นี้
3. ไปที่ **Settings → Pages**
4. เลือก **Source: Deploy from a branch**
5. เลือก **Branch: main** และ **Folder: / (root)**
6. กด **Save** — เกมจะ live ที่ `https://USERNAME.github.io/REPO-NAME`

### วิธีที่ 2 — Git Command Line
```bash
git init
git add .
git commit -m "Initial commit: สยามศึก PWA"
git branch -M main
git remote add origin https://github.com/USERNAME/sayam-suek.git
git push -u origin main
```
จากนั้นเปิด Pages ใน Settings ตามวิธีที่ 1

---

## 📁 File Structure
```
sayam-suek/
├── index.html          # เกมหลัก (ไฟล์เดียว)
├── manifest.json       # PWA manifest
├── sw.js               # Service Worker (offline)
├── README.md           # ไฟล์นี้
└── icons/
    ├── icon-72.png
    ├── icon-96.png
    ├── icon-128.png
    ├── icon-144.png
    ├── icon-152.png
    ├── icon-192.png
    ├── icon-384.png
    └── icon-512.png
```

---

## 🎯 Controls

| | ผู้เล่น 1 | ผู้เล่น 2 |
|---|---|---|
| เดินซ้าย/ขวา | A / D | ← / → |
| กระโดด | W | ↑ |
| ป้องกัน | S (กด) | ↓ (กด) |
| ต่อย | G | K |
| เตะ | H | L |
| สกิล 1 | B | U |
| สกิล 2 | N | I |
| ท่าไม้ตาย | M | O |

---

## 👥 ตัวละคร

| ตัวละคร | ยุค | จุดเด่น |
|---|---|---|
| สมเด็จพระนเรศวรมหาราช | อยุธยา | HP สูง, พลังแรง |
| สมเด็จพระสุริโยไท | อยุธยา | เร็วที่สุด, dash |
| สมเด็จพระเจ้าตากสินมหาราช | ธนบุรี | สมดุล, วังวน |
| พระยาพิชัยดาบหัก | ธนบุรี | พลังสูงสุด |
| พ่อขุนรามคำแหงมหาราช | สุโขทัย | อักษรทอง |
| ท้าวเทพกษัตรี | ถลาง | โล่ป้องกัน |
| สมเด็จพระรามาธิบดีที่ ๑ | อยุธยา | ดาบทองคำ |
| พระยากาวิละ | ล้านนา | พายุหิมะ |
| กรมพระราชวังบวรฯ | รัตนโกสินทร์ | เกราะราชวัง |
| นายดาบจันทร์ | อยุธยา | ดาบคู่ |

---

## 📱 ติดตั้งเป็น App (PWA)

**Android (Chrome)**:
1. เปิดเกมในเบราว์เซอร์
2. แตะเมนู ⋮ → "Add to Home screen"

**iOS (Safari)**:
1. เปิดเกมใน Safari
2. แตะ Share → "Add to Home Screen"

**Desktop (Chrome/Edge)**:
1. คลิกไอคอนติดตั้งในแถบ address bar

---

*Built with HTML5 Canvas · No dependencies · Works offline*

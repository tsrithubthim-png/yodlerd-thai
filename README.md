# ยอดเลือดไทย — PWA Deploy Guide

## ไฟล์ในโปรเจกต์นี้
```
yodlerd-pwa/
├── index.html      ← ตัวเกมหลัก
├── manifest.json   ← PWA config
├── sw.js           ← Service Worker (offline support)
├── icon-192.png    ← App icon
└── icon-512.png    ← App icon (ใหญ่)
```

---

## วิธี Deploy ฟรีบน GitHub Pages

### ขั้นตอนที่ 1 — สร้าง GitHub Repo
1. ไปที่ https://github.com → New repository
2. ตั้งชื่อ เช่น `yodlerd-thai`
3. ตั้งเป็น **Public**
4. กด Create repository

### ขั้นตอนที่ 2 — อัพโหลดไฟล์
วิธีง่ายสุด: ลากไฟล์ทั้ง 5 ไฟล์ วางในหน้า repo

หรือใช้ Git:
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/USERNAME/yodlerd-thai.git
git push -u origin main
```

### ขั้นตอนที่ 3 — เปิด GitHub Pages
1. ไป Settings → Pages
2. Source → Deploy from branch
3. Branch → main → / (root)
4. กด Save
5. รอ 2-3 นาที → ได้ URL เช่น `https://username.github.io/yodlerd-thai`

---

## วิธีติดตั้งบนมือถือ

### Android (Chrome)
1. เปิด URL ใน Chrome
2. แถบบนจะมีปุ่ม **"Add to Home screen"** หรือกด ⋮ → Add to Home screen
3. กด Install → ได้ไอคอนบนหน้าจอเลย

### iPhone (Safari)
1. เปิด URL ใน **Safari** (ต้องเป็น Safari เท่านั้น)
2. กดปุ่ม Share (กล่องมีลูกศรขึ้น)
3. เลือก **Add to Home Screen**
4. กด Add

---

## หมายเหตุ
- เกมเล่นออฟไลน์ได้หลังจากเปิดครั้งแรก (Service Worker cache)
- รองรับ landscape mode อัตโนมัติ
- ไม่มีค่าใช้จ่ายใดๆ ทั้งสิ้น

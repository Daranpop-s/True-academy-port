# รอบ Portfolio TCAS70 — คู่มือสำหรับผู้ปกครอง

หน้าเว็บ static หน้าเดียว (single-page) อธิบายรอบ Portfolio ของ TCAS70 สำหรับผู้ปกครอง

## โครงสร้าง

| ไฟล์ | คำอธิบาย |
| --- | --- |
| `index.html` | ตัวคู่มือทั้งหมด — HTML/CSS อยู่ในไฟล์เดียว ไม่ต้อง build |
| `vercel.json` | ตั้งค่า static hosting บน Vercel |

ฟอนต์ IBM Plex Sans Thai โหลดจาก Google Fonts ส่วนที่เหลือไม่มี dependency ภายนอก

## ดูหน้าเว็บบนเครื่อง

เปิด `index.html` ด้วยเบราว์เซอร์ได้เลย หรือรัน static server:

```bash
npx serve .
```

## Deploy บน Vercel

Vercel จะตรวจเป็นโปรเจกต์ static อัตโนมัติ (ไม่มี build step) และ serve `index.html` ที่ root

1. เข้า [vercel.com/new](https://vercel.com/new) แล้ว import repo นี้
2. Framework Preset: **Other**, Build Command: เว้นว่าง, Output Directory: `.`
3. กด Deploy

หรือใช้ CLI:

```bash
npx vercel --prod
```

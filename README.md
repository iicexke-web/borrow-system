# Borrow & Return — GitHub Pages

โฟลเดอร์นี้พร้อมอัปโหลดขึ้น GitHub แล้ว

## สิ่งที่มีอยู่
- `index.html` — แอปทั้งหมด (CSS + JS + ข้อมูลจาก Excel ฝังอยู่แล้ว)
- `README.md` — ไฟล์นี้

ไม่ต้องอัปโหลด `.xlsx`, `.json` หรือ `.ps1` เพราะข้อมูลถูกฝังใน `index.html` แล้ว

## วิธีอัปโหลด (ไม่ต้องติดตั้ง Git ก็ได้)
1. สร้าง repository ใหม่บน GitHub ชื่อเช่น `asset-lend`
2. กด **Add file → Upload files**
3. เลือกไฟล์ภายในโฟลเดอร์นี้ (** index.html ** และ README.md) แล้วกด Commit
   - ให้ `index.html` อยู่ที่ **root** ของ repo (ไม่ใช่ในโฟลเดอร์ย่อย)
4. ไปที่ **Settings → Pages**
5. Build and deployment:
   - Source: **Deploy from a branch**
   - Branch: `main` → `/ (root)`
   - กด **Save**
6. รอ 1–2 นาที แล้วเปิด:
   `https://<your-github-username>.github.io/asset-lend/`

## อัปเดตทีหลัง
แก้ `index.html` ในโฟลเดอร์นี้ → Upload แทนของเดิม → GitHub Pages จะ deploy ใหม่ 자동

## หมายเหตุ
- ข้อมูลการยืม/คืนเก็บใน `localStorage` ของเบราว์เซอร์แต่ละเครื่อง (ไม่ sync ระหว่างเครื่อง)
- ถ้าอยากให้หลายคนเห็นข้อมูลร่วมกัน ต้องเพิ่ม backend/DB เช่น Firebase หรือ Supabase

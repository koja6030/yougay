# IT ERROR — THE FIVE SOULS

โปรเจกต์นี้เตรียมจากไฟล์ HTML เกมเดิมให้ใช้กับ GitHub และสร้าง Android APK ผ่าน GitHub Actions

## วิธีอัปโหลดขึ้น GitHub
1. สร้าง Repository ใหม่บน GitHub
2. แตก ZIP แล้วอัปโหลดไฟล์และโฟลเดอร์ทั้งหมดภายในโฟลเดอร์ `IT_ERROR_FIVE_SOULS_GitHub` ไปไว้ที่ root ของ Repository (รวมโฟลเดอร์ `.github` ด้วย)
3. ไปที่แท็บ **Actions**
4. เลือก workflow **Build Android APK** แล้วกด **Run workflow**
5. เมื่อทำงานสำเร็จ ดาวน์โหลดไฟล์ APK จากส่วน **Artifacts** ของ workflow

## วิธีเปิดเป็นเว็บ
ไฟล์เกมอยู่ที่ `www/index.html` สามารถเปิดด้วยเว็บเซิร์ฟเวอร์ หรือเปิด GitHub Pages โดยตั้งค่า Pages ให้ deploy จากโฟลเดอร์ `www` ไม่ได้โดยตรงในทุกการตั้งค่า; แนะนำใช้ workflow ที่ให้มาหรือคัดลอกเนื้อหา `www` ไปยัง root หากจะใช้ Pages แบบ branch

## หมายเหตุ
- เกมใช้ Three.js จาก CDN `cdnjs.cloudflare.com` จึงต้องมีอินเทอร์เน็ตขณะโหลดไลบรารีครั้งแรก
- APK จะถูกสร้างบน GitHub Actions ไม่ได้แนบ APK สำเร็จรูปมาใน ZIP นี้
- Package ID: `com.paeng.iterror`

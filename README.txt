วังหลัง: ลิขิตหงส์เหนือบัลลังก์ — เกมนิยายภาพภาษาไทย
วิธีอัปโหลด: แตก ZIP แล้วอัปโหลดไฟล์ทั้งหมด โดยให้ index.html อยู่ที่ root ของ repository
เปิด GitHub repository > Settings > Pages > Build and deployment: Deploy from a branch > เลือก main และ /(root) > Save
รอ GitHub Pages deploy แล้วเปิด URL github.io

สำคัญ: ต้องเปิดผ่าน GitHub Pages/เว็บเซิร์ฟเวอร์ เพราะเกมโหลด story.json ด้วย fetch ไม่ควรเปิด index.html จาก Files โดยตรง

โครงสร้าง:
index.html = หน้าเกม
style.css = ธีม/หน้าจอ
game.js = ระบบตัวเลือก เซฟ และตอนจบ
story.json = เนื้อเรื่อง 20 บทและตัวเลือก
assets/characters/ = ภาพตัวละคร SVG ตัวอย่าง
assets/scenes/ = ภาพฉาก SVG ตัวอย่าง
assets/ui/ = โฟลเดอร์สำรองสำหรับไอคอน/ภาพตกแต่ง
STORY_MAP.md = แผนผังเนื้อเรื่อง

เปลี่ยนภาพ: ใช้ชื่อไฟล์เดิมแทนภาพ SVG หรือแก้ path ใน game.js / ค่า scene ใน story.json ให้ตรงชื่อไฟล์ใหม่ หากใช้ PNG/JPG ต้องแก้นามสกุลใน path ด้วย
ภาพ SVG เป็น placeholder ที่สร้างขึ้นสำหรับเกม สามารถเปลี่ยนเป็นภาพของคุณเองได้
เกมมี 20 บท, 3-4 ตัวเลือกต่อบท, ค่าสถานะ, ประวัติการเลือก, หลักฐาน, เซฟ localStorage และหลายตอนจบตามค่าสถานะ

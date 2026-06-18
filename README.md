<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>My Portfolio</title>

<style>
body{
    margin:0;
    font-family: 'Segoe UI', Arial, sans-serif; /* เปลี่ยนฟอนต์ให้ดูโมเดิร์นขึ้น */
    background:linear-gradient(135deg,#0f172a,#1e293b);
    color:white;
    min-height: 100vh;
}

.container{
    max-width:900px;
    margin:auto;
    padding:30px;
}

.card{
    background:rgba(255,255,255,0.05); /* ปรับความโปร่งใสลงเล็กน้อย */
    backdrop-filter:blur(10px);
    -webkit-backdrop-filter: blur(10px); /* รองรับ Safari */
    border: 1px solid rgba(255, 255, 255, 0.1); /* เพิ่มเส้นขอบบางๆ ให้ดูเหมือนกระจกจริง */
    border-radius:20px;
    padding:25px;
    margin-bottom:20px;
    box-shadow:0 8px 32px rgba(0,0,0,0.3);
}

img{
    width:180px;
    height: 180px;
    object-fit: cover; /* ป้องกันไม่ให้รูปเบี้ยวถ้าสัดส่วนไม่ใช่สี่เหลี่ยมจัตุรัส */
    border-radius:50%;
    border:4px solid white;
}

button{
    background:#3b82f6;
    color:white;
    border:none;
    padding:12px 25px;
    border-radius:10px;
    cursor:pointer;
    font-size:16px;
    font-weight: bold;
    transition: all 0.3s ease; /* เพิ่ม Transition ให้ปุ่มนุ่มนวลขึ้น */
}

button:hover{
    background:#2563eb;
    transform: translateY(-2px); /* ลอยขึ้นเล็กน้อยตอน Hover */
}

ul{
    line-height:1.8;
}

.contact-info {
    margin-top: 15px;
    font-size: 16px;
}

.contact-info a {
    color: #3b82f6;
    text-decoration: none;
    font-weight: bold;
}

.contact-info a:hover {
    text-decoration: underline;
}
</style>

</head>
<body>

<div class="container">

    <div class="card" style="text-align:center;">
        <img src="profile.jpg" alt="Profile">
        <h1>เดชาธร คำแพง</h1>
        <p style="color: #cbd5e1;">Student | Future Programmer</p>
    </div>

    <div class="card">
        <h2>ข้อมูลส่วนตัว</h2>
        <p>กำลังศึกษาอยู่ระดับมัธยมศึกษา มีความสนใจด้านกีฬา การออกกำลังกาย และเทคโนโลยี</p>
    </div>

    <div class="card">
        <h2>ทักษะ</h2>
        <ul>
            <li>Canva (Graphic Design)</li>
            <li>HTML / CSS (Basic Web Development)</li>
        </ul>
    </div>

    <div class="card">
        <h2>งานอดิเรก</h2>
        <ul>
            <li>ฟังเพลง</li>
            <li>เล่นเกม</li>
            <li>ดูการแข่งขัน F1 (Formula 1)</li>
        </ul>
    </div>

    <div class="card" style="text-align:center;">
        <h2>ช่องทางการติดต่อ</h2>
        <button onclick="showMessage()">คลิกเพื่อทักทาย</button>
        <div class="contact-info">
            <p>Instagram: <a href="https://instagram.com/hyoyeon_7_x" target="_blank">@hyoyeon_7_x</a></p>
        </div>
    </div>

</div>

<script>
function showMessage(){
    alert("ขอบคุณที่เข้าชม Portfolio ของฉันครับ ขอให้เป็นวันที่ดีนะ!");
}
</script>

</body>
</html>

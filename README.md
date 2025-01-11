<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Bucin</title>
    <style>
        html, body {
            height: 100%;
            margin: 0;
            padding: 0;
            font-family: 'Poppins', sans-serif;
            background-color: #1a1a1a;
            color: white;
            overflow-x: hidden;
        }
        #home {
            background: url('https://th.bing.com/th/id/OIP.qI_k7pSzRGIyI40QtRuIxQHaHm?rs=1&pid=ImgDetMain') no-repeat center center fixed;
            background-size: cover;
            animation: moveBackground 30s linear infinite;
        }
        #halaman2 {
            background: url('https://i.pinimg.com/736x/d8/f9/52/d8f95249d831d5ff590cad4a1545ace4.jpg') no-repeat center center fixed;
            background-size: cover;
        }
        #halaman3 {
            background: url('https://media.suara.com/pictures/653x366/2021/12/08/32247-ilustrasi-bucin.jpg') no-repeat center center fixed;
            background-size: cover;
        }
        @keyframes moveBackground {
            0% { background-position: 0 0; }
            100% { background-position: 100% 0; }
        }
        .container {
            text-align: center;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.6);
            opacity: 0;
            animation: fadeIn 1.5s forwards;
        }
        .container.page {
            min-height: 100vh; /* Tinggi minimal 100% layar */
            padding: 40px;
            box-sizing: border-box;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }
        h1 {
            font-size: 4.5em;
            font-family: 'Great Vibes', cursive; /* Menggunakan font Great Vibes */
        }
        p {
            font-size: 1.8em;
            margin-bottom: 20px;
        }
        a {
            font-size: 1.5em;
            text-decoration: none;
            color: #ff69b4;
            font-weight: bold;
            letter-spacing: 1px;
            transition: all 0.3s ease;
        }
        a:hover {
            color: #ff1493;
            transform: translateY(-5px);
        }
        .page {
            display: none;
        }
        .show {
            display: block;
            opacity: 1;
            transition: opacity 1s ease-in-out;
        }
        @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap');
    </style>
</head>
<body>
    <div id="home" class="container page show">
        <h1>Haaiiiii LYYNNN Cantikk!</h1>
        <p>Mungkin Aku Gak Perlu Lagi Buat Kenalin Diri aku Yaaaa</p>
        <p> Aku buat ini karena ada satu hal yang ingin aku sampein sama kamu</p>
        <p>Mungkin ini sederhana, tapi isinya disini gak sederhana ;)</p>
        <p>Coba Klik yang dibawah!!!</p>
        <p><a href="javascript:void(0)" onclick="showPage('halaman2')">Hal yang tak mudah!</a></p>
    </div>
    <div id="halaman2" class="container page">
        <h1>Ini tentang Ku, dan Tentang Mu</h1>
        <p>Linnn,,,,</p>
        <p> Aku tau sebenernya buat bilang ini gak mudah</p>
        <p>Tapi karena rasa ini terlalu menggantungku,</p>
        <p>aku katakan saja hari ini</p>
        <p><a href="javascript:void(0)" onclick="playReff(); showPage('halaman3')">COBA KLIK SEKALI LAGI ;)</a></p>
    </div>
    <div id="halaman3" class="container page">
        <h1>Perasaan Aku yang tak semua orang tau</h1>
        <p>Linnn,,,,</p>
        <p>Aku tau aku masih banyak kurangnya</p>
        <p>Jika dilihat, aku tidak sesempurna laki-laki lain</p>
        <p>atau sesempurna orang yang pernah denganmu kala itu</p>
        <p> Tapi ini perasaan ku sekarang</p>
        <p> Linnnn,,,,</p>
        <p>Apakah kamu mau jadi pacarku?</p>
        <p> Untuk sekarang, besok, dan seterusnya</p>
        <p> jujur saja, aku bukan hanya sekedar suka dan sayang</p>
        <p> Tapi rasa nyaman yang ku rasakan setip harii</p>
        <p> dan itu semua aku ingin menjalaninya denganmu.</p>
        <p> aku butuh jawabanmu,</p>
        <p> dan aku akan terima semuanya.</p>
        <p> Kinggg Pramudyaaaaa</p>
        <p><a href="javascript:void(0)" onclick="showPage('home')">Kembali ke Halaman Utama</a></p>
    </div>
    <audio id="backgroundMusic" src="ANDMESH  ANUGERAH TERINDAH VIDEO LIRIK LIRIK LAGU TERBARU.mp3"></audio>
    <script>
        function showPage(pageId) {
            var pages = document.querySelectorAll('.page');
            pages.forEach(function(page) {
                page.classList.remove('show');
            });
            var pageToShow = document.getElementById(pageId);
            pageToShow.classList.add('show');
        }
        function playReff() {
            var audio = document.getElementById('backgroundMusic');
            audio.currentTime = 60; 
            audio.play();
                audio.pause();
            }, 15000);
        }
    </script>

</body>
</html>

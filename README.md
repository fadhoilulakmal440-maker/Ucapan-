[Untitled-1.html](https://github.com/user-attachments/files/26149587/Untitled-1.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Selamat Hari Raya Idul Fitri</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Amiri:ital@0;1&family=Poppins:wght@300;400;600&display=swap');

        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #013220 0%, #064e3b 100%);
            color: #fff;
            overflow: hidden;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        /* Tampilan Awal (Cover) */
        #cover {
            position: absolute;
            top: 0; left: 0; width: 100%; height: 100%;
            background-color: #013220;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            z-index: 10;
            transition: opacity 1s ease-in-out;
        }

        #cover h2 {
            color: #FFD700;
            margin-bottom: 20px;
        }

        .btn-buka {
            background-color: #FFD700;
            color: #013220;
            border: none;
            padding: 12px 30px;
            font-size: 18px;
            font-weight: 600;
            border-radius: 25px;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(255, 215, 0, 0.3);
            transition: transform 0.2s, background-color 0.2s;
        }

        .btn-buka:hover {
            transform: scale(1.05);
            background-color: #ffea75;
        }

        /* Konten Utama */
        #content {
            text-align: center;
            padding: 40px;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            border: 1px solid rgba(255, 215, 0, 0.3);
            max-width: 90%;
            width: 400px;
            opacity: 0;
            transform: translateY(30px);
            transition: all 1.5s ease;
        }

        #content.show {
            opacity: 1;
            transform: translateY(0);
        }

        .ketupat-icon {
            font-size: 50px;
            margin-bottom: 10px;
            animation: float 3s ease-in-out infinite;
        }

        h1 {
            font-family: 'Amiri', serif;
            color: #FFD700;
            font-size: 32px;
            margin-bottom: 5px;
        }

        .arabic {
            font-family: 'Amiri', serif;
            font-size: 24px;
            margin: 15px 0;
            color: #FFD700;
        }

        p {
            font-size: 16px;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        .sender {
            font-weight: 600;
            font-size: 18px;
            color: #FFD700;
            margin-top: 30px;
            text-transform: capitalize; /* Memastikan huruf awal nama menjadi kapital */
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }

        .hidden {
            display: none !important;
        }
    </style>
</head>
<body>

    <div id="cover">
        <h2>Ada pesan spesial untukmu! 🌙</h2>
        <button class="btn-buka" onclick="bukaUcapan()">Buka Pesan</button>
    </div>

    <div id="content">
        <div class="ketupat-icon">🕌</div>
        <h1>Selamat Idul Fitri</h1>
        <div class="arabic">تَقَبَّلَ اللَّهُ مِنَّا وَمِنْكُمْ</div>
        <p>1 Syawal 1447 H<br><br>Gema takbir telah berkumandang.<br>Taqabbalallahu minna wa minkum.<br>Mohon maaf lahir dan batin atas segala khilaf dan salah.</p>
        
        <div class="sender">- Fadhoilul Firdausi Akmal -</div>
    </div>

    <audio id="laguRaya" loop>
        <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    </audio>

    <script>
        function bukaUcapan() {
            // Sembunyikan cover
            document.getElementById('cover').style.opacity = '0';
            
            // Putar musik
            var audio = document.getElementById('laguRaya');
            audio.play();

            setTimeout(function() {
                document.getElementById('cover').classList.add('hidden');
                
                // Munculkan konten dengan animasi
                var content = document.getElementById('content');
                content.classList.add('show');
            }, 1000); // Menunggu animasi fade-out selesai
        }
    </script>

</body>
</html>

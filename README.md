[index.html](https://github.com/user-attachments/files/26149659/index.html)
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ucapan Idul Fitri - Fadhoilul Firdausi Akmal</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&family=Great+Vibes&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-blue: #1e3a8a;
            --gold: #d4af37;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #eff6ff 0%, #bfdbfe 100%);
            overflow-x: hidden;
        }

        .arabic-text {
            font-family: 'Amiri', serif;
        }

        .cursive {
            font-family: 'Great+Vibes', cursive;
        }

        .glass-morphism {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.3);
            box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.15);
        }

        .lantern {
            animation: swing 3s ease-in-out infinite;
            transform-origin: top center;
        }

        @keyframes swing {
            0% { transform: rotate(-5deg); }
            50% { transform: rotate(5deg); }
            100% { transform: rotate(-5deg); }
        }

        .fade-in {
            animation: fadeIn 1.5s ease-out forwards;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .star {
            position: absolute;
            background: var(--gold);
            border-radius: 50%;
            opacity: 0.5;
            animation: twinkle 2s infinite ease-in-out;
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.2); }
        }

        #overlay {
            position: fixed;
            inset: 0;
            background: linear-gradient(135deg, #1e3a8a 0%, #172554 100%);
            z-index: 100;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            transition: opacity 0.8s ease;
        }

        .envelope-button {
            background: var(--gold);
            padding: 1rem 2.5rem;
            border-radius: 9999px;
            font-weight: 600;
            transition: all 0.3s;
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);
        }

        .envelope-button:hover {
            transform: scale(1.05);
            background: #b8962d;
        }
    </style>
</head>
<body class="min-h-screen flex items-center justify-center p-4 sm:p-8">

    <!-- Overlay Opening -->
    <div id="overlay">
        <div class="mb-8 text-center px-4">
            <svg class="w-24 h-24 text-yellow-400 mx-auto mb-4 lantern" viewBox="0 0 24 24" fill="currentColor">
                <path d="M12,2L10,4H14L12,2M8,5V7H16V5H8M6,8V18H18V8H6M9,10H15V16H9V10M11,12V14H13V12H11M8,19V21H16V19H8Z" />
            </svg>
            <h2 class="text-2xl font-bold mb-2">Ada Pesan Spesial Untukmu</h2>
            <p class="text-blue-200 opacity-80">Dari Fadhoilul Firdausi Akmal</p>
        </div>
        <button onclick="openCard()" class="envelope-button">Buka Pesan</button>
    </div>

    <!-- Background Stars -->
    <div id="star-container" class="fixed inset-0 pointer-events-none"></div>

    <!-- Main Card Content -->
    <main id="main-content" class="max-w-2xl w-full glass-morphism rounded-3xl overflow-hidden relative opacity-0">
        <!-- Corner Decorations -->
        <div class="absolute top-0 right-0 p-4">
            <svg class="w-16 h-16 text-blue-800 opacity-20" viewBox="0 0 100 100" fill="currentColor">
                <path d="M0,0 L100,0 L100,100 Z" />
            </svg>
        </div>

        <div class="p-8 sm:p-12 text-center relative z-10">
            <!-- Header Icons -->
            <div class="flex justify-center space-x-4 mb-6">
                <svg class="w-10 h-10 text-blue-800 lantern" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12,2L10,4H14L12,2M8,5V7H16V5H8M6,8V18H18V8H6M9,10H15V16H9V10M11,12V14H13V12H11M8,19V21H16V19H8Z" />
                </svg>
                <div class="text-blue-900">
                    <svg class="w-12 h-12" viewBox="0 0 24 24" fill="currentColor">
                        <path d="M12,2C12,2 14,5.46 14,9C14,11.21 12.21,13 10,13C7.79,13 6,11.21 6,9C6,5.46 8,2 8,2C8,2 2,2 2,12C2,17.5 6.5,22 12,22C17.5,22 22,17.5 22,12C22,2 12,2 12,2Z" />
                    </svg>
                </div>
                <svg class="w-10 h-10 text-blue-800 lantern" style="animation-delay: 0.5s" viewBox="0 0 24 24" fill="currentColor">
                    <path d="M12,2L10,4H14L12,2M8,5V7H16V5H8M6,8V18H18V8H6M9,10H15V16H9V10M11,12V14H13V12H11M8,19V21H16V19H8Z" />
                </svg>
            </div>

            <h3 class="arabic-text text-4xl sm:text-5xl mb-6 text-blue-900 font-bold">تَقَبَّلَ اللهُ مِنَّا وَمِنْكُمْ</h3>
            <p class="text-sm text-blue-700 italic mb-8">"Taqabbalallahu Minna wa Minkum"</p>
            
            <h1 class="cursive text-5xl sm:text-6xl text-yellow-500 mb-4">Selamat Hari Raya</h1>
            <h2 class="text-2xl sm:text-3xl font-bold text-blue-900 mb-6 uppercase tracking-widest">Idul Fitri 1 Syawal 1447 H</h2>
            
            <div class="w-24 h-1 bg-gradient-to-r from-blue-400 to-blue-600 mx-auto mb-8 rounded-full"></div>

            <div class="space-y-4 text-blue-800 leading-relaxed mb-10 max-w-lg mx-auto text-sm sm:text-base text-justify text-left">
                <p>"Ing sawingkingipun layar pagesangan, boten sedanten adegan mlampah jumbuh kaliyan naskah. Wonten kalaning wicanten kita boten <em>in-sync</em>, wonten wekdalipun tumindak kula kraos <em>out of frame</em>, saha mbok bilih wonten pitembungan ingkang nate <em>distorsi</em> ing talingan."</p>
                <p>Mapag dinten ingkang fitri punika, kula <strong>Fadhoilul Firdausi Akmal</strong> badhe nindakaken <em>final render</em> dhumateng manah kita. Sumangga kita busak sedaya <em>noise</em> kalepatan lan wangsul ing frekuensi kesucian.</p>
                <div class="pt-4 text-center">
                    <p class="font-bold text-lg sm:text-xl text-blue-900">Nyuwun pangapunten lair lan batin saking sedaya kalepatan.</p>
                    <p class="text-sm mt-3 italic">"Mugi-mugi silaturahmi kita tansah sambung kaliyan sinyal ingkang kiyat saha kebak ing berkah."</p>
                </div>
            </div>

            <div class="bg-gradient-to-r from-blue-900 to-blue-800 text-white py-6 px-8 rounded-2xl inline-block shadow-lg">
                <p class="text-xs uppercase tracking-widest opacity-70 mb-1">Salam Hangat Dari</p>
                <p class="text-xl font-bold tracking-wide">Fadhoilul Firdausi Akmal</p>
                <p class="text-xs mt-1 text-blue-300">& Keluarga</p>
            </div>
        </div>

        <!-- Footer Pattern -->
        <div class="h-4 bg-gradient-to-r from-blue-900 via-blue-400 to-blue-900"></div>
    </main>

    <!-- Music Takbiran Idul Fitri -->
    <audio id="eidMusic" loop>
        <!-- Menggunakan audio takbiran dari Internet Archive -->
        <source src="https://archive.org/download/takbir-syaikh-abdul-karim-al-makki/takbir-syaikh-abdul-karim-al-makki.mp3" type="audio/mpeg">
        <source src="https://archive.org/download/TakbiranIdulFitri1433H/Takbiran%20Idul%20Fitri%201433%20H.mp3" type="audio/mpeg">
    </audio>

    <script>
        // Create stars background
        const starContainer = document.getElementById('star-container');
        for (let i = 0; i < 50; i++) {
            const star = document.createElement('div');
            star.className = 'star';
            const size = Math.random() * 3 + 1;
            star.style.width = `${size}px`;
            star.style.height = `${size}px`;
            star.style.left = `${Math.random() * 100}vw`;
            star.style.top = `${Math.random() * 100}vh`;
            star.style.animationDelay = `${Math.random() * 2}s`;
            starContainer.appendChild(star);
        }

        function openCard() {
            const overlay = document.getElementById('overlay');
            const mainContent = document.getElementById('main-content');
            const audio = document.getElementById('eidMusic');

            overlay.style.opacity = '0';
            setTimeout(() => {
                overlay.style.display = 'none';
                mainContent.classList.add('fade-in');
            }, 800);

            // Memutar mp3 lagu idul fitri / takbiran ketika tombol ditekan
            if (audio) {
                audio.play().catch(e => console.log("Audio autoplay prevented", e));
            }
        }

        // Detect window resize to ensure layout stays clean
        window.addEventListener('resize', () => {
            // Re-adjust stars if needed
        });
    </script>
</body>
</html>

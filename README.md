
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Muhammad Naufal Ardhi Zaidan</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000; /* Background belakang hitam */
            color: #fff; /* Teks putih untuk kontras */
            line-height: 1.6;
            overflow: hidden; /* Mencegah scroll karena background animasi */
        }
        .dragon-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 200px; /* Ukuran naga besar */
            animation: rotate 10s linear infinite; /* Animasi berputar */
            opacity: 0.1; /* Transparan agar tidak mengganggu konten */
        }
        @keyframes rotate {
            from {
                transform: rotate(0deg);
            }
            to {
                transform: rotate(360deg);
            }
        }
        .container {
            max-width: 900px;
            margin: 20px auto;
            padding: 30px;
            background-color: rgba(255, 255, 255, 0.05); /* Semi-transparan untuk efek glow */
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(102, 126, 234, 0.5), 0 0 40px rgba(118, 75, 162, 0.3); /* Glow effect */
            overflow: hidden;
            animation: glow 2s ease-in-out infinite alternate; /* Animasi glow */
            position: relative;
            z-index: 1; /* Di atas background */
        }
        @keyframes glow {
            from {
                box-shadow: 0 0 20px rgba(102, 126, 234, 0.5), 0 0 40px rgba(118, 75, 162, 0.3);
            }
            to {
                box-shadow: 0 0 30px rgba(102, 126, 234, 0.8), 0 0 60px rgba(118, 75, 162, 0.5);
            }
        }
        header {
            text-align: center;
            padding: 50px 20px;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            border-radius: 10px 10px 0 0;
            animation: blink 1.5s infinite; /* Animasi berkedip pada header */
        }
        @keyframes blink {
            0%, 50% {
                opacity: 1;
            }
            51%, 100% {
                opacity: 0.7;
            }
        }
        header h1 {
            margin: 0;
            font-size: 3em;
            font-weight: 300;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.8); /* Glow pada teks */
        }
        header p {
            margin: 10px 0 0;
            font-size: 1.3em;
            opacity: 0.9;
        }
        section {
            padding: 30px 20px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }
        section:last-of-type {
            border-bottom: none;
        }
        section h2 {
            color: #667eea;
            font-size: 2em;
            margin-bottom: 15px;
            font-weight: 400;
            text-shadow: 0 0 5px rgba(102, 126, 234, 0.5); /* Subtle glow pada heading */
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            margin: 10px 0;
            padding-left: 25px;
            position: relative;
            font-size: 1.1em;
        }
        ul li:before {
            content: '▸';
            color: #667eea;
            font-weight: bold;
            position: absolute;
            left: 0;
            font-size: 1.2em;
        }
        .experience li {
            background-color: rgba(255, 255, 255, 0.1);
            padding: 15px;
            border-radius: 5px;
            margin-bottom: 10px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        .contact {
            text-align: center;
        }
        .contact p {
            margin: 10px 0;
            font-size: 1.1em;
        }
        .contact a {
            color: #667eea;
            text-decoration: none;
            font-weight: 500;
        }
        .contact a:hover {
            text-decoration: underline;
        }
        .rainbow-blink {
            animation: rainbow-blink 2s infinite; /* Animasi berkedip warna warni */
        }
        @keyframes rainbow-blink {
            0% { color: #ff0000; opacity: 1; }
            16% { color: #ff8000; opacity: 0.8; }
            33% { color: #ffff00; opacity: 1; }
            50% { color: #00ff00; opacity: 0.8; }
            66% { color: #0080ff; opacity: 1; }
            83% { color: #8000ff; opacity: 0.8; }
            100% { color: #ff0000; opacity: 1; }
        }
    </style>
</head>
<body>
    <div class="dragon-bg">🐉</div> <!-- Naga yang berputar di background -->
    <div class="container">
        <header>
            <h1>Muhammad Naufal Ardhi Zaidan</h1>
            <p>crew store</p>
        </header>
        
        <section id="tentang-saya">
            <h2>Tentang Saya</h2>
            <p>Saya adalah individu yang antusias dan berkomitmen untuk terus belajar dan berkembang. Dengan latar belakang yang beragam, saya berusaha untuk menggabungkan pengetahuan teknis dan keterampilan praktis dalam berbagai bidang.</p>
        </section>
        
        <section id="pendidikan">
            <h2>Pendidikan</h2>
            <ul>
                <li>SMKN 7 Kota Bekasi</li>
            </ul>
        </section>
        
        <section id="pengalaman-kerja">
            <h2>Pengalaman Kerja</h2>
            <ul class="experience">
                <li>Magang PKL di PT Gagana Megah Utama (Mei 2023 - Nov 2023)</li>
                <li>PT Sumber Alfaria Trijaya Tbk (16 Okt 2024 - 16 Okt 2025)</li>
            </ul>
        </section>
        
        <section id="keahlian">
            <h2>Keahlian</h2>
            <ul>
                <li>Programmer Basic</li>
                <li>Dasar Elektro</li>
                <li>MS Excel</li>
                <li>MS Word</li>
                <li>Kasir / Pramu</li>
            </ul>
        </section>
        
        <section id="hobi">
            <h2>Hobi</h2>
            <ul>
                <li>Membaca Buku</li>
                <li>Olahraga</li>
            </ul>
        </section>
        
        <section id="kontak" class="contact">
            <h2>Kontak</h2>
            <p><strong>Telepon:</strong> <a href="https://wa.me/628972317715" target="_blank">08972317715 (Chat WhatsApp)</a></p>
            <p><strong>Email:</strong> <a href="mailto:m.naufalardhiz@gmail.com">m.naufalardhiz@gmail.com</a></p>
            <p class="rainbow-blink"><strong>Alamat:</strong> Jl Swadaya 1 No 16 B, Kec Pondok Gede, Kel Jati Makmur, Kota Bekasi</p>
        </section>
    </div>
</body>
</html>

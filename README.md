          <!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portofolio Kerja - [muhammad naufal ardhi zaidan]</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); /* Latar belakang gradien yang bagus */
            color: #fff;
            line-height: 1.6;
        }
        header {
            text-align: center;
            padding: 50px 20px;
            background: rgba(0, 0, 0, 0.5);
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        header p {
            font-size: 1.2em;
            margin: 10px 0;
        }
        section {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
        }
        h2 {
            border-bottom: 2px solid #fff;
            padding-bottom: 10px;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            margin: 10px 0;
        }
        footer {
            text-align: center;
            padding: 20px;
            background: rgba(0, 0, 0, 0.5);
        }
        @media (max-width: 600px) {
            header h1 {
                font-size: 2em;
            }
            section {
                margin: 10px;
                padding: 15px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>[muhammad naufal ardhi zaidan]</h1>
        <p>pelayanan & pemasaran</p>
    </header>

    <section id="data-pribadi">
        <h2>Data Pribadi</h2>
        <p><strong>Nama:</strong> [muhammad naufal ardhi zaidan]</p>
        <p><strong>Tempat/Tanggal Lahir:</strong> [bekasi, 07/08/2006]</p>
        <p><strong>Alamat:</strong> [jl swadaya no 16 b rt 010/rw 008 kec pondok gede kel jatimakmur kota bekasi]</p>
        <p><strong>Status:</strong> [belum menikah]</p>
    </section>

    <section id="kontak">
        <h2>Kontak</h2>
        <ul>
            <li><strong>Email:</strong> [m.naufalardhiz@gmail.com]</li>
            <li><strong>Telepon:</strong> [08972317715]</li>
            <li><strong>LinkedIn:</strong> <a href="[https://www.linkedin.com/in/muhammad-n-8bb292309]" target="_blank" style="color: #fff;">[Nama Profil LinkedIn]</a></li>
            <li><strong>GitHub:</strong> <a href="[https://mnaufalardhiz-cyber.github.io/PORTOFOLIO-naufal--/]" target="_blank" style="color: #fff;">[Nama Profil GitHub]</a></li>
        </ul>
    </section>

    <section id="pendidikan">
        <h2>Pendidikan</h2>
        <ul>
            <li><strong>[2021 - 2024]:</strong> [smkn 7 kota bekasi], [teknik elektro]</li>
            
            <!-- Tambahkan lebih banyak jika diperlukan -->
        </ul>
    </section>

    <section id="keahlian">
        <h2>Keahlian</h2>
        <ul>
            <li>HTML, CSS, JavaScript</li>
            <li>kerja sama team</li>
            <li>komunikasi</li>
            <li>transaksi kasir</li>
            <li>berpikir kritis</li>
            <!-- Tambahkan keahlian Anda -->
        </ul>
    </section>

    <footer>
        <p>&copy; 2023 [muhammad naufal ardhi zaidan]. Semua hak dilindungi.</p>
    </footer>

    <script>
        // Script sederhana untuk animasi scroll (opsional)
        window.addEventListener('scroll', function() {
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                const rect = section.getBoundingClientRect();
                if (rect.top < window.innerHeight && rect.bottom > 0) {
                    section.style.opacity = '1';
                    section.style.transform = 'translateY(0)';
                } else {
                    section.style.opacity = '0';
                    section.style.transform = 'translateY(20px)';
                }
            });
        });
        // Inisialisasi opacity awal
        document.querySelectorAll('section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(20px)';
            section.style.transition = 'opacity 0.5s, transform 0.5s';
        });
    </script>
</body>
</html>

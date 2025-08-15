<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Travel & Tour - PT Liburan Asik</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      line-height: 1.6;
    }
    header {
      background: #008080;
      color: white;
      padding: 15px 0;
    }
    header nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      max-width: 1100px;
      margin: auto;
      padding: 0 20px;
    }
    header nav a {
      color: white;
      text-decoration: none;
      margin: 0 10px;
      font-weight: bold;
    }
    .hero {
      background: url('https://source.unsplash.com/1600x600/?travel,beach') center/cover no-repeat;
      color: white;
      height: 400px;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 20px;
    }
    .hero h1 {
      font-size: 48px;
      background: rgba(0,0,0,0.5);
      padding: 10px 20px;
      border-radius: 10px;
    }
    section {
      max-width: 1100px;
      margin: auto;
      padding: 40px 20px;
    }
    .packages {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }
    .card {
      border: 1px solid #ddd;
      border-radius: 10px;
      overflow: hidden;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .card-body {
      padding: 15px;
    }
    .card-body h3 {
      margin: 0 0 10px;
      color: #008080;
    }
    .btn {
      display: inline-block;
      padding: 10px 15px;
      background: #008080;
      color: white;
      text-decoration: none;
      border-radius: 5px;
    }
    .about, .contact {
      background: #f9f9f9;
      border-radius: 10px;
      padding: 20px;
    }
    form input, form textarea {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      padding: 10px 15px;
      background: #008080;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    footer {
      text-align: center;
      padding: 15px;
      background: #222;
      color: white;
      margin-top: 30px;
    }
  </style>
</head>
<body>
  <header>
    <nav>
      <div class="logo"><h2>PT Liburan Asik</h2></div>
      <div class="menu">
        <a href="#home">Beranda</a>
        <a href="#packages">Paket Tour</a>
        <a href="#about">Tentang</a>
        <a href="#contact">Kontak</a>
      </div>
    </nav>
  </header>

  <section class="hero" id="home">
    <h1>Jelajahi Dunia Bersama Kami</h1>
  </section>

  <section id="packages">
    <h2>Paket Tour Terpopuler</h2>
    <div class="packages">
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?bali,beach" alt="Bali">
        <div class="card-body">
          <h3>Bali Paradise</h3>
          <p>5 Hari 4 Malam menikmati pantai dan budaya Bali.</p>
          <a href="#contact" class="btn">Pesan Sekarang</a>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?japan,city" alt="Japan">
        <div class="card-body">
          <h3>Japan Explorer</h3>
          <p>7 Hari wisata kota Tokyo, Kyoto, dan Osaka.</p>
          <a href="#contact" class="btn">Pesan Sekarang</a>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?paris,eiffel" alt="Paris">
        <div class="card-body">
          <h3>Romantic Paris</h3>
          <p>4 Hari menikmati kota romantis Paris dan sekitarnya.</p>
          <a href="#contact" class="btn">Pesan Sekarang</a>
        </div>
      </div>
    </div>
  </section>

  <section id="about" class="about">
    <h2>Tentang Kami</h2>
    <p>PT Liburan Asik telah berpengalaman lebih dari 10 tahun menyediakan paket wisata terbaik di seluruh dunia. Dengan tim profesional dan harga terjangkau, kami berkomitmen memberikan pengalaman liburan yang tak terlupakan.</p>
  </section>

  <section id="contact" class="contact">
    <h2>Hubungi Kami</h2>
    <form>
      <input type="text" placeholder="Nama Lengkap" required>
      <input type="email" placeholder="Email" required>
      <input type="tel" placeholder="Nomor Telepon" required>
      <textarea rows="5" placeholder="Pesan Anda"></textarea>
      <button type="submit">Kirim</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 PT Liburan Asik. Semua Hak Dilindungi.</p>
  </footer>
</body>
</html>

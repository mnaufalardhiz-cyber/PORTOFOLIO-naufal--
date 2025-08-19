<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Portofolio – Naufal | Crew Store • Kasir • Desain</title>
  <meta name="description" content="Portofolio kerja Naufal: pengalaman Crew Store, keahlian kasir dan desain. Siap bekerja profesional dan berorientasi pada pelayanan pelanggan." />
  <style>
    :root{
      --bg:#0f172a;      /* slate-900 */
      --card:#111827;    /* gray-900 */
      --muted:#94a3b8;   /* slate-400 */
      --text:#e5e7eb;    /* gray-200 */
      --brand:#ef4444;   /* red-500 */
      --brand-2:#f59e0b; /* amber-500 */
      --ring:#22d3ee;    /* cyan-400 */
      --shadow:0 10px 30px rgba(0,0,0,.35);
      --radius:18px;
    }
    *{box-sizing:border-box}
    html,body{margin:0;background:linear-gradient(180deg,var(--bg),#0b1220);color:var(--text);font:16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji"}
    a{color:inherit}
    .container{max-width:1050px;margin-inline:auto;padding:24px}
    header.hero{position:relative;border-radius:var(--radius);padding:32px 28px;background:radial-gradient(1200px 400px at 15% 0%, rgba(239,68,68,.18), transparent 60%),
      radial-gradient(900px 300px at 85% 20%, rgba(245,158,11,.18), transparent 60%),
      linear-gradient(180deg,#101827, #0e1625);box-shadow:var(--shadow);overflow:hidden}
    .hero-top{display:flex;gap:20px;align-items:center;flex-wrap:wrap}
    .avatar{width:110px;height:110px;border-radius:20px;background:#1f2937;border:1px solid #374151;display:grid;place-items:center;color:#9ca3af;font-weight:700;letter-spacing:.5px}
    .title h1{margin:0;font-size:clamp(28px,4vw,40px)}
    .title p{margin:6px 0 0;color:var(--muted)}
    .badges{display:flex;flex-wrap:wrap;gap:10px;margin-top:14px}
    .badge{background:rgba(239,68,68,.12);border:1px solid rgba(239,68,68,.35);color:#fecaca;padding:6px 10px;border-radius:999px;font-weight:600;font-size:14px}
    .actions{margin-left:auto;display:flex;gap:10px}
    .btn{appearance:none;border:0;border-radius:12px;padding:10px 14px;font-weight:700;cursor:pointer;background:#1f2937;color:#e5e7eb;border:1px solid #334155;transition:.2s box-shadow,.2s transform}
    .btn:hover{box-shadow:0 0 0 3px rgba(34,211,238,.25)}
    .btn.primary{background:linear-gradient(180deg,#ef4444,#b91c1c);border:0}

    .grid{display:grid;gap:22px;margin-top:22px}
    @media(min-width:860px){.grid{grid-template-columns:2fr 1fr}}

    .card{background:linear-gradient(180deg,#0f172a,#0b1220);border:1px solid #1f2937;border-radius:var(--radius);padding:22px;box-shadow:var(--shadow)}
    .card h2{margin:0 0 14px;font-size:22px}
    .muted{color:var(--muted)}
    .timeline{position:relative;margin:0;padding:0;list-style:none}
    .timeline::before{content:"";position:absolute;left:14px;top:0;bottom:0;width:2px;background:#1f2937}
    .timeline li{position:relative;padding-left:42px;margin:18px 0}
    .timeline li::before{content:"";position:absolute;left:7px;top:.25rem;width:16px;height:16px;border-radius:50%;background:var(--brand);box-shadow:0 0 0 3px rgba(239,68,68,.25)}
    .pill{display:inline-block;padding:6px 10px;border-radius:999px;border:1px solid #374151;background:#0b1220;margin:6px 8px 0 0}

    .skills{display:flex;flex-wrap:wrap;gap:10px}
    .skill{flex:1 1 180px;background:#0b1220;border:1px solid #1f2937;border-radius:14px;padding:14px}
    .skill h3{margin:0 0 6px;font-size:16px}
    .meter{height:8px;border-radius:999px;background:#111827;border:1px solid #1f2937;overflow:hidden}
    .meter > span{display:block;height:100%;background:linear-gradient(90deg,var(--brand),var(--brand-2));width:0}

    .projects{display:grid;grid-template-columns:repeat(12,1fr);gap:14px}
    .project{grid-column:span 6;background:#0b1220;border:1px solid #1f2937;border-radius:14px;padding:14px}
    @media(max-width:680px){.project{grid-column:span 12}}

    footer{opacity:.8;text-align:center;margin:26px 0;color:var(--muted)}
    .sep{height:1px;background:#1f2937;margin:18px 0}

    @media print{
      body{background:#fff;color:#111}
      header.hero, .card{box-shadow:none;background:#fff;border:1px solid #ddd}
      .btn, .actions, .avatar{display:none}
      .badge{border:1px solid #999;color:#000;background:#eee}
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="hero">
      <div class="hero-top">
        <div class="avatar">FOTO</div>
        <div class="title">
          <h1>Naufal</h1>
          <p>Profesional retail dengan pengalaman <strong>Crew Store</strong>. Memiliki keahlian utama sebagai <strong>Kasir</strong> dan <strong>Desain</strong> (grafis & konten), berorientasi pada layanan pelanggan dan efisiensi operasional.</p>
          <div class="badges">
            <span class="badge">Crew Store</span>
            <span class="badge">Kasir</span>
            <span class="badge">Desain</span>
          </div>
        </div>
        <div class="actions">
          <button class="btn" onclick="window.print()">Unduh / Cetak PDF</button>
          <a class="btn primary" href="#kontak">Hubungi Saya</a>
        </div>
      </div>
    </header>

    <section class="grid">
      <article class="card">
        <h2>Ringkasan</h2>
        <p class="muted">Terbiasa mengelola transaksi kasir yang akurat, menjaga display barang, stok, dan kebersihan area. Mampu membuat materi visual sederhana untuk promo toko (poster, feed, banner) serta dokumentasi produk. Cepat belajar sistem baru dan nyaman bekerja dalam target.</p>
        <div class="sep"></div>
        <h2>Pengalaman Kerja</h2>
        <ul class="timeline">
          <li>
            <h3>Crew Store (Retail Minimarket)</h3>
            <div class="muted">2023 – 2025</div>
            <p>Menangani transaksi di kasir, memastikan akurasi uang masuk/keluar, rekap harian, serta pelayanan pelanggan yang ramah. Melakukan penataan display, FIFO/FEFO, cek tanggal kedaluwarsa, dan stock opname berkala.</p>
            <div>
              <span class="pill">Pelayanan Pelanggan</span>
              <span class="pill">Cash Handling</span>
              <span class="pill">Stock & Display</span>
              <span class="pill">Kebersihan Area</span>
            </div>
          </li>
          <li>
            <h3>Desain Konten Toko (Freelance Internal)</h3>
            <div class="muted">2024 – 2025</div>
            <p>Membuat materi promosi mingguan: poster, banner, konten media sosial. Adaptif terhadap brief, konsisten dengan identitas merek, dan siap produksi cepat.</p>
            <div>
              <span class="pill">Poster & Banner</span>
              <span class="pill">Konten Instagram</span>
              <span class="pill">Foto Produk</span>
              <span class="pill">Canva / Photoshop</span>
            </div>
          </li>
        </ul>
      </article>

      <aside class="card">
        <h2>Data Singkat</h2>
        <p><strong>Nama:</strong> Naufal</p>
        <p><strong>Domisili:</strong> Indonesia</p>
        <p><strong>Status:</strong> Siap bergabung segera</p>
        <div class="sep"></div>
        <h2>Keahlian Utama</h2>
        <div class="skills">
          <div class="skill">
            <h3>Kasir & Operasional</h3>
            <div class="meter"><span style="width:88%"></span></div>
            <p class="muted">POS, scanning, rekap kas, retur, voucher, penanganan komplain, SOP layanan.</p>
          </div>
          <div class="skill">
            <h3>Desain</h3>
            <div class="meter"><span style="width:78%"></span></div>
            <p class="muted">Canva, dasar Photoshop, tipografi & layout, konten media sosial.</p>
          </div>
          <div class="skill">
            <h3>Administrasi</h3>
            <div class="meter"><span style="width:72%"></span></div>
            <p class="muted">Ms. Excel/Spreadsheet, pencatatan stok, laporan harian.</p>
          </div>
        </div>
        <div class="sep"></div>
        <h2>Bahasa</h2>
        <p>Indonesia (aktif), Inggris (pasif/menengah)</p>
      </aside>
    </section>

    <section class="card">
      <h2>Contoh Proyek Desain</h2>
      <div class="projects">
        <div class="project">
          <strong>Poster Promo Mingguan</strong>
          <p class="muted">Desain poster diskon produk utama, format A3 & feed IG.</p>
        </div>
        <div class="project">
          <strong>Banner Spanduk Event</strong>
          <p class="muted">Spanduk event toko (Grand Opening / Payday Sale).</p>
        </div>
        <div class="project">
          <strong>Feed & Story Template</strong>
          <p class="muted">Template konsisten brand untuk pengumuman promo.</p>
        </div>
        <div class="project">
          <strong>Foto & Editing Produk</strong>
          <p class="muted">Foto sederhana dengan pencahayaan natural + retouch ringan.</p>
        </div>
      </div>
    </section>

    <section id="kontak" class="card">
      <h2>Kontak</h2>
      <p>Siap dipanggil interview. Silakan hubungi melalui:</p>
      <ul>
        <li><strong>WhatsApp:</strong> 089508293502</li>
        <li><strong>Email:</strong> m.naufalardhiz@gmail.com</li>
        <li><strong>Instagram/Portofolio:</strong> @hansi_fal (opsional)</li>
      </ul>
    </section>

    <footer>
      © <span id="y"></span> Naufal • Portofolio Kerja (Crew Store • Kasir • Desain)
    </footer>
  </div>
  <script>
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>

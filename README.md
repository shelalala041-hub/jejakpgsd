# jejakpgsd
web ini akan membantu mahasiswa pgsd tahu SD/MI mana yang sedang dikunjungi
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jejak PGSD</title>
  <link rel="stylesheet" href="style.css">
  <link rel="icon" href="logo.svg" type="image/svg+xml">
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.3/dist/leaflet.css" />
</head>
<body>
  <header>
    <img src="logo.svg" alt="Logo Jejak PGSD" class="logo">
    <h1>Jejak PGSD</h1>
    <p>Catat dan pantau kunjungan SD oleh mahasiswa PGSD</p>
  </header>
  <main>
    <section id="map-section">
      <div id="map"></div>
    </section>
    <section id="form-section">
      <h2>Isi Data Kunjungan SD</h2>
      <form id="visit-form" autocomplete="off">
        <label>Nama SD:
          <input type="text" name="nama_sd" required>
        </label>
        <label>Alamat SD:
          <input type="text" name="alamat_sd" required>
        </label>
        <label>Nama Mahasiswa:
          <input type="text" name="nama_mahasiswa" required>
        </label>
        <label>Tanggal Kunjungan:
          <input type="date" name="tanggal_kunjungan" required>
        </label>
        <label>Deskripsi/ Catatan Kunjungan:
          <textarea name="catatan" required></textarea>
        </label>
        <label>Lokasi SD (klik di peta):
          <input type="text" name="lokasi" id="lokasi" readonly required>
        </label>
        <button type="submit">Simpan Kunjungan</button>
      </form>
    </section>
    <section id="list-section">
      <h2>Daftar SD yang Dikunjungi</h2>
      <ul id="kunjungan-list"></ul>
    </section>
  </main>
  <footer>
    <small>&copy; 2025 Jejak PGSD</small>
  </footer>
  <script src="https://unpkg.com/leaflet@1.9.3/dist/leaflet.js"></script>
  <script src="script.js"></script>
</body>
</html>

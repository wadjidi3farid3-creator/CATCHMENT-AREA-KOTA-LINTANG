KML UNIVERSAL WEBGIS INTEGRATED v1.4

PUBLIKASI GITHUB PAGES
1. Upload seluruh isi folder terpadu_WEBGIS_v1_4 ke repository GitHub.
2. Pastikan index.html berada di root folder publik dan folder DATA sejajar dengannya.
3. Pastikan DATA/sumber.kml ikut diunggah.
4. Aktifkan GitHub Pages melalui Settings > Pages.
5. Buka URL Pages yang disediakan GitHub. Jangan membuka index.html langsung melalui file://.

MEKANISME PEMUATAN
- DATA/sumber.kml dimuat otomatis saat index.html dibuka.
- Tidak perlu menekan tombol Tambah Layer untuk memuat sumber awal.
- Tombol Tambah Layer KML/KMZ digunakan untuk file tambahan melalui URL HTTP(S).
- URL sumber yang sama dicegah agar tidak dimuat dua kali dalam satu sesi halaman.

ISI PAKET
- index.html: aplikasi WebGIS
- DATA/sumber.kml: file KML sumber asli, terpisah dari HTML
- manifest.json: metadata paket dan CRS
- README.txt: petunjuk publikasi

FITUR
- Google Hybrid dan Google Satellite
- Zoom + / - kanan atas
- Zoom Seluruh Data, Lokasi Saya, Tambah Layer, Panel Layer kiri bawah
- Struktur Folder KML bersarang ditampilkan sebagai hierarki
- Checkbox tampil/sembunyi dan hapus layer dari tampilan
- Pembaca KMZ di browser dengan doc.kml diprioritaskan
- Tidak menyediakan tombol/fungsi Simpan atau Simpan Sebagai

SISTEM KOORDINAT
- WGS 84 / EPSG:4326
- KML: longitude,latitude[,altitude]
- GeoJSON: [longitude, latitude]
- Leaflet: [latitude, longitude]
- Validasi longitude -180..180 dan latitude -90..90

CATATAN
- Untuk layer tambahan, gunakan URL raw.githubusercontent.com atau URL GitHub Pages.
- URL halaman github.com/blob/... bukan URL file KML mentah.
- Pemuatan lintas domain bergantung pada izin CORS server sumber.
- Pemuatan file relatif tidak berjalan jika index.html dibuka langsung dengan file://.
- Basemap Google menggunakan endpoint tile yang bukan integrasi resmi Google Maps Platform; akses dapat berubah atau dibatasi.
- Lokasi Saya memerlukan HTTPS dan izin lokasi browser/perangkat.

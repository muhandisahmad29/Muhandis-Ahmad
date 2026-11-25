# Portofolio Muhandis Ahmad

Website personal portfolio statis (satu file HTML, tanpa build dan tanpa library). Tema dark cinematic dengan aksen silver dan cool blue.

## Struktur

```
portofolio-muhandis/
├── index.html          # seluruh website (HTML, CSS, JavaScript)
├── assets/
│   ├── video/          # taruh video hero dan video karya (MP4)
│   └── img/            # taruh foto profil dan gambar poster
├── .gitignore
└── README.md
```

## Menjalankan di komputer

Buka `index.html` dengan browser (klik dua kali). Tidak perlu instalasi apa pun. Font dimuat dari Google Fonts, jadi butuh internet agar tampil sesuai desain.

## Mengisi aset

Semua slot sudah disiapkan di `index.html`. Cari komentar HTML yang menyebutnya, lalu isi atribut `src`.

| Slot | Contoh isi |
|---|---|
| Video hero | `<video class="hv" ... src="assets/video/hero.mp4" poster="assets/img/hero.jpg">` |
| Foto profil hero | `<img src="assets/img/foto-profil.jpg" alt="Portrait of Muhandis Ahmad">` |
| Foto di About | `<img src="assets/img/foto-about.jpg" alt="Portrait of Muhandis Ahmad Basyasya">` |
| Video karya | `<video controls preload="none" playsinline src="assets/video/karya1.mp4" poster="assets/img/karya1.jpg">` |
| YouTube | isi `href` pada `<a id="yt">` lalu hapus atribut `hidden` |

Begitu `src` terisi, placeholder hilang otomatis. Saran video hero: MP4 H.264, 720p sampai 1080p, 10 sampai 20 detik, tanpa suara, di bawah 8 MB. Tambahkan `poster` pada video karya agar kotaknya tidak hitam sebelum diputar.

## Catatan

- Menu EXPERIENCE dan tombol EXPLORE MY JOURNEY sementara mengarah ke bagian About karena belum ada section Experience.
- Judul dan deskripsi karya kedua dan ketiga masih placeholder.
- Email dan akun media sosial di halaman ini tampil publik. Pakai email khusus kerja jika ingin mengurangi spam.

## Menayangkan dengan GitHub Pages

1. Buat repository baru di GitHub (misalnya `portofolio`).
2. Unggah semua isi folder ini (lihat perintah di bawah, atau tombol Add file, Upload files di GitHub).
3. Buka Settings, Pages. Pada Source pilih Deploy from a branch, branch `main`, folder `/ (root)`, lalu Save.
4. Tunggu satu sampai dua menit. Websitemu tayang di `https://USERNAME.github.io/NAMA-REPO/`.

Ukuran satu file di GitHub maksimal 100 MB, dan sebaiknya video dikompres jauh di bawah itu agar website cepat dimuat.

```bash
cd portofolio-muhandis
git init
git add .
git commit -m "Initial commit: personal portfolio"
git branch -M main
git remote add origin https://github.com/USERNAME/NAMA-REPO.git
git push -u origin main
```

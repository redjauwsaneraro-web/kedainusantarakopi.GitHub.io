# Kopi Nusantara - Proyek Praktikum Pemrograman Internet I

Website statis Sistem Informasi Pemesanan Kafe **Kopi Nusantara** untuk mata kuliah
**Praktek Pemrograman Internet I (SI4072)**, Program Studi Sistem Informasi,
Fakultas Ilmu Komputer dan Manajemen, Universitas Sains dan Teknologi Jayapura.

Seluruh tugas **Modul 1 sampai Modul 12** sudah dikerjakan dalam satu folder proyek
ini. Tema proyek akhir yang dipilih: **SI Pemesanan Kafe/Rumah Makan**.

## Cara menjalankan

1. Buka folder `kopi-nusantara` di Visual Studio Code.
2. Buka `index.html`, klik kanan, pilih **Open with Live Server**.
3. Halaman admin ada di `admin/dashboard.html`.
4. Alternatif tanpa VS Code: buka `index.html` langsung di Chrome, atau jalankan
   `python -m http.server 8080` di folder ini lalu buka `http://localhost:8080`.

Bootstrap 5.3 sudah disimpan **offline** di `css/` dan `js/`, jadi tidak perlu internet.

## Struktur folder

```
kopi-nusantara/
├── index.html                  Beranda (Modul 1, 4)
├── kontak.html                 Halaman kontak (Modul 1)
├── menu.html                   Menu versi Bootstrap (Modul 10)
├── menu-manual.html            Menu versi CSS manual (Modul 3, 4)
├── pesan.html                  Form pemesanan + validasi (Modul 2, 7, 8)
├── admin/
│   ├── dashboard.html          Dashboard CSS Grid (Modul 5)
│   ├── pesanan.html            Tabel pesanan + cari + tombol Selesai (Modul 2, 5, 7)
│   ├── tambah-menu.html        Form tambah menu + validasi (Modul 2, 8)
│   └── dashboard-bs.html       Dashboard Bootstrap + modal (Modul 10)
├── css/
│   ├── style.css               CSS utama (Modul 3, 4, 8, 9)
│   ├── admin.css               Layout dashboard Grid (Modul 5, 9)
│   ├── bootstrap.min.css       Bootstrap 5.3.3 offline
│   └── bootstrap-kopi.css      Penyesuaian warna Bootstrap
├── js/
│   ├── app.js                  JavaScript, DOM, validasi (Modul 6, 7, 8)
│   └── bootstrap.bundle.min.js Bootstrap 5.3.3 offline
├── img/                        Logo dan gambar menu
├── lampiran/
│   └── flexbox-variasi.html    Bukti 3 variasi justify-content (Modul 4)
├── screenshot/                 Screenshot hasil untuk lampiran
├── README.md                   Panduan proyek (file ini)
└── DOKUMENTASI.md              Jawaban tugas pendahuluan, perhitungan, laporan
```

## Peta tugas per modul

| Modul | Tugas | File / bukti | Status |
|---|---|---|---|
| 1 | Struktur HTML, halaman beranda & kontak, testimoni `<article>`, nav berfungsi | `index.html`, `kontak.html` | Selesai |
| 2 | Tabel menu, form pesanan, tabel admin, form tambah menu, total `colspan` | `menu-manual.html`, `pesan.html`, `admin/pesanan.html`, `admin/tambah-menu.html` | Selesai |
| 3 | CSS external, selector element/class/ID, box model, kartu menu | `css/style.css`, `menu-manual.html` | Selesai |
| 4 | Navbar & galeri Flexbox, "Mengapa Memilih Kami" 3 kotak, 3 variasi `justify-content` | `index.html`, `lampiran/flexbox-variasi.html`, screenshot 16-19 | Selesai |
| 5 | Layout Grid dashboard (header, sidebar, main, footer), 3 kartu ringkasan, tabel di bawahnya | `admin/dashboard.html`, `admin/pesanan.html`, `admin/tambah-menu.html`, `css/admin.css` | Selesai |
| 6 | Array, object, `if`, `for`, function, diskon 10%, total pendapatan di Console | `js/app.js` | Selesai |
| 7 | Total harga otomatis, pencarian nama, tombol Selesai + baris hijau | `pesan.html`, `admin/pesanan.html`, `js/app.js` | Selesai |
| 8 | Validasi form pesanan & form tambah menu | `pesan.html`, `admin/tambah-menu.html`, `js/app.js` | Selesai |
| 9 | Responsif 375/768/desktop, sidebar pindah atas, tabel bisa di-scroll | `css/style.css`, `css/admin.css`, screenshot 04-05, 10-11 | Selesai |
| 10 | Bootstrap offline: navbar, card grid, table, badge, modal; menu Bootstrap; perbandingan | `menu.html`, `admin/dashboard-bs.html`, `css/bootstrap-kopi.css` | Selesai |
| 11 | Proyek akhir: halaman pengguna & admin, JS, validasi, responsif, sketsa | seluruh proyek, `DOKUMENTASI.md` | Selesai |
| 12 | Presentasi 5 menit, ZIP proyek + screenshot | `kopi-nusantara-proyek-akhir.zip`, `screenshot/` | Selesai |

## Fitur yang bisa diuji

- **Diskon otomatis**: pilih menu lalu isi jumlah ≥ 5 di `pesan.html`,
  total langsung berubah (mis. Kopi Susu × 5 = Rp90.000).
- **Validasi form**: nama minimal 3 huruf, No. HP harus diawali `08` dan 10-13 angka.
  Coba isi data salah lalu klik **Pesan Sekarang**.
- **Pencarian pesanan**: ketik nama pelanggan di `admin/pesanan.html`.
- **Tombol Selesai**: klik tombol pada baris berstatus "Diproses"; status berubah
  menjadi "Selesai" dan baris menjadi hijau.
- **Validasi tambah menu**: nama wajib, kategori wajib, harga minimal Rp5.000.
- **Bootstrap**: buka `menu.html`, klik **Cara Pesan** untuk melihat modal;
  `admin/dashboard-bs.html` memakai navbar, alert, card, table, badge, dan modal.
- **Responsif**: kecilkan jendela browser atau gunakan DevTools (375px, 768px).

## Catatan aset

Gambar di `img/` dibuat sebagai aset contoh (logo, kopi Wamena, kopi susu, teh tarik,
dan hero). Jika asisten membagikan **Folder Aset Kopi Nusantara**, timpa file dengan
nama yang sama:

- `img/logo.png`
- `img/kopi-wamena.jpg`
- `img/kopi-susu.jpg`
- `img/teh-tarik.jpg`
- `img/hero.jpg` (opsional, latar hero)

File Bootstrap di `css/bootstrap.min.css` dan `js/bootstrap.bundle.min.js` sudah
versi 5.3.3 dan dipakai secara offline.

## Hasil pengujian

Proyek diuji otomatis dengan Chrome headless (Playwright):

- 10 halaman: tidak ada error console, semua gambar dan link lokal valid.
- Tidak ada scroll horizontal pada lebar 1366px, 768px, dan 375px.
- Form pesanan: total diskon, validasi, dan pesan sukses benar.
- Tabel pesanan: pencarian, total Rp204.000, tombol Selesai berfungsi.
- Form tambah menu: semua validasi dan penambahan baris berfungsi.
- Bootstrap offline dan modal berfungsi.

**Hasil: 80 pengujian lulus, 0 gagal.**

## Screenshot

| File | Isi |
|---|---|
| `01-beranda-desktop.png` | Beranda desktop |
| `02-beranda-mobile.png` | Beranda ponsel (375px) |
| `03-menu-bootstrap-desktop.png` | Menu Bootstrap desktop |
| `04-menu-bootstrap-tablet.png` | Menu tablet (768px) |
| `05-menu-bootstrap-mobile.png` | Menu ponsel (375px) |
| `06-menu-css-manual.png` | Menu versi CSS manual |
| `07-pesan-desktop.png` | Form pemesanan |
| `08-kontak-desktop.png` | Halaman kontak |
| `09-dashboard-desktop.png` | Dashboard admin desktop |
| `10-dashboard-tablet.png` | Dashboard tablet (768px) |
| `11-dashboard-mobile.png` | Dashboard ponsel (375px) |
| `12-pesanan-desktop.png` | Data pesanan |
| `13-tambah-menu-desktop.png` | Form tambah menu |
| `14-dashboard-bootstrap-desktop.png` | Dashboard Bootstrap |
| `15-dashboard-bootstrap-mobile.png` | Dashboard Bootstrap ponsel |
| `16-flexbox-variasi.png` | Tiga variasi `justify-content` |
| `17-19-flexbox-*.png` | Screenshot terpisah tiap variasi |

## Penilaian

- Nilai pertemuan: rata-rata Modul 1-10 (50%)
- Proyek akhir: rubrik Modul 12 (50%)
- Nilai Akhir = 50% × rata-rata pertemuan + 50% × proyek akhir

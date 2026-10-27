# Dashboard Akademik — Pertemuan 6

## Tugas

Membuat Simple Design System untuk warna, tipografi, spacing, tombol, form
controls, dan cards, kemudian menerapkannya pada mockup Dashboard Mahasiswa
Contoh 2 dari modul Pertemuan 6.

## Berkas

- `../index-sebelum.html` — salinan tampilan dashboard sebelum pembaruan.
- `../tugas.html` — mockup dashboard sesudah menerapkan design system.
- `../design-system.html` — dokumentasi visual token dan contoh komponen.
- `../css/style.css` — token desain, komponen, dan aturan responsif.
- `../images/darwin-icon.jpg` — ikon Darwin yang digunakan sebagai foto profil.

Nama pada mockup disesuaikan menjadi **Farid Zhahir Muttaqin**, dan foto
profil pada tampilan sebelum maupun sesudah menggunakan ikon Darwin.

## Simple Design System

### Color palette

| Token | Nilai | Penggunaan |
| --- | --- | --- |
| Primary | `#4F46E5` | Tombol utama, navigasi aktif, tautan aksi |
| Primary dark | `#3730A3` | Hover dan kontras tombol utama |
| Accent | `#EEF2FF` | Latar ikon dan sorotan ringan |
| Text | `#172033` | Teks utama |
| Muted | `#667085` | Keterangan dan metadata |
| Border | `#E7EAF1` | Batas kartu dan pemisah |
| Success | `#15803D` | Status akademik aktif |
| Warning | `#B45309` | Pengumuman penting |
| Info | `#1D4ED8` | Informasi umum |

### Typography

Font utama `Arial, Helvetica, sans-serif` dengan skala: display 36px, heading
halaman 28px, heading bagian 20px, body 14px, dan label 12px. Label
menggunakan uppercase dan letter spacing untuk membedakannya dari isi.

### Spacing

Token spacing menggunakan kelipatan 4px: `space-1` 4px, `space-2` 8px,
`space-3` 12px, `space-4` 16px, `space-6` 24px, dan `space-8` 32px. Radius
kartu 14px; kontrol dan tombol 9px. Kartu memakai border tipis dan shadow
lembut agar terpisah dari latar.

### Komponen

- **Buttons:** primary untuk aksi utama, secondary untuk aksi pendamping, dan
  quiet untuk tautan aksi tanpa bidang tombol.
- **Form controls:** label terlihat, petunjuk input, pilihan semester, dan
  checkbox dengan focus state.
- **Cards:** kartu statistik dan panel pengumuman menggunakan token radius,
  warna permukaan, border, dan shadow yang konsisten.

## Perubahan, masalah, dan solusi

Dashboard awal memakai warna, jarak, dan komponen yang belum didokumentasikan
sebagai sistem, serta susunan desktop yang terlalu padat untuk layar ponsel.
Saya membuat token CSS terpusat agar warna, skala tipografi, spacing, tombol,
form, dan card dapat digunakan kembali. Ringkasan akademik dipisahkan menjadi
kartu, jadwal dan pengumuman disusun dalam panel dengan prioritas informasi
yang jelas, dan tabel diberi pembungkus horizontal. Grid desktop beralih
menjadi satu kolom pada layar kecil; sidebar menjadi navigasi yang dapat
digulir mendatar. Dengan cara ini konten tetap dapat dibaca tanpa
menghilangkan fungsi dan data penting dari Contoh 2.

## Dokumentasi sebelum dan sesudah

### Sebelum — Desktop

![Dashboard sebelum perubahan pada desktop](./screenshots/sebelum-desktop.png)

### Sebelum — Mobile

![Dashboard sebelum perubahan pada mobile](./screenshots/sebelum-mobile.png)

### Sesudah — Desktop

![Dashboard sesudah perubahan pada desktop](./screenshots/sesudah-desktop.png)

### Sesudah — Mobile

![Dashboard sesudah perubahan pada mobile](./screenshots/sesudah-mobile.png)

### Simple Design System

![Dokumentasi Simple Design System](./screenshots/design-system.png)

## Struktur

```text
tugas/
|-- tugas.html
|-- index-sebelum.html
|-- design-system.html
|-- css/
|   |-- style.css
|   `-- sebelum.css
|-- images/
|   `-- darwin-icon.jpg
`-- dokumentasi/
    |-- Readme.md
    `-- screenshots/
        |-- sebelum-desktop.png
        |-- sebelum-mobile.png
        |-- sesudah-desktop.png
        |-- sesudah-mobile.png
        `-- design-system.png
```

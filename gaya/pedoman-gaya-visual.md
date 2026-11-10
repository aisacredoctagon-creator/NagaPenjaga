# Pedoman Gaya Visual Naga Penjaga

Acuan tunggal: `referensi/konsep-visual.webp`. Token siap pakai: `gaya/gaya-token.css`. Pratinjau: `gaya/pratinjau.html`.
Tandanya: **[UKUR]** diukur dari gambar, **[TURUNAN]** dibuat dari warna terukur, **[USULAN]** tidak ada di gambar dan menunggu persetujuan Ibnu.
Pedoman ini hanya soal tampilan. Cara main, soal, skor, dan level tidak berubah.

## 1. Rasa dan prinsip
Cerah, hangat, jenaka, seperti kartun petualangan. Tidak menakutkan, termasuk Morvax (ungu gelap tetapi tidak seram). Anak 6–14 tahun harus langsung paham yang mana tombol, yang mana bola, dan yang mana bahaya. Cahaya selalu dari atas: kilau di atas, bayangan jatuh ke bawah, tidak pernah ke samping.

## 2. Karakter dan peta (keputusan Ibnu)
| Stage | Peta | Penjaga | Warna unsur | Catatan |
|---|---|---|---|---|
| 1 | Hutan Misterius | Bayunara, Naga Angin | hijau `#518d60` | |
| 2 | Gunung Bersalju | Esvara, Naga Es | biru `#3181c9` | |
| 3 | Gunung Berapi | Baranji, Naga Api | jingga `#e65328` | Morvax muncul sebagai bos final |
Morvax (`#6c52af`) hanya bos di stage 3. Di stage 1–2 pencuri telur tetap berupa siluet Morvax dan tidak dihitung sebagai bos. Tiga telur di sarang selalu biru, jingga, dan hijau seperti gambar, di semua stage.

## 3. Warna [UKUR]
| Peran | Warna |
|---|---|
| Pil judul biru | `#2b62a4` (atas `#3b78c4`) |
| Pil judul ungu | `#5e4ba1` (atas `#7561bd`) |
| Pil peta | hutan `#065548`, salju `#0a4996`, berapi `#992112` |
| Panel | biru muda `#ddecfc`, lavender `#d8d2fb` / `#dbddfb` |
| Peta (terang / median / gelap) | hutan `#b4b88d` / `#759357` / `#3a6542`; salju `#d6e7ff` / `#99b1e1` / `#456daa`; berapi `#dd896a` / `#935b50` / `#6e3a2a` |
| Orb (tepi / isi / kilau) | ungu `#4a0e86` / `#8a35d8` / `#e2c6ff`; biru `#1a5fb0` / `#3aa0ea` / `#d4ecff`; jingga `#b33a04` / `#f56a14` / `#ffd9a8`; hijau `#4f8a0e` / `#7cc61e` / `#e3f5b8` |
Bola jenis bilangan: asli = hijau, bulat = biru, desimal = jingga, pecahan = ungu. Ungu gelap pada gambar tidak dipakai.

## 4. Bentuk, tepi, bayangan
- **Label (pil) dan chip:** kapsul penuh `999px` [UKUR], isi gradasi (terang di atas), teks putih tebal dengan bayangan tipis, bayangan lembut `0 3px 8px`.
- **Panel:** sudut `22px` [UKUR], isi gradasi pastel (lebih putih di atas), garis terang tipis di tepi, bayangan lembut `0 8px 22px` biru-navy. Tanpa tepi gelap tebal.
- **Tombol:** kapsul seperti pil [TURUNAN], tepi `3px` sewarna gelap, kilau tipis di tepi atas dan setengah atas, "tebing" `4px` di bawah. Saat ditekan turun `3px`. Tinggi minimal `48px` (utama) dan `44px` (lainnya). Utama = jingga, kedua = biru, khusus ("Lihat jawabanmu") = ungu, pasif ("Menu") = biru-abu. **Pemilihan warna tombol adalah [USULAN]** karena gambar tidak punya tombol.
- **HUD di atas peta:** kapsul biru-navy gelap tembus pandang `rgba(18,24,60,.58)` [USULAN], teks putih tebal, supaya terbaca di peta terang (salju) maupun gelap.

## 5. Huruf
Bulat, tebal, mirip gambar: urutan `Nunito, Poppins, Segoe UI, Trebuchet MS, Roboto, Arial` [USULAN]. Tanpa berkas huruf luar, jadi di perangkat tanpa Nunito atau Poppins tampil huruf sistem yang mirip tetapi tidak sama. Judul berat 800, teks berat 600. Ukuran: judul 28, subjudul 18, teks 16, kecil 13 (minimal 11 piksel layar di HP).

## 6. Komponen game
- **Bola:** gambar orb dengan **cakram putih datar** di tengah untuk angka (teks navy tebal). Pecahan tetap bersusun. Peluru memakai cincin emas tebal di sekeliling orb jenis soal supaya tidak tertukar dengan orb jingga [USULAN, diuji di Tahap 3].
- **Naga:** gambar tiap stage (Bayunara, Esvara, Baranji) di tempat 🐲. Auman tetap berupa membesar dan bergetar. Cadangan kembali ke emoji.
- **Telur dan sarang:** sarang daun-ranting dari gambar, tiga telur biru, jingga, hijau satu per satu.
- **Bos dan pencuri:** Morvax di tempat 🧙.
- **Peta (digambar dengan kode):** lantai bertekstur sesuai tema (lumut dan batu, es dan salju, batu dan lava) dengan hiasan dari potongan gambar konsep seperlunya. **Jalur Bola Sihir berupa parit alami:** akar pohon (hutan), jejak es berbingkai salju (bersalju), aliran lava bercahaya `#ff7a1f` dengan tepi batu gelap (berapi). Jalur tetap terbaca sebagai jalur: lebih terang atau lebih gelap dari lantai, dengan tepi tegas.
- **Kerangka layar menang/kalah:** kerangka yang sudah disetujui (medali, pita, bintang, pelat telur dan skor, tombol) diubah mengikuti token ini: panel pastel, pita biru atau merah tua, bintang emas, tombol jingga/biru/ungu/biru-abu.

## 7. Keterbacaan dan anggaran
- Kontras teks diukur di `pratinjau.html`: putih di pil dan tombol 3,7–7,0 : 1; navy di panel 8,9–10,7 : 1. **Chip kecil (15 px) di unsur es, api, angin hanya 3,7–4,1 : 1:** pakai varian gelap (`--ng-*-gelap`) untuk teks kecil atau naikkan ukuran ke 18 px tebal.
- Gambar WebP di folder `aset/`, tiap gambar ≤ ±150 KB, total tambahan ≤ ±2 MB (perkiraan sekitar 1 MB), dengan cadangan emoji dan satu tombol pengaman `ASET_AKTIF`.
- Tombol minimal 44–48 px, game tetap lancar di HP kelas menengah (gambar dimuat sekali, latar peta digambar sekali ke kanvas cadangan).

## 8. Yang tidak ada di gambar dan perlu keputusan [USULAN]
| Hal | Pilihan 1 (rekomendasi) | Pilihan 2 |
|---|---|---|
| Huruf | tanpa berkas huruf, huruf sistem | tambah satu berkas huruf bulat (±30 KB) agar sama di semua perangkat |
| Tombol utama | jingga (hangat, mencolok, selaras chip Baranji) | biru permata (selaras pil judul, kurang mencolok) |
| Peluru | orb jenis soal dengan cincin emas | orb ungu gelap (bisa tertukar dengan ungu pecahan) |
| HUD | kapsul gelap tembus pandang | tanpa latar, hanya teks bertepi |

## 9. Elemen yang tidak bisa dipotong bersih dari gambar (perlu dibuat ulang)
1. Telur tunggal dan sarang kosong (telur muncul dan hilang satu per satu di game).
2. Pose kecil naga dan Morvax (±70 px, terlalu kecil).
3. Peta latar (jalur sudah "terpanggang" di gambar).
4. Naga dilihat dari atas (hanya satu naga biru di panel kecil).
5. Naga besar untuk layar sambutan di layar retina (gambar ±300 px, kurang tajam).

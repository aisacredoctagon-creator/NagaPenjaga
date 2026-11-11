# Daftar aset gambar akhir (gaya fantasi semi-realistis)

Semua benda di bawah sekarang digambar dengan kode dan terdaftar di `LIB` (Bagian 2B `index.html`). Untuk mengganti: simpan gambar WebP **dengan nama dan ukuran persis seperti tabel** di `aset/gambar/NAMA.webp`, lalu tulis `ASET_JADI['NAMA'] = true;` di Bagian 2B. Tidak ada logika game yang berubah.

Aturan semua gambar karakter: **latar polos (transparan, bukan putih)**, tepi bersih tanpa sisa putih, benda di tengah dengan ruang kosong ±5% di tepi, cahaya dari kiri atas. Jangan menaruh angka di gambar (angka digambar kode). Warna biru/hijau-toska/merah muda/ungu murni jangan dipakai pada benda kecil di dekat jalur (itu warna jenis bilangan).

| Nama berkas | Piksel | Pose / isi |
|---|---|---|
| `naga-bayunara-atas` | 400×400 | Naga angin hijau dilihat dari ATAS, kepala menghadap ATAS gambar, sayap terbentang, ekor ke bawah. Dipakai berputar mengikuti bidikan. |
| `naga-esvara-atas` | 400×400 | Sama, naga es biru |
| `naga-baranji-atas` | 400×400 | Sama, naga api oranye |
| `naga-bayunara-depan` | 512×512 | Duduk menghadap depan, sayap setengah terbuka (menu, cerita, spanduk, layar akhir) |
| `naga-esvara-depan` | 512×512 | Sama, naga es |
| `naga-baranji-depan` | 512×512 | Sama, naga api |
| `morvax` | 384×512 (3:4) | Penyihir menghadap depan, berdiri, tongkat dengan bola ungu di tangan kanan (sisi kanan gambar). Mata ungu menyala, wajah tidak terlalu seram. Siluet gelapnya dibuat otomatis oleh kode. |
| `telur-biru` | 128×160 | Telur es, tegak, tanpa sarang |
| `telur-hijau` | 128×160 | Telur angin |
| `telur-jingga` | 128×160 | Telur api |
| `sarang-belakang` | 320×200 | Bagian belakang sarang (dasar + bibir belakang), tanpa telur. Titik tengah sarang di 50% lebar, 25% tinggi |
| `sarang-depan` | 320×200 | Bibir depan sarang saja (setengah bawah), di posisi yang sama dengan `sarang-belakang`, supaya telur bisa terselip di antaranya |
| `bayangan-naga` | 256×256 | Bayangan lembut bulat/lonjong (boleh tetap dibuat kode) |

Latar (Batch 2; sekarang masih kode): latar bersih TANPA jalur, bola, sarang, teks, dalam dua bentuk per stage: tegak 1200×2000 (dan sampai 1200×2600 untuk HP panjang; isi tepi atas/bawah boleh dipotong) dan lebar 2000×1200. Nama: `latar-hutan-tegak`, `latar-hutan-lebar`, `latar-salju-tegak`, `latar-salju-lebar`, `latar-api-tegak`, `latar-api-lebar`. Jalur batu digambar kode di atasnya.

Tidak perlu gambar: bola dan peluru (digambar kode), angka, panel persamaan, tombol, bintang, perisai, titik kemajuan.

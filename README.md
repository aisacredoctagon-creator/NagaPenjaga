# Naga Penjaga

Game matematika di browser untuk anak usia 6–14 tahun. Pemain menembak bola angka, mencocokkan dua bola yang hasilnya sama dengan angka di panel, dan menjaga telur naga dari penyihir jahat.

## Main sekarang

**[▶ Buka game](https://aisacredoctagon-creator.github.io/NagaPenjaga/)**

Berjalan di browser tanpa instal. Dirancang untuk laptop dan HP (dipegang tegak). Uji di HP asli belum dilakukan.

## Tentang game

- **Untuk siapa:** anak usia 6–14 tahun, dengan dua tingkat: Mudah dan Menantang.
- **Yang dilatih:** tambah, kurang, kali, dan bagi, juga bilangan bulat, desimal, dan pecahan. Anak berlatih lewat permainan, bukan lewat kuis yang ditempelkan.
- **Lama main:** sekitar 3–5 menit per stage (tahap).

**Cara bermain dalam 3 langkah**

1. **Pilih** tingkat, waktu, dan hitungan di menu, lalu tekan "Mulai Petualangan".
2. **Ketuk bola** di jalur. Jika bola tembakan dan bola yang kena dihitung hasilnya sama dengan angka di panel (contoh ◯ + ◯ = 10: bola 4 dan bola 6), keduanya meledak.
3. **Jaga 3 telur.** Jawaban salah atau bola yang sampai di sarang membuat satu telur dicuri. Habiskan semua bola untuk menang.

## Isi game

| Bagian | Isi |
| --- | --- |
| Stage 1: Hutan Hijau | 22 bola (Mudah) / 26 (Menantang). Ada peragaan 4 detik tanpa kata di awal. |
| Stage 2: Gunung Bersalju | 24 / 29 bola, sedikit lebih cepat. |
| Stage 3: Gunung Api | 24 / 29 bola, lalu bertambah. Penyihir bos tiap 30 detik mengganti angka panel dan menambah 1 bola. |
| Hitungan | Tambah, kurang, kali, bagi, bilangan bulat, desimal, pecahan berpenyebut sama. Boleh memilih lebih dari satu. |
| Pelengkap | Perisai, bola telur naga, dua bola bertukar tempat, dan layar tinjauan jawaban. |

## Status saat ini

**Sudah jadi (versi 2.6):** game lengkap dari menu sampai layar tamat. Tampilan sudah diperiksa di lebar layar 360, 390, 768 piksel dan desktop. Uji otomatis (64 uji) tidak menemukan galat halaman. Robot uji ini selalu memilih jawaban benar, jadi tidak mengukur kesulitan untuk anak.

**Hasil uji pemain robot.** Diuji dengan pemain robot, bukan anak-anak. Robot menembak tiap 2,5–4,5 detik dengan tingkat salah acak tertentu (10 percobaan per sel). Di Menantang stage 1 / 2 / 3 dengan telur dan perisai (v2.6), robot yang salah 5% menang 10 / 10 / 10 dari 10, dan robot yang salah 25% menang 4 / 2 / 2 dari 10. Robot yang sangat sering salah tetap kesulitan. Hanya petunjuk awal; tabel lengkap ada di [dokumen konsep](konsep-naga-penjaga-telur.md#status-dan-hasil-uji).

**Batasan:**
- Belum diuji di HP asli, Safari iPhone, dan dengan anak sungguhan.
- Gambar masih emoji sementara.
- Pecahan hanya berpenyebut sama dan tidak disederhanakan (2/4 tetap 2/4).

## Belum ada dan keputusan terbuka

- [ ] Pecahan berpenyebut beda.
- [ ] Gambar resmi karakter dan aturan merek.
- [ ] Cara mengumpulkan masukan dari pemain.
- [ ] Keseimbangan telur: pelonggaran "telur hilang tiap 2 salah" masih opsi bila anak terlalu sering kalah, termasuk di Menantang stage 2 dan 3.

## Catatan teknis

- Seluruh game ada di satu berkas, [`index.html`](index.html), tanpa pustaka tambahan.
- Dokumen lengkap (aturan, hitungan, rincian pengembangan): [konsep-naga-penjaga-telur.md](konsep-naga-penjaga-telur.md).

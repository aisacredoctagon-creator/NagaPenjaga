# Naga Penjaga

Game matematika di browser untuk anak usia 6–14 tahun. Pemain menembak bola angka, mencocokkan dua bola yang hasilnya sama dengan angka di panel, dan menjaga telur naga dari penyihir jahat.

## Main sekarang

**[▶ Buka game](https://aisacredoctagon-creator.github.io/NagaPenjaga/)**

Berjalan di browser tanpa instal. Tampilan menyesuaikan layar: tegak di HP berdiri, lebar di laptop dan HP mendatar. Game dibuka dengan layar sambutan, ada musik dan efek suara buatan kode, dan semuanya bisa dimatikan. Uji di HP asli belum dilakukan.

## Tentang game

- **Untuk siapa:** anak usia 6–14 tahun, dengan dua tingkat: Mudah dan Menantang.
- **Yang dilatih:** tambah, kurang, kali, dan bagi, juga bilangan bulat, desimal, dan pecahan. Anak berlatih lewat permainan, bukan lewat kuis yang ditempelkan.
- **Lama main:** sekitar 3–5 menit per stage (tahap).

**Cara bermain dalam 3 langkah**

1. **Tekan "Mulai Main"**, lalu pilih tingkat, waktu, dan hitungan di menu dan tekan "Mulai Petualangan".
2. **Bidik bola** di jalur (komputer: arahkan mouse lalu klik; HP: tahan jari pada bola, lepas untuk menembak). Kotak di panel atas berubah mengikuti bola itu. Jika peluru dan bola yang dibidik menyusun persamaan yang benar (contoh ◯ + ◯ = 10: bola 4 dan bola 6), keduanya meledak. Di stage 2 dan 3 ada angka tetap di panel, misalnya ◯ + ◯ + 2 = 8.
3. **Jaga 3 telur.** Jawaban salah atau bola yang sampai di sarang membuat satu telur dicuri. Habiskan semua bola untuk menang.

## Isi game

| Bagian | Isi |
| --- | --- |
| Stage 1: Hutan Hijau | 22 bola (Mudah) / 26 (Menantang). Tur 3 langkah di awal (bisa dilewati), sekali per permainan. |
| Stage 2: Gunung Bersalju | 24 / 29 bola, sedikit lebih cepat. |
| Stage 3: Gunung Api | 26 / 31 bola, lebih cepat dari stage 2, lalu bertambah. Penyihir bos tiap 22 detik mengganti angka panel dan menambah 1 bola. |
| Hitungan | Tambah, kurang, kali, bagi, bilangan bulat, desimal, pecahan berpenyebut sama. Boleh memilih lebih dari satu. |
| Pelengkap | Perisai, bola telur naga, dua bola bertukar tempat, dan layar tinjauan jawaban. |
| Layar | Dua layout yang berganti otomatis: tegak (HP berdiri) dan lebar (laptop, HP mendatar). Bila layar diputar saat bermain, game berhenti sampai layar dikembalikan, tanpa kehilangan kemajuan. |
| Layar sambutan | Muncul setiap halaman dibuka: judul "Naga Penjaga", naga, telur, penyihir kecil, bola angka melayang, dan satu tombol "Mulai Main". Isinya diatur dari satu tempat di kode (`SPLASH` dan `SPLASH_ART`). |
| Suara | Dua lagu (menu dan bermain) dan enam efek suara, semuanya dibuat kode, tanpa berkas. Baru berbunyi setelah ketukan pertama (aturan browser). Tiga tombol: 🎵 Musik, 🔊 Suara, ✨ Efek gambar; di menu ada di pojok kanan atas, di dalam game ada di menu Jeda. Pilihan tersimpan di browser. |
| Jeda | Tombol ⏸ di pojok kanan atas game (menggantikan ✕): ▶ Lanjut main, ↻ Mulai ulang (stage ini dari awal, skor total tetap), 🏠 Ke menu (kemajuan permainan itu hilang). |

## Status saat ini

**Sudah jadi (versi 2.6 dengan mekanik "Rakit Persamaan" v7):** game lengkap dari menu sampai layar tamat. Tampilan sudah diperiksa di beberapa ukuran: 360, 390, 768 piksel (tegak) serta 844×390, 1024×600, dan 1024×576 (lebar). Uji otomatis (102 uji) tidak menemukan galat halaman, dan layout tegak terbukti tidak berubah oleh layout lebar. Robot uji ini selalu memilih jawaban benar, jadi tidak mengukur kesulitan untuk anak.

**Hasil uji pemain robot.** Diuji dengan pemain robot, bukan anak-anak. Robot menembak tiap 2,5–4,5 detik dengan tingkat salah acak tertentu (10 percobaan per sel). Di Menantang stage 1 / 2 / 3 dengan telur dan perisai (v2.6), robot yang salah 5% menang 10 / 10 / 10 dari 10, dan robot yang salah 25% menang 4 / 2 / 2 dari 10. Robot yang sangat sering salah tetap kesulitan. Robot yang kadang salah di layout lebar menang 381 dari 480 percobaan, setara dengan layout tegak (383 dari 480). Hanya petunjuk awal; tabel lengkap ada di [dokumen konsep](konsep-naga-penjaga-telur.md#status-dan-hasil-uji).

**Batasan:**
- Belum diuji di HP asli, Safari iPhone, dan dengan anak sungguhan.
- Suara baru diukur otomatis (bunyi ada, tidak meluap, pelan). Enak atau tidaknya di telinga, dan suara di HP asli serta Safari iPhone, belum didengar langsung.
- Gambar masih emoji sementara.
- Pecahan hanya berpenyebut sama dan tidak disederhanakan (2/4 tetap 2/4).
- Layout lebar memakai dunia tetap 1000×600, jadi di layar yang jauh lebih lebar ada pita kosong di sisi.

## Belum ada dan keputusan terbuka

- [ ] Pecahan berpenyebut beda.
- [ ] Sembilan jalur lebar dan layout lebar yang lentur mengikuti bentuk layar.
- [ ] Gambar resmi karakter dan aturan merek.
- [ ] Cara mengumpulkan masukan dari pemain.
- [ ] Keseimbangan telur: pelonggaran "telur hilang tiap 2 salah" masih opsi bila anak terlalu sering kalah, termasuk di Menantang stage 2 dan 3.

## Catatan teknis

- Seluruh game ada di satu berkas, [`index.html`](index.html), tanpa pustaka tambahan.
- Dokumen lengkap (aturan, hitungan, rincian pengembangan): [konsep-naga-penjaga-telur.md](konsep-naga-penjaga-telur.md).

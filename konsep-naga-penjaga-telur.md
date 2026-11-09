# Konsep Game Naga Penjaga Telur

Tanggal: 8 November 2026

## Ringkasan

Naga Penjaga Telur adalah game matematika di browser untuk anak usia 6–14 tahun: pemain menembakkan bola angka agar dua bola yang dihitung hasilnya sama dengan angka di panel, lalu keduanya meledak. Versi 2 sudah bisa dimainkan penuh dari menu sampai layar tamat, dengan 3 stage dan satu bos.

- **Tujuan:** melatih tambah, kurang, kali, dan bagi lewat permainan, bukan lewat kuis yang ditempelkan.
- **Bentuk:** satu halaman web (HTML5), responsif di laptop, PC, Android, dan iPhone lewat browser.
- **Lama main:** sekitar 3–5 menit per stage; waktu bisa dinyalakan atau dimatikan.
- **Tingkat:** Mudah dan Menantang.
- **Tenggat:** bisa dimainkan utuh pada Jumat 13 November 2026 (presentasi pukul 14.00).
- **Yang belum ada:** pecahan berpenyebut beda, gambar resmi karakter, dan uji di HP asli.

## Cerita

Seekor naga menjaga telur-telurnya, tetapi Penyihir Jahat ingin mencurinya untuk menguasai dunia. Pemain membantu naga dengan meledakkan bola-bola sihir sebelum sampai ke telur.

Cerita tampil sebagai 3 slide bergambar dengan teks pendek, dan bisa dilewati kapan saja:

1. Naga menjaga telur-telurnya.
2. Penyihir Jahat ingin mencuri telur untuk menguasai dunia.
3. Ajakan: cocokkan dua bola untuk meledakkan bola sihir.

Tiap stage melindungi satu telur; di stage 3 pemain mengalahkan penyihirnya langsung.

## Cara bermain (konsep "Pasangan Ajaib")

Bola-bola angka bergerak pelan di sepanjang jalur menuju telur. Di panel atas tertulis persamaan dengan dua lingkaran kosong, misalnya ◯ + ◯ = 10. Pemain menembak bola dari naga ke bola di jalur; jika bola tembakan dan bola yang kena, saat dihitung, sama dengan angka di panel, keduanya meledak.

1. **Bidik dan tembak:** ketuk bola yang dituju. Peluru sihir menembus bola lain dan menempel di bola itu, jadi bola yang tertutup tetap bisa dijawab; bola yang disentuh kursor diberi cincin. Mengetuk tempat kosong menembak lurus ke arah itu.
2. **Cocok:** dua bola dihitung (misalnya 4 + 6 = 10), keduanya meledak, bola di sekitarnya merapat; jika hasil rantai bertemu pasangan baru, meledak berantai.
3. **Tidak cocok:** bola menempel di rantai, dan jalur berjalan sedikit lebih cepat (bukan hukuman keras).
4. **Tukar bola:** ketuk naga untuk menukar dengan bola berikutnya (ditampilkan kecil di samping naga).
5. **Menang:** semua bola di jalur habis sebelum menyentuh telur. **Kalah:** bola menyentuh telur, atau waktu habis (jika memakai waktu).

Angka di panel (angka kunci) berganti setiap 3 pasangan yang berhasil. Game memastikan selalu ada bola yang bisa dicocokkan, supaya pemain tidak buntu.

## Tiga stage

Setiap stage punya latar, jalur berkelok, dan jumlah bola sendiri; stage 2 dan 3 lebih banyak bola dan sedikit lebih cepat dari stage 1. Stage 3 menambah bos.

| Stage | Latar | Jumlah bola (Mudah / Menantang) | Laju relatif | Yang baru |
| --- | --- | --- | --- | --- |
| 1. Hutan Hijau | Hijau, pohon dan jamur | 22 / 26 | ×1,00 | Peragaan 4 detik tanpa kata di awal |
| 2. Gunung Bersalju | Biru es, salju, pohon cemara, boneka salju, dan penguin | 24 / 29 | ×1,08 | Jalur miring berkelok seperti jalan setapak gunung, warna jalur putih salju |
| 3. Gunung Api | Ungu gelap, lava dan kelelawar | 24 / 29, lalu bertambah | ×1,05 | Penyihir bos dengan bar nyawa |

Bos di stage 3: penyihir berdiri di awal jalur. Bar nyawanya menunjukkan sisa bola dibanding jumlah awal. Setiap 30 detik ia merapal mantra: angka di panel berganti, 1 bola ditambahkan di ujung rantai, dan muncul tulisan "Mantra baru!". Pemain menang dengan menghabiskan semua bola.

Jumlah bola dasar dan laju dasar di tabel dikali pengali stage; angka persisnya ada di bagian rincian pengembangan.

**Jalur dan posisi acak.** Tiap stage punya 3 jalur (total 9 variasi) dengan panjang setara (selisih paling banyak 7%). Satu jalur dipilih acak saat stage dimulai dan tetap sama jika pemain mengulang stage setelah kalah; permainan baru mengacak lagi. Naga berada di tengah bawah layar atau di tengah layar (naga tengah menembak ke segala arah), dan sarang telur di tempat berbeda tiap jalur.

Aturan perancangan jalur: sarang paling jauh 260 satuan dari naga, jarak sarang dari tempat bola masuk paling sedikit 450 satuan, dan jalur tidak lewat dekat naga (kecuali menuju sarang). Di stage 3, penyihir berdiri dekat tempat bola masuk.

## Matematika di dalam permainan

Setiap tembakan adalah satu soal: pemain memilih bola mana yang cocok dengan bola tembakannya. Tidak ada kuis terpisah. Sebelum bermain, pemain memilih hitungan lewat tombol + − × ÷, Bilangan bulat, Desimal, dan Pecahan (boleh lebih dari satu).

Angka di panel diambil dari daftar berikut, menurut operasi dan tingkat:

| Operasi | Mudah | Menantang |
| --- | --- | --- |
| Tambah | 7, 8, 9, 10, 10, 11, 12 | 14, 16, 18, 20, 22, 25 |
| Kurang | 1, 2, 3, 4, 5 | 3, 4, 5, 6, 7, 8, 9 |
| Kali | 6, 8, 12, 18, 24 | 24, 30, 36, 48, 60, 72 |
| Bagi | 2, 3, 4 | 2, 3, 4, 5, 6 |

Angka bola di jalur dibatasi 1–9 di Mudah; di Menantang sampai 12 (kali dan bagi) atau 15 (tambah dan kurang). Bola tembakan kadang lebih besar, karena dipilih sebagai pasangan bola yang ada di jalur. Untuk kurang dan bagi, yang dihitung adalah angka besar terhadap angka kecil, sehingga urutan bola tidak berpengaruh.

Tiga jenis bilangan tambahan ada di tingkat Mudah dan Menantang, dengan angka lebih kecil di Mudah. Ketiganya dimainkan dengan cara menjumlahkan dua bola; angka di panel tetap berbentuk ◯ + ◯ = hasil.

| Jenis | Tingkat | Bola di jalur | Angka panel | Contoh |
| --- | --- | --- | --- | --- |
| Bilangan bulat | Mudah | −5 sampai 5, tanpa 0 | 1–3 dan −1 sampai −3 | 3 + (−2) = 1 |
| Bilangan bulat | Menantang | −9 sampai 9, tanpa 0 | 1–5 dan −1 sampai −5 | 5 + (−3) = 2 |
| Desimal | Mudah | 0,1 sampai 0,5 | 0,6 sampai 1,0 | 0,2 + 0,4 = 0,6 |
| Desimal | Menantang | 0,1 sampai 0,9 | 0,8 sampai 1,3 | 0,3 + 0,7 = 1,0 |
| Pecahan (penyebut sama) | Mudah | 1/penyebut sampai (penyebut−1)/penyebut; penyebut 2, 3, 4 untuk stage 1, 2, 3 | penyebut−1, 1, dan penyebut+1 per penyebut (stage 2: 2/3, 1, 4/3) | 1/3 + 2/3 = 1 |
| Pecahan (penyebut sama) | Menantang | sama; penyebut 4, 5, 6 untuk stage 1, 2, 3 | sama (stage 1: 3/4, 1, 5/4) | 1/4 + 3/4 = 1 |

Bola ditulis bersusun (pembilang di atas penyebut). Bola hanya cocok dengan bola sejenis; menembak bola beda jenis menampilkan "Beda jenis bilangan". Jika jenis dicampur, jalur diperlambat (2 jenis ×0,92; 3 jenis ×0,82; 4 jenis ×0,78) dan tiap jenis punya warna sendiri.

## Tingkat, waktu, dan kesalahan

- **Mudah:** bola lebih sedikit, jalur lebih pelan (laju dasar 8), angka kecil, dan ada bantuan: setelah 2 tembakan salah berturut-turut, satu bola yang cocok berdenyut dengan lingkaran.
- **Menantang:** bola lebih banyak (26), jalur sedikit lebih cepat (laju dasar 9), angka lebih besar, tanpa bantuan berkedip.
- **Dengan waktu:** 5 menit per stage; waktu habis berarti stage diulang. **Tanpa waktu:** tampil "∞ Tanpa waktu".
- **Kesalahan:** tidak ada nyawa yang hilang. Tiap salah menambah laju jalur 7%, dengan batas ×1,8. Laju ditampilkan di layar (misalnya "Laju ×1.00").
- **Bintang tiap stage:** ketepatan 80% ke atas = 3 bintang, 60% ke atas = 2 bintang, selain itu 1 bintang. Skor total terkumpul sepanjang 3 stage.
- **Kalah:** stage bisa diulang langsung dari layar kalah tanpa kembali ke menu.

## Kejelasan untuk anak 6–14 tahun

Prototipe awal membingungkan karena "angka kunci" tidak jelas. Empat perbaikan disetujui dan sudah dipasang:

1. **Panel persamaan bergambar:** ◯ + ◯ = 10 menunjukkan bahwa dua bola harus dijumlahkan menjadi 10.
2. **Peragaan 4 detik tanpa kata** di awal stage 1, supaya tidak perlu membaca aturan.
3. **Persamaan sebagai umpan balik:** setelah menembak, tampil persamaan nyata (misalnya 4 + 6 = 10), sehingga anak melihat kenapa cocok atau tidak.
4. **Bantuan berkedip di tingkat Mudah** setelah 2 salah berturut-turut.

Prinsip yang dipakai: sedikit teks, banyak isyarat gambar, dan contoh. Anak usia 6–8 tahun masih belajar membaca, jadi petunjuk utamanya harus berupa gambar. Saat jenis bilangan dicampur, bola dan lubang di panel diberi warna yang sama per jenis (asli hijau-biru, bulat biru, desimal merah muda, pecahan ungu), supaya anak tahu bola mana yang dicari.

Catatan: belum ada uji dengan anak sungguhan sebelum publikasi; hanya Ibnu, tim kantor, dan atasan yang akan mencoba.

## Status, hasil uji, dan jadwal

Pada 8 November 2026, v2 sudah lengkap dari menu sampai layar tamat dan lolos uji simulasi tanpa galat halaman. Uji ini memakai pemain robot, bukan anak-anak, jadi angkanya hanya petunjuk awal.

Jumlah kemenangan dari 8 percobaan per skenario:

| Skenario | Robot cepat (4 dtk/tembakan) | Robot lambat (6 dtk/tembakan) |
| --- | --- | --- |
| Stage 1, Mudah tambah–kurang | 8 | 8 |
| Stage 1, Mudah kali–bagi | 8 | 8 |
| Stage 1, Menantang semua operasi | 8 | 6 |
| Stage 2, Mudah tambah–kurang | 8 | 7 |
| Stage 2, Mudah kali–bagi | 8 | 8 |
| Stage 2, Menantang semua operasi | 7 | 3 |
| Stage 3, Mudah tambah–kurang | 8 | 8 |
| Stage 3, Mudah kali–bagi | 7 | 6 |
| Stage 3, Menantang semua operasi | 7 | 4 |

Temuan: Menantang di stage 2 dan 3 masih berat untuk pemain lambat; perlu dilonggarkan atau diputuskan memang sengaja sulit.

Jenis bilangan baru di Menantang (8 percobaan): robot cepat menang 7–8 dari 8 di semua stage; hanya campuran semua jenis di stage 3 turun ke 6. Robot lambat menang 5–8 di stage 1–2, tetapi di stage 3 bilangan bulat 2/8, desimal 1/8, campuran 3/8 (pecahan 7/8). Stage 3 Menantang lambat memang sudah berat sebelum ada jenis baru. Di Mudah (8 percobaan): robot cepat menang 8 dari 8 di semua skenario; robot lambat menang 7–8 dari 8 (stage 3: bulat 7/8, desimal 8/8, pecahan 7/8, campuran 7/8).

Sembilan jalur (8 percobaan per jalur, tambah-kurang-kali-bagi di Menantang): robot cepat menang 6–8 dari 8 di semua jalur (campur semua jenis: 5–8); robot lambat menang 7 dari 8 di stage 1, 5–7 di stage 2, dan hanya 2–3 di stage 3. Jalur lain tidak membuat game lebih sulit dari jalur lama. Uji peluru menembus: 54 dari 54 ketukan mengenai bola yang diketuk.

Usulan jadwal (menunggu persetujuan Ibnu):

1. **Senin–Selasa:** uji di HP asli (termasuk Safari iPhone), longgarkan Menantang, rapikan layar menang dan kalah.
2. **Rabu pagi:** uji bilangan bulat, desimal, dan pecahan bersama tim, lalu perbaiki. **Rabu 13.00:** check-in dengan atasan; pecahan berpenyebut beda diputuskan setelahnya.
3. **Kamis:** poles tampilan, uji di beberapa perangkat dan browser.
4. **Jumat sebelum 14.00:** perbaikan akhir, lalu presentasi.

## Rincian untuk pengembangan

Seluruh game ada di satu berkas `index.html` (HTML, gaya, dan JavaScript tanpa pustaka tambahan), digambar di kanvas (area gambar di halaman). Berkas dibagi 12 bagian bertanda komentar; semua angka yang sering diubah ada di Bagian 1 (Pengaturan).

| Bagian | Isi |
| --- | --- |
| 1 | Pengaturan: ukuran bola, jumlah bola, laju, waktu, daftar angka kunci, data stage, tema |
| 2–3 | Alat bantu dan jalur (titik-titik jalur dengan sudut membulat) |
| 4–6 | Keadaan game, hitungan, bola tembakan dan angka panel |
| 7–8 | Alur stage (banner, peragaan, menang/kalah) dan efek |
| 9–10 | Logika permainan dan menembak |
| 11–12 | Gambar, layar sentuh, menu, cerita |

Angka pengaturan utama:

| Pengaturan | Nilai sekarang | Fungsi |
| --- | --- | --- |
| Waktu per stage | 300 detik | batas waktu jika memilih dengan waktu |
| Bola dasar | 22 Mudah, 26 Menantang | dikali pengali stage |
| Laju dasar | 8 Mudah, 9 Menantang | piksel per detik, dikali pengali stage |
| Pengali stage 1 / 2 / 3 | bola 1,0 / 1,1 / 1,1; laju 1,0 / 1,08 / 1,05 | menaikkan kesulitan tiap stage |
| Ganti angka kunci | tiap 3 pasangan | variasi soal |
| Percepatan per salah | 7%, maksimum ×1,8 | kesalahan membuat jalur lebih cepat |
| Mantra bos | tiap 30 detik, +1 bola | tekanan di stage 3 |

Penjaga agar tidak buntu: sekitar 70% bola tembakan dibuat sebagai pasangan bola yang bisa dijangkau, game memilih angka kunci yang punya minimal 2 bola cocok, dan memeriksa tiap 0,25 detik bahwa salah satu dari 2 bola siap tembak berguna. Tiap bola dan peluru membawa tanda jenis bilangan; desimal disimpan sebagai bilangan bulat satuan 0,1 dan pecahan sebagai pembilang, supaya tidak ada galat pembulatan. Pengaturan baru di Bagian 1: penyebut pecahan per stage, batas bola bulat dan desimal per tingkat, angka panel jenis baru, dan faktor perlambatan jika jenis dicampur.

Tampilan: lebar logis 600, tinggi menyesuaikan layar (1000–1300), kanvas diskalakan penuh dengan batas ketajaman layar 2,5×. Kontrol memakai pointer events sehingga sentuhan dan mouse sama. Tiap stage menyimpan daftar 3 jalur (titik jalur, posisi naga, posisi bos) di Bagian 1; jalur terpilih disimpan per permainan. Peluru menembus: peluru mengejar bola sasaran dan mengabaikan bola lain; jika bola sasaran hilang di tengah jalan, peluru menjadi tembakan lurus biasa.

## Batasan dan keputusan terbuka

Batasan saat ini:

- Belum diuji di HP asli, Safari iPhone, dan sentuhan sungguhan; hanya simulasi dan tangkapan layar ukuran HP.
- Gambar masih emoji sementara; menunggu aturan merek dan karakter dari kantor.
- Pecahan hanya berpenyebut sama, tidak disederhanakan (2/4 tetap 2/4), dan belum ada pecahan campuran; jenis baru belum diuji pada anak. Di Mudah stage 1 penyebutnya 2, sehingga semua bola ½ dan hanya ada ½ + ½ = 1 (sangat mudah).
- Konsep "Persamaan Bolong" tidak ada di v2 (hanya di prototipe lama).
- Belum diunggah ke GitHub kantor atau dipasang di Sarang Gasing.
- Keseimbangan kesulitan baru diuji dengan robot. Peluru menembus membuat semua bola bisa dijawab, jadi kesulitan perlu dicek lagi dengan pemain sungguhan; stage 3 Menantang tetap berat untuk robot lambat.

Keputusan yang menunggu Ibnu:

- [ ] Melonggarkan tingkat Menantang di stage 2 dan 3, atau membiarkannya sulit.
- [ ] Apakah pecahan berpenyebut beda masuk sebelum Jumat; diputuskan setelah check-in Rabu 13.00.
- [ ] Cara mengumpulkan masukan setelah game dipasang di Sarang Gasing.
- [ ] Aturan merek dan karakter: kapan dan dari siapa.

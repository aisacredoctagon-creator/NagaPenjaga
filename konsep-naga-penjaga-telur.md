# Konsep Game Naga Penjaga Telur

Tanggal: 8 November 2026 (diperbarui 9 November 2026, versi 2.6 dengan layout lebar, layar sambutan, suara, dan menu Jeda)

## Ringkasan

Naga Penjaga Telur adalah game matematika di browser untuk anak usia 6–14 tahun: pemain menembakkan bola angka agar dua bola yang dihitung hasilnya sama dengan angka di panel, lalu keduanya meledak. Versi 2 sudah bisa dimainkan penuh dari menu sampai layar tamat, dengan 3 stage dan satu bos.

- **Tujuan:** melatih tambah, kurang, kali, dan bagi lewat permainan, bukan lewat kuis yang ditempelkan.
- **Bentuk:** satu halaman web (HTML5), responsif di laptop, PC, Android, dan iPhone lewat browser. Ada dua layout yang berganti otomatis menurut bentuk layar: tegak (HP berdiri, tablet tegak) dan lebar (laptop, PC, HP mendatar).
- **Lama main:** sekitar 3–5 menit per stage; waktu bisa dinyalakan atau dimatikan.
- **Tingkat:** Mudah dan Menantang.
- **Nyawa:** 3 telur di sarang tiap stage; salah jawab atau bola yang sampai di sarang membuat satu telur dicuri penyihir. 5 jawaban benar berturut-turut memberi perisai yang menahan satu salah jawab.
- **Tinjauan:** setelah stage selesai atau kalah, ada layar terpisah untuk melihat jawaban (kesalahan dulu, hanya dibaca).
- **Dimainkan di:** https://aisacredoctagon-creator.github.io/NagaPenjaga/
- **Yang belum ada:** pecahan berpenyebut beda, gambar resmi karakter, uji di HP asli, dan 9 jalur lebar (sekarang satu jalur lebar per stage).

## Cerita

Seekor naga menjaga telur-telurnya, tetapi Penyihir Jahat ingin mencurinya untuk menguasai dunia. Pemain membantu naga dengan meledakkan bola-bola sihir sebelum sampai ke telur.

Cerita tampil sebagai 3 slide bergambar dengan teks pendek, dan bisa dilewati kapan saja:

1. Naga menjaga telur-telurnya.
2. Penyihir Jahat ingin mencuri telur untuk menguasai dunia.
3. Ajakan: cocokkan dua bola untuk meledakkan bola sihir.

Tiap stage menjaga 3 telur di sarang; di stage 3 pemain mengalahkan penyihirnya langsung.

## Cara bermain (konsep "Pasangan Ajaib")

Bola-bola angka bergerak pelan di sepanjang jalur menuju telur. Di panel atas tertulis persamaan dengan dua lingkaran kosong, misalnya ◯ + ◯ = 10. Pemain menembak bola dari naga ke bola di jalur; jika bola tembakan dan bola yang kena, saat dihitung, sama dengan angka di panel, keduanya meledak.

1. **Bidik dan tembak:** ketuk bola yang dituju. Peluru sihir menembus bola lain dan menempel di bola itu, jadi bola yang tertutup tetap bisa dijawab; bola yang disentuh kursor diberi cincin. Mengetuk tempat kosong menembak lurus ke arah itu.
2. **Cocok:** dua bola dihitung (misalnya 4 + 6 = 10), keduanya meledak, bola di sekitarnya merapat; jika hasil rantai bertemu pasangan baru, meledak berantai.
3. **Tidak cocok:** bola menempel di rantai, jalur berjalan sedikit lebih cepat, dan satu telur dicuri penyihir.
4. **Tukar bola:** ketuk naga untuk menukar dengan bola berikutnya (ditampilkan kecil di samping naga).
5. **Menang:** semua bola di jalur habis selagi masih ada telur. **Kalah:** ketiga telur dicuri, atau waktu habis (jika memakai waktu).

Angka di panel (angka kunci) berganti setiap 3 pasangan yang berhasil. Game memastikan selalu ada bola yang bisa dicocokkan, supaya pemain tidak buntu: sekitar 70% bola tembakan dibuat berpasangan dan 30% sebagai pengecoh, tetapi minimal satu dari peluru dan bola penukar (ketuk naga) selalu punya pasangan.

## Telur, bola telur naga, dan bola tertukar

**Tiga telur sebagai nyawa.** Tiap stage dimulai dengan 3 telur di sarang dan kembali penuh di stage berikutnya. Satu telur dicuri penyihir (dengan animasi energi jahat yang menghisap telur) setiap kali pemain salah menjawab atau ada bola yang sampai di sarang. Bola yang sampai di sarang dihapus, jalur mundur sekitar 4 jarak bola, dan melambat setengah laju selama 4 detik. Setelah telur hilang ada perlindungan 2 detik: tidak ada telur lain yang hilang. Saat tinggal 1 telur, tepi layar berdenyut merah pelan dan naga mengaum. Telur habis berarti kalah. Salah jawab tetap menambah laju jalur 7%.

**Perisai (v2.6).** Setiap 5 jawaban benar berturut-turut (tembakan, bukan pasangan berantai) memberi satu perisai: titik kemajuan di kiri atas layar dan gelembung emas di sekitar telur saat siap. Satu salah jawab berikutnya tidak mengambil telur, lalu perisai pecah; laju jalur tetap naik dan kesalahan tetap tercatat. Perisai tidak menumpuk, tidak menahan bola yang sampai di sarang, dan kembali kosong di tiap stage. Salah jawab memutus rentetan.

**Bola telur naga.** Satu per stage, muncul saat sekitar separuh bola awal sudah habis. Telur dititipkan di satu bola angka yang pasangannya bisa dijawab; bola itu bercincin emas dengan lencana "+1" (atau "+500" jika telur sudah 3/3). Kalau pasangannya dijawab benar, telur terbang ke sarang: telur bertambah 1, atau skor +500 jika telur sudah penuh. Jika bola itu sampai di sarang sebelum dijawab, hadiahnya hilang.

**Bola tertukar.** Secara acak, dua bola yang terlihat bertukar posisi. Sebelum bertukar ada tanda 1,5 detik: dua bola bergetar dan bercincin ungu yang mengecil, dengan garis putus-putus dan tanda ⇄ (tidak hanya mengandalkan warna). Jeda antar tukar acak: 14–20 detik di Mudah, 8–14 detik di Menantang. Yang tidak ikut tertukar: bola telur, bola yang sedang dituju peluru, dan bola paling depan. Jika salah satu bola hilang saat tanda menyala, tukar dibatalkan.

## Tiga stage

Setiap stage punya latar, jalur berkelok, dan jumlah bola sendiri; stage 2 dan 3 lebih banyak bola dan sedikit lebih cepat dari stage 1. Stage 3 menambah bos.

| Stage | Latar | Jumlah bola (Mudah / Menantang) | Laju relatif | Yang baru |
| --- | --- | --- | --- | --- |
| 1. Hutan Hijau | Hijau, pohon dan jamur | 22 / 26 | ×1,00 | Peragaan 4 detik tanpa kata di awal |
| 2. Gunung Bersalju | Biru es, salju, pohon cemara, boneka salju, dan penguin | 24 / 29 | ×1,08 | Jalur miring berkelok seperti jalan setapak gunung, warna jalur putih salju |
| 3. Gunung Api | Ungu gelap, lava dan kelelawar | 24 / 29, lalu bertambah | ×1,05 | Penyihir bos dengan bar nyawa |

Bos di stage 3: penyihir berdiri di awal jalur. Bar nyawanya menunjukkan sisa bola dibanding jumlah awal. Setiap 30 detik ia merapal mantra: angka di panel berganti, 1 bola ditambahkan di ujung rantai, dan muncul tulisan "Mantra baru!". Pemain menang dengan menghabiskan semua bola. Karena ikon penyihir besar bisa menumpuk dengan tulisan di pojok layar, di stage 3 tulisan itu diberi latar gelap tembus pandang supaya tetap terbaca.

Jumlah bola dasar dan laju dasar di tabel dikali pengali stage; angka persisnya ada di bagian rincian pengembangan.

**Jalur dan posisi acak (layout tegak).** Tiap stage punya 3 jalur tegak (total 9 variasi) dengan panjang setara (selisih paling banyak 7%). Satu jalur dipilih acak saat stage dimulai dan tetap sama jika pemain mengulang stage setelah kalah; permainan baru mengacak lagi. Naga berada di tengah bawah layar atau di tengah layar (naga tengah menembak ke segala arah), dan sarang telur di tempat berbeda tiap jalur. Layout lebar punya satu jalur per stage (lihat bagian Layout tegak dan lebar).

Aturan perancangan jalur: di layar standar (tinggi dunia 1000) sarang paling jauh 260 satuan dari naga, jarak sarang dari tempat bola masuk paling sedikit 450 satuan, dan jalur tidak lewat dekat naga (kecuali menuju sarang). Di layar HP yang tinggi (tinggi dunia sampai 1300) jarak sarang ke naga bisa sampai sekitar 370 satuan; ini hanya soal tata letak dan tidak memengaruhi permainan. Di stage 3, penyihir berdiri dekat tempat bola masuk. Aturan yang sama berlaku untuk jalur lebar.

## Layout tegak dan lebar

Game punya dua layout dengan jalur yang digambar khusus untuk masing-masing, supaya terasa dirancang untuk layarnya dan tidak sekadar diperbesar. Mekanik, jumlah bola, laju, telur, perisai, dan bos sama di keduanya.

| | Tegak | Lebar |
| --- | --- | --- |
| Dunia (satuan game) | lebar 600, tinggi 1000–1300 menyesuaikan layar | 1000 × 600 tetap |
| Dipakai di | HP berdiri, tablet tegak, jendela sempit | laptop, PC, HP mendatar |
| Jalur | 3 per stage (total 9), dipilih acak | 1 per stage (total 3) |
| Naga | tengah bawah atau tengah layar | tengah bawah |

- **Pemilihan layout:** lebar layar lebih besar dari tingginya → lebar; selain itu tegak. Dengan batas ganda 5%: masuk lebar saat lebar ≥ 1,05 × tinggi, kembali tegak saat lebar ≤ 0,95 × tinggi, dan di antaranya layout tidak berganti (supaya tidak berkedip di layar hampir persegi).
- **Jalur lebar:** panjang 2037 (stage 1), 2036 (stage 2), dan 2651 (stage 3), setara jalur tegak di stage yang sama (selisih paling banyak 7%). Semua aturan jalur terpenuhi: jarak antar-baris ≥100, jalur ≥100 dari naga, sarang ≤260 dari naga, jarak masuk ke sarang ≥450, dan di stage 3 bos ≤200 dari tempat bola masuk. Bola masuk dari 60 satuan di luar layar (dari kiri di stage 1, dari kanan di stage 2 dan 3). Stage 2 hanya miring sekitar 2,5° (di tegak sekitar 6,7°) karena tinggi dunia 600.
- **Tampilan lebar:** latar gelap tembus pandang di belakang HUD di semua stage (jalur lewat tepat di bawahnya), petunjuk bawah dua baris di kiri-bawah, dan tulisan melayang global sedikit lebih tinggi. Latar halaman di luar dunia ikut warna tema stage.
- **Layout berganti di menu, cerita, dan layar selesai:** hanya tampilan yang berganti, posisi bola dihitung ulang dari jaraknya di jalur.
- **Layout berganti saat spanduk stage atau peragaan:** belum ada kemajuan yang bisa hilang, jadi stage disusun ulang diam-diam untuk layout baru.
- **Layout berganti saat bermain:** layout terkunci dan game berhenti penuh (jalur, peluru, waktu, mantra bos, hitung mundur tukar, perisai). Tampil pesan "Putar layar kembali" ke posisi tegak atau mendatar dengan ikon HP yang berputar (di komputer: ubah ukuran jendela kembali). Game lanjut otomatis begitu layout semula kembali; skor, telur, perisai, dan posisi bola tidak berubah.
- **Layar pendek dan lebar** (tinggi sampai 780 piksel, termasuk HP mendatar): menu jadi dua kolom dan jarak dirapatkan; di tinggi sampai 400 piksel dirapatkan lagi. Menu, cerita, layar selesai, dan tinjauan muat tanpa digulir di HP mendatar setinggi 360–430 piksel.
- **Pengaman:** satu konstanta `LAYOUT_LEBAR_AKTIF`. Bila diset salah, game kembali seperti sebelum layout lebar ada (selalu tegak, dan layar "Putar HP" muncul di HP mendatar yang pendek).

## Layar sambutan, suara, dan menu Jeda

**Urutan layar:** layar sambutan → menu kategori → cerita (3 slide) → stage 1. Layar sambutan tampil pertama setiap halaman dibuka dan tidak ada jalan kembali ke sana. Ketukan ganda cepat pada "Mulai Main" tidak langsung menekan tombol di menu (pengaman 350 milidetik).

**Layar sambutan.** Judul besar "Naga Penjaga"; naga besar di tengah yang naik-turun pelan, telur di depannya, penyihir kecil miring dengan kilau ✨ di kanan atas, dan bola angka warna-warni melayang di tepi kiri dan kanan. Latar langit biru di atas dan rumput hijau di bawah, penuh layar; isi berada di kolom sekitar 480 piksel di tengah (di HP mendatar pendek: judul dan tombol di kiri, gambar di kanan). Satu tombol besar "Mulai Main" yang berdenyut pelan, tanpa tulisan "Ketuk untuk mulai" dan tanpa tombol suara. Tidak ada logo atau karakter pihak lain. Semua yang sering diubah ada di Bagian 1: `SPLASH` (judul, tulisan tombol, lebar kolom, jumlah dan ukuran bola, warna, kecepatan gerak naga, penyihir, bola, dan tombol) dan `SPLASH_ART` (gambar naga, telur, penyihir, kilau). Untuk mengganti emoji dengan gambar resmi, isi baris di `SPLASH_ART` dengan nama berkas gambar di folder yang sama (mis. `'naga.png'`); hanya di situ.

**Musik dan efek suara.** Semua dibuat kode (Web Audio), tanpa berkas dan tanpa jaringan. Dua lagu: riang untuk layar sambutan, menu, dan cerita; lebih tenang dan bergerak untuk bermain (spanduk, peragaan, bermain, layar selesai). Peralihan antar lagu halus (0,7 detik). Efek suara: tembak, ledak (pasangan cocok; nada naik bila rentetan panjang), salah, telur dicuri, menang, dan kalah. Musik dikecilkan saat menu Jeda terbuka (30%) dan di layar selesai (50%), dan semua suara berhenti saat tab disembunyikan. Browser baru mengizinkan suara setelah ketukan pertama pemain; sebelum itu game senyap. Volume diatur di `AUDIO` di Bagian 1 (keseluruhan 0,5; musik 0,5; efek 0,8) dan sengaja pelan. Pengaman: `AUDIO_AKTIF = false` mematikan semua suara dan menyembunyikan tombol Musik dan Suara.

**Tiga tombol pengaturan** (bahasa sederhana, tulisan Nyala / Mati, bawaan semuanya Nyala): 🎵 Musik, 🔊 Suara (efek suara), ✨ Efek gambar (percikan ledakan, denyut merah di tepi layar saat telur terakhir, naga bergetar saat mengaum, penyihir yang membesar saat merapal, denyut cahaya telur emas, gerak di layar sambutan; tulisan dan angka tetap ada). Efek gambar otomatis mati bila perangkat meminta gerak dikurangi. Pilihan tersimpan di browser (`localStorage`; bila diblokir, game tetap jalan dengan pilihan bawaan). Letak: di menu kategori, di pojok kanan atas di luar kotak pilihan (satu baris di layar tinggi, lajur tegak di kanan di layar pendek ≤ 430 piksel), langsung bisa diubah tanpa membuka kotak baru; di dalam game, di menu Jeda. Semua tombol minimal 44 piksel.

**Menu Jeda.** Di dalam game, tombol ✕ di pojok kanan atas diganti tombol ⏸ di tempat yang sama (area ketuk sama, ±48 piksel). Menu Jeda menghentikan game dan berisi: ▶ Lanjut main; ↻ Mulai ulang (stage ini diulang dari awal: jalur sama, telur penuh, skor stage 0, skor total tetap); 🏠 Ke menu (langsung, tanpa pertanyaan kedua; di menu tertulis bahwa kemajuan permainan itu hilang); dan tiga tombol pengaturan di atas. Tidak ada tombol lain. Dialog lama "Keluar ke menu?" sudah diganti.

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

Angka bola hanya dibuat bila punya pasangan di salah satu angka panel. Ini terasa saat hanya "× Kali" yang dipilih (sendirian, atau bersama jenis bilangan lain): di Mudah angka 5 dan 7 tidak dipakai, dan di Menantang angka 1, 7, dan 11 tidak dipakai, karena tidak ada angka panel kali yang bisa dipasangkan dengannya. Pada kombinasi hitungan lain semua angka tetap dipakai.

Tiga jenis bilangan tambahan ada di tingkat Mudah dan Menantang, dengan angka lebih kecil di Mudah. Ketiganya dimainkan dengan cara menjumlahkan dua bola; angka di panel tetap berbentuk ◯ + ◯ = hasil.

| Jenis | Tingkat | Bola di jalur | Angka panel | Contoh |
| --- | --- | --- | --- | --- |
| Bilangan bulat | Mudah | −5 sampai 5, tanpa 0 | 1–3 dan −1 sampai −3 | 3 + (−2) = 1 |
| Bilangan bulat | Menantang | −9 sampai 9, tanpa 0 | 1–5 dan −1 sampai −5 | 5 + (−3) = 2 |
| Desimal | Mudah | 0,1 sampai 0,5 | 0,6 sampai 1,0 | 0,2 + 0,4 = 0,6 |
| Desimal | Menantang | 0,1 sampai 0,9 | 0,8 sampai 1,3 | 0,3 + 0,7 = 1,0 |
| Pecahan (penyebut sama) | Mudah | 1/penyebut sampai (penyebut−1)/penyebut; penyebut 3, 4, 5 untuk stage 1, 2, 3 | penyebut−1, 1, dan penyebut+1 per penyebut (stage 1: 2/3, 1, 4/3) | 1/3 + 2/3 = 1 |
| Pecahan (penyebut sama) | Menantang | sama; penyebut 4, 5, 6 untuk stage 1, 2, 3 | sama (stage 1: 3/4, 1, 5/4) | 1/4 + 3/4 = 1 |

Bola ditulis bersusun (pembilang di atas penyebut). Bola hanya cocok dengan bola sejenis; menembak bola beda jenis menampilkan "Beda jenis bilangan". Jika jenis dicampur, jalur diperlambat (2 jenis ×0,92; 3 jenis ×0,82; 4 jenis ×0,78) dan tiap jenis punya warna sendiri.

## Tingkat, waktu, dan kesalahan

- **Mudah:** bola lebih sedikit, jalur lebih pelan (laju dasar 8), angka kecil, dan ada bantuan: setelah 2 tembakan salah berturut-turut, satu bola yang cocok berdenyut dengan lingkaran.
- **Menantang:** bola lebih banyak (26), jalur sedikit lebih cepat (laju dasar 9), angka lebih besar, tanpa bantuan berkedip.
- **Dengan waktu:** 5 menit per stage; waktu habis berarti stage diulang. **Tanpa waktu:** tampil "∞ Tanpa waktu".
- **Kesalahan:** tiap salah mengambil 1 telur (lihat bagian Telur) dan menambah laju jalur 7%, dengan batas ×1,8. Laju ditampilkan di layar (misalnya "Laju ×1.00").
- **Bintang tiap stage:** 3 bintang jika sisa telur 2–3 dan ketepatan 80% ke atas; 2 bintang jika sisa telur 2–3 atau ketepatan 60% ke atas; selain itu 1 bintang. Skor total terkumpul sepanjang 3 stage.
- **Kalah:** telur habis atau waktu habis. Stage bisa diulang langsung dari layar kalah, dengan jalur yang sama dan telur penuh kembali.

## Tinjauan jawaban (v2.6)

Setelah stage selesai atau saat kalah ("justru saat kalah anak butuh belajar"), popup stage punya tombol "📝 Lihat jawabanmu". Layar tinjauan terpisah dari popup supaya popup tidak padat dan momen hadiah tetap utuh. Awalnya hanya kesalahan yang tampil, dengan tombol "Lihat semua". Tiap kartu memuat soal, persamaan yang ditembakkan ("Belum pas: 1 + 5 = 6"), dan petunjuk pasangan yang pas. Layar ini hanya dibaca; menjawab ulang belum ada karena waktu sempit. Jika tidak ada kesalahan tampil "Tidak ada kesalahan. Hebat!".

## Kejelasan untuk anak 6–14 tahun

Prototipe awal membingungkan karena "angka kunci" tidak jelas. Empat perbaikan disetujui dan sudah dipasang:

1. **Panel persamaan bergambar:** ◯ + ◯ = 10 menunjukkan bahwa dua bola harus dijumlahkan menjadi 10.
2. **Peragaan 4 detik tanpa kata** di awal stage 1, supaya tidak perlu membaca aturan.
3. **Persamaan sebagai umpan balik:** setelah menembak, tampil persamaan nyata (misalnya 4 + 6 = 10), sehingga anak melihat kenapa cocok atau tidak.
4. **Bantuan berkedip di tingkat Mudah** setelah 2 salah berturut-turut.

Prinsip yang dipakai: sedikit teks, banyak isyarat gambar, dan contoh. Anak usia 6–8 tahun masih belajar membaca, jadi petunjuk utamanya harus berupa gambar. Saat jenis bilangan dicampur, bola dan lubang di panel diberi warna yang sama per jenis (asli hijau-biru, bulat biru, desimal merah muda, pecahan ungu), supaya anak tahu bola mana yang dicari.

Perlindungan salah ketuk dan layar kecil: tombol ⏸ di pojok kanan atas membuka menu Jeda (Lanjut main, Mulai ulang, Ke menu) dan menjeda permainan; area ketuknya minimal sekitar 48 piksel. HP yang dipegang mendatar memakai layout lebar, dan menu serta layar lain dipadatkan di layar pendek supaya muat tanpa digulir. Bila layar diputar saat bermain, game berhenti dan meminta layar dikembalikan (lihat bagian Layout tegak dan lebar). Teks kecil di dalam game ikut membesar di layar kecil (minimal sekitar 11 piksel).

Catatan: belum ada uji dengan anak sungguhan.

## Status dan hasil uji

Versi 2.6 lengkap dari menu sampai layar tamat. Semua angka pemain di bagian ini diukur dengan pemain robot, bukan anak-anak, jadi hanya petunjuk awal. Hasil uji robot sebelum sistem telur tidak dicantumkan lagi karena sudah tidak berlaku.

**Sistem telur (v2.5, 9 November 2026).** Robot menembak tiap 2,5–4,5 detik dengan tingkat salah acak tertentu (10 percobaan per sel; ini bukan anak sungguhan). Jumlah menang dari 10 di Menantang stage 1 / 2 / 3:

| Salah | Sebelum ada telur | Sesudah telur (saat ini) | Usulan A: telur hilang tiap 2 salah | Usulan B: perisai setelah 5 benar berturut-turut |
| --- | --- | --- | --- | --- |
| 5% | 10 / 10 / 10 | 10 / 10 / 7 | tidak diuji | tidak diuji |
| 10% | 10 / 10 / 10 | 5 / 4 / 5 | 10 / 10 / 10 | 8 / 10 / 7 |
| 15% | 10 / 10 / 10 | 7 / 4 / 4 | 10 / 9 / 7 | 8 / 10 / 10 |
| 25% | 10 / 10 / 8 | 2 / 1 / 0 | 8 / 5 / 3 | 5 / 1 / 2 |

Di Mudah (stage 1 / 2 / 3) dengan salah 15%: sebelum telur 10 / 10 / 10, sesudah 7 / 8 / 4; dengan salah 25%: 10 / 10 / 10 menjadi 7 / 2 / 1. Bola telur naga berhasil diambil pada 5–10 dari 10 percobaan (lebih jarang di stage 3 dan saat salah tinggi). Temuan: sistem telur membuat game jauh lebih ketat daripada sebelumnya; usulan A dan B diuji pada salinan.

**Ukur ulang v2.6 (perisai + bola penukar berpasangan).** Jumlah menang dari 10 (robot, bukan anak), Menantang stage 1 / 2 / 3:

| Salah | v2.5 (telur saja) | v2.6 (telur + perisai) |
| --- | --- | --- |
| 5% | 10 / 10 / 7 | 10 / 10 / 10 |
| 10% | 5 / 4 / 5 | 10 / 9 / 9 |
| 15% | 7 / 4 / 4 | 7 / 9 / 7 |
| 25% | 2 / 1 / 0 | 4 / 2 / 2 |

Telur sisa rata-rata pada Menantang stage 3 dengan salah 25%: 1,0. Perisai terutama menolong pemain yang cukup baik; robot yang sangat sering salah tetap kesulitan.

**Uji otomatis (9 November 2026).** Halaman uji memainkan game sungguhan di browser: 95 uji mencakup angka dan hitungan, tabel stage, tembak dan kesalahan, perisai, telur, tukar posisi, bos, layar tinjauan, jalur, menu dan cerita, layout tegak dan lebar (pemilihan layout, batas ganda 5%, aturan jalur lebar, jeda dan pulih saat layar berganti, 300 kali ubah ukuran cepat, dan layar pendek), serta 18 uji untuk layar sambutan, pengaturan, menu Jeda, dan suara (lihat di bawah). Hasilnya: 88 lulus, 0 gagal, 5 hanya berupa angka, dan 2 uji animasi yang hanya jalan bila halaman uji dibuka di tab terdepan.

**Uji layar sambutan, pengaturan, Jeda, dan suara (18 uji).** Layar sambutan tampil pertama dengan isi yang benar dan tanpa tombol suara; alur sambutan → menu → cerita → stage 1 tanpa jalan kembali; ketukan ganda tidak menekan tombol menu; tombol pengaturan tersimpan dan terbaca lagi setelah halaman dimuat ulang, sinkron antara menu dan menu Jeda; Efek gambar mati menghentikan percikan dan gerak splash; Efek gambar bawaan mati saat perangkat meminta gerak dikurangi; menu Jeda berisi tepat tombol yang disepakati; Mulai ulang mengembalikan stage yang sama (jalur sama, telur penuh, skor stage 0, skor total tetap) dan Ke menu langsung; tombol ⏸ digambar di tempat ✕ (dicek per piksel); efek suara terpasang di tempat yang benar (tembak, ledak, salah, telur dicuri, menang, kalah); tidak ada AudioContext sebelum ketukan pertama, lagu berganti menu ↔ main, volume turun saat Jeda; tab disembunyikan menghentikan suara; `AUDIO_AKTIF = false` mematikan semuanya. Bunyi diukur di konteks suara tanpa speaker: kedua lagu dan keenam efek menghasilkan bunyi (tidak senyap), tidak meluap (puncak musik sekitar 0,11 dan 0,15 dari penuh; puncak efek 0,11 sampai 0,25), dan pelan. Tata letak diperiksa di 10 ukuran (360×740, 390×844, 768×1024, 1366×768, 1280×720, 1024×576, 844×390, 667×375, 800×360, 932×430): layar sambutan penuh layar tanpa saling menimpa dan kolom ≤ 480 piksel; tombol pengaturan di pojok kanan atas tanpa menimpa kotak menu; menu Jeda muat tanpa digulir. Semua ini hanya mengukur perilaku dan angka; telinga manusia belum menilai suara. Pemain robot yang selalu membidik pasangan benar (4 atau 6 detik per tembakan) memainkan ratusan permainan di semua stage dan tingkat, di kedua layout, serta satu permainan penuh stage 1 sampai 3 di masing-masing layout; hasilnya tidak ada bola tanpa pasangan, tidak ada saat tanpa peluru yang berguna, tidak ada peluru yang jenisnya tidak cocok dengan panel, dan tidak ada galat halaman. Karena robot ini selalu memilih jawaban benar, ia tidak mengukur kesulitan untuk anak. Layout tegak terbukti tidak berubah oleh penambahan layout lebar: panjang jalur, posisi naga dan sarang, bos, jumlah bola, laju, isi latar, dan bola pertama sama dengan rekaman sebelumnya (18 perbandingan, 0 beda).

**Layout lebar dibanding tegak (robot yang kadang salah).** Robot menembak tiap 2,5–4,5 detik dengan tingkat salah acak tertentu, Menantang dengan + − × ÷, 40 percobaan per sel (ini robot, bukan anak). Jumlah menang dari 40, stage 1 / 2 / 3:

| Salah | Tegak | Lebar |
| --- | --- | --- |
| 5% | 39 / 40 / 40 | 40 / 40 / 40 |
| 10% | 38 / 38 / 36 | 40 / 39 / 35 |
| 15% | 38 / 32 / 31 | 35 / 32 / 31 |
| 25% | 22 / 15 / 14 | 18 / 17 / 14 |

Total menang: tegak 383 dan lebar 381 dari 480. Selisih per sel paling besar 4 dari 40. Jadi tingkat kesulitan layout lebar setara dengan tegak menurut robot ini. Dengan hanya 10 percobaan per sel, dua kali jalan memberi selisih yang berbeda-beda (kebisingan), karena itu jumlah percobaan dinaikkan.

**Tampilan.** Tangkapan layar di lebar 360, 390, 768 piksel (tegak) serta 844×390, 1024×600, dan 1024×576 (lebar) untuk menu, bermain, spanduk stage, tinjauan, dan layar kalah atau selesai: tidak ada teks terpotong dan tidak ada tombol HTML di bawah 44 piksel. Menu, cerita, layar selesai, dan tinjauan diperiksa otomatis di 11 ukuran, termasuk HP mendatar setinggi 360–430 piksel: tidak ada yang perlu digulir. Ukuran 1920×1080 dan 1280×720 (rasio 16:9 yang sama dengan 1024×576) tidak bisa dipotret utuh di lingkungan uji.

## Rincian untuk pengembangan

Seluruh game ada di satu berkas `index.html` (HTML, gaya, dan JavaScript tanpa pustaka tambahan), digambar di kanvas (area gambar di halaman). Berkas dibagi 12 bagian bertanda komentar (ditambah Bagian 8B untuk pengaturan dan suara); semua angka yang sering diubah ada di Bagian 1 (Pengaturan).

| Bagian | Isi |
| --- | --- |
| 1 | Pengaturan: ukuran bola, jumlah bola, laju, waktu, daftar angka kunci, data stage, tema |
| 2–3 | Alat bantu dan jalur (titik-titik jalur dengan sudut membulat) |
| 4–6 | Keadaan game, hitungan, bola tembakan dan angka panel |
| 7–8 | Alur stage (banner, peragaan, menang/kalah), efek, telur, perisai, tukar posisi |
| 8B | Pengaturan Musik / Suara / Efek gambar (tombol, simpanan), mesin suara (dua lagu, enam efek, penjadwal nada, peralihan lagu, volume jeda, berhenti saat tab tersembunyi) |
| 9–10 | Logika permainan dan menembak |
| 11–12 | Gambar (termasuk tombol ⏸), layar sentuh, layar sambutan, menu, cerita, menu Jeda, pemilihan layout dan jeda saat layout berganti |

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

Penjaga agar tidak buntu: sekitar 70% bola tembakan dibuat sebagai pasangan bola yang bisa dijangkau, game memilih angka kunci yang punya minimal 2 bola cocok, angka bola yang tidak punya pasangan tidak pernah dibuat, dan setiap frame game memeriksa bahwa salah satu dari 2 bola siap tembak (peluru atau penukar) berguna, dengan cadangan yang pasti punya pasangan. Jika angka panel berganti sendiri, kedua bola siap tembak dibuat ulang supaya sejenis dengan panel. Tiap bola dan peluru membawa tanda jenis bilangan; desimal disimpan sebagai bilangan bulat satuan 0,1 dan pecahan sebagai pembilang, supaya tidak ada galat pembulatan. Pengaturan baru di Bagian 1: penyebut pecahan per stage, batas bola bulat dan desimal per tingkat, angka panel jenis baru, dan faktor perlambatan jika jenis dicampur.

Pengaturan telur di Bagian 1: EGGS = 3, PROTECT_T = 2 detik, NEST_PUSH = 216 (4 jarak bola), NEST_SLOW_T = 4 detik, NEST_SLOW = 0,5, EGG_BONUS = 500, EGG_AT = 0,5 (pertengahan stage), SWAP_EVERY (Mudah 14–20, Menantang 8–14 detik), SWAP_WARN = 1,5 detik, SHIELD_AT = 5 jawaban benar berturut-turut.

Pengaturan layar sambutan dan suara di Bagian 1: `SPLASH` (judul, tombol, kolom, bola, kecepatan gerak, warna), `SPLASH_ART` (gambar), `AUDIO_AKTIF` (true/false), `AUDIO` (volume keseluruhan, musik, efek, pengali saat Jeda, lama peralihan lagu), dan `PREF_KEY` (nama simpanan pengaturan). Lagu dan efek suara didefinisikan di Bagian 8B (`TRACKS`, `SFX`); untuk mengubah nada cukup ubah daftar nada di sana.

Pengaturan layout di Bagian 1: `LAYOUT_LEBAR_AKTIF` (true/false), `TEGAK_W` = 600, dan `WIDE` (dunia 1000×600; batas masuk 1,05 dan kembali 0,95). `resize()` memilih layout dan memasang dunia; `syncLayout()` mengunci layout saat bermain dan menjeda game bila layar berganti bentuk.

Tampilan: dunia tegak lebar 600 dengan tinggi menyesuaikan layar (1000–1300), dunia lebar 1000×600; kanvas diskalakan penuh dengan batas ketajaman layar 2,5×. Kontrol memakai pointer events sehingga sentuhan dan mouse sama. Tiap stage menyimpan daftar 3 jalur tegak (titik jalur, posisi naga, posisi bos) dan satu jalur lebar (`wide`) di Bagian 1; jalur tegak terpilih disimpan per permainan. Peluru menembus: peluru mengejar bola sasaran dan mengabaikan bola lain; jika bola sasaran hilang di tengah jalan, peluru menjadi tembakan lurus biasa. Jika halaman dimuat saat ukuran jendela masih 0 (bingkai atau tab tersembunyi), game memakai ukuran cadangan lalu menyesuaikan diri begitu ukuran asli ada. Game tayang sebagai halaman statis di GitHub Pages tanpa proses build.

## Batasan dan rencana lanjutan

Batasan saat ini:

- Belum diuji di HP asli, Safari iPhone, dan sentuhan sungguhan; hanya simulasi dan tangkapan layar ukuran HP.
- Suara hanya diukur otomatis (bunyi ada, tidak meluap, pelan) dan dicek urutan serta pemicunya; enak atau tidaknya di telinga, kenyaringan di speaker HP, dan perilaku Safari iPhone (izin suara, suara berhenti saat layar dikunci) belum didengar langsung. Volume dan nada bisa disetel di `AUDIO` dan `TRACKS`/`SFX`; `AUDIO_AKTIF = false` mematikan semuanya.
- Gambar layar sambutan masih emoji sementara (satu tempat penggantian: `SPLASH_ART`).
- Gambar masih emoji sementara; belum ada gambar resmi karakter dan aturan merek.
- Pecahan hanya berpenyebut sama, tidak disederhanakan (2/4 tetap 2/4), dan belum ada pecahan campuran; jenis baru belum diuji pada anak. Di Mudah penyebut kini 3, 4, 5 (stage 1 memakai ⅓ dan ⅔).
- Layout lebar memakai dunia tetap 1000×600, jadi di layar yang lebih lebar dari rasio 1,67 (misalnya HP mendatar) ada pita kosong di sisi dan bola tampak muncul dari tepi dunia, bukan tepi layar; di layar 4:3 pitanya ada di atas dan bawah. Stage 2 lebar hanya miring sekitar 2,5°.
- Keseimbangan layout lebar hanya diuji dengan robot (setara dengan tegak, lihat bagian Status); belum dicoba dengan pemain sungguhan.
- Konsep "Persamaan Bolong" tidak ada di v2 (hanya di prototipe lama).
- Keseimbangan kesulitan baru diuji dengan robot. Dengan sistem telur, game jauh lebih ketat bagi pemain yang sering salah (lihat tabel di bagian Status); perlu dicoba dengan pemain sungguhan. Angka mundur jalur, perlambatan, dan jeda tukar masih tebakan awal.

Rencana lanjutan:

- [ ] Keseimbangan telur: aturan telur tetap + perisai berlaku sekarang; pelonggaran A (telur hilang tiap 2 salah) masih opsi bila anak yang kesulitan terlalu sering kalah, termasuk Menantang stage 2 dan 3.
- [ ] Pecahan berpenyebut beda.
- [ ] Sembilan jalur lebar (3 per stage seperti tegak) dan dunia lebar yang lentur mengikuti bentuk layar, tanpa pita kosong.
- [ ] Cara mengumpulkan masukan dari pemain.
- [ ] Gambar resmi karakter dan aturan merek.

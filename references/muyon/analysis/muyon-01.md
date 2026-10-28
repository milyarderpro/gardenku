# Video Analysis — Muyon / muyon-01

> **STATUS: `draft` — sudah dianalisis AI dari MP4 asli yang diunggah pengguna, belum ditinjau/disetujui pengguna.** Dokumen ini mengikuti [aturan analisis](../../../rules/analysis.md) dan [template analisis](../../../templates/video-analysis.md). Kategori tanaman atau gerakan yang belum dapat dipastikan ditandai terpisah.

## 1. Reference Information

| Field | Isi |
|---|---|
| Video ID | `muyon-01` |
| Creator / Collection | Muyon (label koleksi, identitas akun asli belum diverifikasi) |
| Input MP4 (chat) | `muyon01(1).mp4` — diunggah pengguna saat analisis, 2026-10-28 |
| Penyimpanan MP4 | PC pengguna; **tidak ada MP4 di repository setelah migrasi v1.1** |
| Bukti cocok historis | Saat MP4 masih berada di repo, ukuran dan SHA Git blob unggahan chat cocok dengan file `muyon-01.mp4` (pemeriksaan 2026-10-28) |
| SHA Git blob historis | `5bc8ff90e091ca7233b633774ac288171edb1465`; **bukan tautan MP4 aktif** |
| File size | 19.234.334 bytes |
| Source URL | URL unggahan Facebook asli belum diketahui; URL repo bukan sumber publikasi asli |
| Rights / Permission | Belum diverifikasi; jangan menganggap video bebas didistribusikan |
| Analysis date | 2026-10-28 |
| Analysis status | **`draft`** — memerlukan peninjauan pengguna |
| Verification Gate Opsi B+ | **Gate A: PASS** untuk cakupan visual; **Gate B: PASS** untuk integritas Git; **Overall: PASS**. Audio belum diaudit dan pratinjau UI GitHub belum diuji langsung. Status tetap `draft` sampai ditinjau pengguna. |
| Evidence checked | [OBSERVASI] MP4 asli: 682 frame terdekode; timeline dipetakan (Pass 1), transisi dan komposisi tiap shot diperiksa ulang (Pass 2); 22 panel dalam empat contact sheet |
| Durasi kontainer MP4 | **22,870 detik** (termasuk audio) |
| Durasi trek video | **22,733 detik** — 682 frame pada 30 FPS |
| Durasi trek audio | **22,870 detik** — lebih panjang dari trek gambar |
| Resolution / Frame rate | **720 × 1280**, **30 FPS** |
| Aspect ratio | **9:16 (vertikal)** |
| Video / audio codec | H.264; audio AAC stereo 44,1 kHz (isi suara belum diaudit secara auditori) |
| Main shot count | **4** (batas waktu perkiraan karena perpindahan singkat/dissolve) |
| Contact sheets folder | [`../frames/muyon-01/`](../frames/muyon-01/) — **4 JPG contact sheet terverifikasi di GitHub**, masing-masing satu per shot (5–6 panel) |

## 2. Overall Description

[OBSERVASI] Video vertikal menampilkan kebun tropis terbuka yang sangat rimbun dan produktif: sayur daun, tomat merah, terong, tanaman rambat, serta sejumlah pohon buah besar tampak dalam susunan berlapis. Bedengan dibatasi bata merah dan dipisahkan jalur tanah/bata yang terlihat lembap; pada bagian lain terdapat kolam bertanaman air, sprinkler, dan aktivitas orang menyiram di dekat ayam. Kamera menampilkan empat bagian kebun dengan pergerakan perlahan untuk mengungkap objek menarik, bukan satu perjalanan maju yang terus-menerus. Cahaya relatif menyebar di bawah langit terang berawan, dengan kontras buah merah/kuning/ungu terhadap dedaunan hijau.

- **Garden type:** [OBSERVASI] `open-field` / kebun terbuka campuran sayur dan buah, bukan bukti kebun depan rumah atau rooftop.
- **Garden size / space:** [INTERPRETASI] Kesan cukup luas dan terorganisasi; **luas dalam meter tidak diketahui**.
- **Visual hook awal:** [OBSERVASI 00:00.00–00:00.02] Banyak durian bergantung di cabang besar, dengan gugusan tomat merah di bedengan bawah.
- **Visual density:** [OBSERVASI] Tinggi: sayuran rendah, tanaman merambat, pohon buah menengah, pohon besar memenuhi beberapa lapisan frame.
- **Overall camera style:** [INTERPRETASI] Slow pan dan pergeseran lateral halus; pan vs gerak kamera berpindah posisi tidak selalu dapat dipisahkan secara pasti dari rekaman.
- **Distinctive character:** Lapisan vertikal pohon buah–sayuran; batas bedengan bata; kombinasi tanah basah, kolam, penyiraman, dan aktivitas kebun.

## 3. Shot Breakdown

**Shot Map — hasil pemeriksaan MP4 dua tahap:**

| Shot | Waktu awal–akhir (perkiraan) | Durasi | Bukti transisi | Contact sheet |
|---|---|---:|---|---|
| 01 | 00:00.00–00:05.60 | ±5,6 dtk | 05.35–05.55 masih durian; 05.75 sudah adegan kebun berbeda | [`shot-01.jpg`](../frames/muyon-01/shot-01.jpg), 6 panel |
| 02 | 00:05.60–00:11.60 | ±6,0 dtk | 11.35–11.55 pohon buah/orang; 11.75 sudah sprinkler | [`shot-02.jpg`](../frames/muyon-01/shot-02.jpg), 6 panel |
| 03 | 00:11.60–00:16.60 | ±5,0 dtk | 16.35–16.55 kolam; 16.75 sudah kelapa/bedengan | [`shot-03.jpg`](../frames/muyon-01/shot-03.jpg), 5 panel |
| 04 | 00:16.60–00:22.57 | ±6,0 dtk | Setelah ±22.57 layar menjadi hitam | [`shot-04.jpg`](../frames/muyon-01/shot-04.jpg), 5 panel |

Batas transisi **perkiraan** karena perpindahan lembut; tidak diklaim sebagai hard cut presisi. Bagian 00:22.57–00:22.87 adalah penutup hitam, bukan shot kebun kelima. Pan dibanding tracking tetap **interpretasi** bila bukti gerakan belum cukup untuk membedakannya.

**Catatan timestamp:** Batas perpindahan sekitar **00:05.6, 00:11.6, dan 00:16.6 detik** adalah **perkiraan** berdasarkan pemeriksaan frame. Ada perpindahan lembut (mirip dissolve) sehingga tidak diklaim sebagai hard cut tepat pada satu frame. Mulai sekitar 00:22.57 gambar menjadi hitam hingga akhir **trek video (±22.73 detik)**, bukan shot kebun kelima; kontainer MP4 masih memiliki audio sampai ±22.87 detik.

### Shot 01 — Durian di atas bedengan tomat

- **Timestamp:** `00:00.00–00:05.6` (perkiraan; durasi ±5,6 detik).
- **Hero subject:** [OBSERVASI] Batang dan cabang pohon durian dengan banyak buah berduri yang menggantung.
- **Supporting subjects:** [OBSERVASI] Tomat merah/oranye dan sebagian masih hijau di depan; sayur daun hijau dan kemerahan, tanaman merambat pada penyangga, pohon palem/kelapa pada latar.
- **Visual hook:** Buah durian berukuran besar di atas, buah tomat merah kontras di lapisan bawah sejak awal.
- **Camera movement:** [INTERPRETASI] Slow pan ke kanan / pergeseran sedikit menyamping; batang durian bergeser dari dekat tengah ke kiri frame sambil area tanaman di kanan semakin tampak. **Bukan forward walkthrough yang terus maju.**
- **Speed and stability:** Lambat, cukup stabil dengan gerak ringan.
- **Camera angle and framing:** Medium-wide vertikal pada ketinggian kira-kira mata/dada; pepohonan bagian atas hingga sayuran di tanah masih terlihat dalam satu frame.
- **Composition:** Foreground = tomat dan daun bedengan; middle ground = batang durian, jalur basah, batas bata dan rambatan; background = kanopi hijau/palem dan baris tanaman lebih jauh.
- **Garden layout:** Bedengan berbingkai bata merah, jalur sempit tanah/bata di antaranya, rangka bambu/kayu untuk tanaman rambat; pohon durian tumbuh di sela area kebun.
- **Lighting and colors:** Cahaya mendung/terdifusi, hijau dominan, buah tomat merah sebagai aksen.
- **Weather and surfaces:** Jalur dan tanah tampak basah/lembap; tidak cukup bukti dari shot ini saja untuk memastikan gerimis sedang turun.
- **Action / interaction:** Tidak terlihat manusia atau hewan yang jelas pada shot ini.
- **Audio:** Track tersedia, tetapi konten suara belum dapat diidentifikasi secara auditori.
- **Transition to next shot:** Transisi lembut menuju area kebun berbeda sekitar 00:05.6 detik.

**Perkembangan gambar asli:** Awal menonjolkan pohon durian di tengah dan tomat bawah → kamera bergeser menampilkan lebih banyak rambatan dan bedengan → akhir batang durian semakin di kiri, jajaran tanaman menjadi dominan.

**Bukti & keyakinan:** [OBSERVASI 00:00.35–00:05.35] buah durian berduri, tomat berwarna merah, tepian bata, jalur basah (**tinggi**). [INTERPRETASI] jenis pan vs tracking (**sedang**).

**Teknik yang bisa dipelajari:** Gunakan pohon buah tinggi sebagai kerangka atas dan buah kecil berwarna mencolok sebagai hook di foreground; pergeseran lambat mengungkap lapisan tanpa harus berjalan jauh.

### Shot 02 — Pohon buah, orang menyiram, dan ayam

- **Timestamp:** `00:05.6–00:11.6` (perkiraan; durasi ±6 detik).
- **Hero subject:** [OBSERVASI] Kebun berlapis dengan orang memakai caping menyemprot air melalui selang di antara pohon buah dan bedengan.
- **Supporting subjects:** [OBSERVASI] Cabai/tomat di bawah, sayuran daun, batang jagung, rambatan dengan bunga kuning, pohon pepaya berbuah hijau, beberapa pohon dengan buah kuning lonjong serta gugusan buah merah muda. Ayam cokelat/krem terlihat di tanah; satu sosok manusia lain tampak lebih jauh dalam sebagian rentang.
- **Visual hook:** Lanskap kebun yang terlihat hidup karena aksi menyiram dan buah bergelantungan; jalur bata mengarah ke subjek manusia.
- **Camera movement:** [INTERPRETASI] Pergeseran/pan perlahan ke kanan, bergerak dari area orang menyiram menuju pohon berbuah merah muda dan pemandangan lahan hijau terbuka di kejauhan.
- **Speed and stability:** Lambat sampai sedang, relatif stabil; subjek berganti tanpa cut internal yang jelas.
- **Camera angle and framing:** Wide–medium-wide, sekitar tinggi pengamat berdiri, mempertahankan manusia ukuran kecil hingga sedang di antara tanaman.
- **Composition:** Foreground = sayuran rapat dan batas bata; middle ground = jalur, orang memakai caping, ayam, pohon berbuah; background = barisan pohon dan bentang lahan hijau/ladang di horizon.
- **Garden layout:** Bedengan dengan batas bata, beberapa jalur sempit, rambatan bambu, pohon buah rapat tetapi masih menyisakan ruang jalan; selang air melintang di tanah.
- **Lighting and colors:** Cahaya menyebar; perpaduan hijau daun, kuning buah, merah muda buah, dan pakaian ungu pada sosok dekat kamera.
- **Weather and surfaces:** Tanah lembap; air yang diarahkan orang **berasal dari selang** dan bukan bukti hujan alami.
- **Action / interaction:** [OBSERVASI ±00:07.7] Orang bertopi caping dan celana ungu memegang selang yang mengeluarkan semprotan air. [OBSERVASI ±00:07.7 dan ±00:10.6] Sejumlah ayam kecil terlihat mencari makan/berjalan di tanah dekat jalur; sosok lain memakai caping tampak di kejauhan.
- **Audio:** Isi track belum diverifikasi.
- **Transition to next shot:** Perpindahan lembut sekitar 00:11.6 detik.

**Perkembangan gambar asli:** Awal terlihat orang dan pepaya/pohon buah → tengah memperlihatkan kegiatan menyiram serta ayam di dekat bedengan → akhir kamera menonjolkan pohon dengan gugus buah merah muda, lahan hijau terbuka di latar.

**Bukti & keyakinan:** [OBSERVASI ±00:07.7] orang, caping, selang, semprotan, ayam (**tinggi**); [OBSERVASI ±00:10.6] pohon buah merah muda dan ayam (**tinggi**); [BELUM PASTI] identitas spesies buah merah muda, jenis seluruh ayam, dan jumlah unik orang sepanjang shot.

**Teknik yang bisa dipelajari:** Tempatkan aktivitas manusia/ayam sebagai elemen pendukung, bukan pusat cerita wajib; gunakan kebun dan pohon berbuah sebagai jangkar visual.

### Shot 03 — Tomat, sprinkler, pepaya, dan kolam

- **Timestamp:** `00:11.6–00:16.6` (perkiraan; durasi ±5 detik).
- **Hero subject:** [OBSERVASI] Rumpun tomat merah/oranye berbuah banyak di depan, lalu kolam berdaun teratai/serupa teratai dan semprotan air sprinkler.
- **Supporting subjects:** [OBSERVASI] Tanaman jagung, sayur daun, rangka bambu dengan buah/vegetasi merambat panjang, pohon pepaya dengan buah hijau dan jingga, pepohonan buah lainnya.
- **Visual hook:** Gugusan tomat merah banyak dalam foreground, ditambah semburan air yang membentuk pola kipas melintasi area kebun.
- **Camera movement:** [INTERPRETASI] Pan/pergeseran lateral ke kanan, menggeser perhatian dari tomat dan bedengan menuju pepaya, tanaman rambat, dan kolam.
- **Speed and stability:** Halus, lambat/sedang; tanaman dekat kamera memberi efek parallax/kedalaman.
- **Camera angle and framing:** Medium-wide, sudut pandang agak tinggi dari bedengan depan sehingga kolam di bagian belakang dapat terlihat.
- **Composition:** Foreground = tomat, sayur hijau, batang rambat; middle ground = jagung, pepaya, sprinkler; background = kolam dengan daun bundar dan bunga merah muda/pucat, pepohonan.
- **Garden layout:** Bedengan berbaris rapat dipisahkan jalan tanah, konstruksi bambu vertikal/atas, sumber penyiram di dekat area tanaman, dan kolam terpisah sebagai latar.
- **Lighting and colors:** Langit terang berawan, hijau dominan, tomat merah/oranye dan pepaya jingga kontras; semprotan air terlihat putih.
- **Weather and surfaces:** [OBSERVASI ±00:12.3–00:16.3] **Sprinkler menyemprot air** dengan arah menyebar dari titik penyiram. Tanah/daun terlihat lembap. Pancaran itu tidak boleh dijadikan bukti intensitas gerimis alami.
- **Action / interaction:** [OBSERVASI] Air memancar dari sprinkler, permukaan kolam beriak; bentuk jingga tampak di air sekitar 00:15.9, kemungkinan ikan **tetapi belum dipastikan**.
- **Audio:** Isi track belum diverifikasi.
- **Transition to next shot:** Perpindahan lembut sekitar 00:16.6 detik.

**Perkembangan gambar asli:** Awal rumpun tomat dan bambu → tengah sprinkler menyiram dekat jagung, daun dan kolam → akhir pepaya, tanaman rambat, air kolam dan tanaman hijau semakin jelas.

**Bukti & keyakinan:** [OBSERVASI ±00:13.2–00:15.9] tomat, sprinkler, pepaya dan kolam bertanaman air (**tinggi**). [BELUM PASTI] bentuk jingga di air merupakan ikan, jenis bunga/daun air yang tepat.

**Teknik yang bisa dipelajari:** Padukan foreground berbuah cerah, garis struktur vertikal bambu, gerakan semprotan air yang nyata, dan permukaan kolam di background untuk memperkaya kedalaman.

### Shot 04 — Bedengan terong di bawah pohon kelapa dan mangga

- **Timestamp:** `00:16.6–00:22.57` (perkiraan; durasi gambar kebun ±5,9 detik).
- **Hero subject:** [OBSERVASI] Bedengan sayuran rapi yang mengarah ke pohon buah dengan banyak buah kuning/hijau dan kelapa besar di latar.
- **Supporting subjects:** [OBSERVASI] Terong ungu menggantung di kiri depan, kelompok selada/sayur daun hijau terang, buah hijau bulat pada pohon kiri, mangga hijau–kuning pada pohon tengah, tanaman merambat panjang pada rangka bambu di kanan.
- **Visual hook:** Jalur sempit lurus di tengah membingkai terong dan sayur, kemudian membawa mata ke mangga serta kelapa besar yang memenuhi bagian atas frame.
- **Camera movement:** [INTERPRETASI] Pergeseran/pan lambat dengan penyesuaian arah sedikit ke kanan; bingkai tetap mempertahankan jalur tengah dan hierarki pohon–bedengan, tidak ada perjalanan maju jauh.
- **Speed and stability:** Stabil, lambat, mendekati shot penutup yang tenang.
- **Camera angle and framing:** Wide vertikal, jalur dari bawah frame, tajuk kelapa di atas.
- **Composition:** Foreground = sayur daun hijau terang dan terong; middle ground = jalur basah, batas bata, pohon buah rendah; background = kelapa berbuah dan lapisan pohon lainnya.
- **Garden layout:** Bedengan berpola sejajar, masing-masing bertepi bata merah, koridor basah sempit, pohon buah di ujung koridor, rambatan di sisi kanan.
- **Lighting and colors:** Cahaya mendung terang/tersebar; hijau daun, ungu terong, kuning mangga, cokelat bata.
- **Weather and surfaces:** Jalur tampak basah; tidak ada semburan sprinkler yang jelas pada shot ini.
- **Action / interaction:** Tidak tampak manusia atau hewan yang jelas pada shot ini; gerak alami tanaman tampak ringan.
- **Audio:** Isi track belum diverifikasi.
- **Transition to next shot:** **Tidak ada shot kelima**; sekitar `00:22.57–00:22.87` tampilan berubah menjadi **hitam** (penutup video).

**Perkembangan gambar asli:** Awal langsung memperlihatkan jalur, bedengan, dan kelapa besar → tengah penonjolan buah mangga dan buah hijau kiri melalui gerak lambat → akhir komposisi rimbun stabil sebelum layar hitam.

**Bukti & keyakinan:** [OBSERVASI ±00:19.5] terong ungu, mangga dan kelapa, jalur bata basah (**tinggi**). [BELUM PASTI] identitas pasti buah hijau bulat di pohon kiri (citrus/jeruk atau kerabat), jumlah varietas mangga.

**Teknik yang bisa dipelajari:** Gunakan leading lines jalur dan bedengan untuk membingkai beberapa lapis tanaman; penutup tidak wajib berupa kamera maju sampai jauh.

## 4. Plants, Fruits & Garden Layout

| Elemen | Shot / waktu bukti | Penataan dan ciri visual | Keyakinan |
|---|---|---|---|
| Durian | Shot 01, 00:00.35–00:05.35 | Buah besar berduri menggantung pada cabang di atas sayur | Tinggi |
| Tomat | Shot 01 ±00:02.1, Shot 03 ±00:13.2 | Gugusan buah merah, oranye, dan hijau pada tanaman rendah | Tinggi |
| Terong ungu | Shot 04 ±00:19.5 | Buah ungu panjang di bedengan kiri bawah | Tinggi |
| Jagung | Shot 02 ±00:07.7, Shot 03 ±00:13.2 | Batang tegak berdaun panjang di antara sayuran | Tinggi |
| Pepaya | Shot 02 ±00:07.7, Shot 03 ±00:15.9 | Gugusan buah pada batang; hijau serta jingga | Tinggi |
| Mangga | Shot 02 ±00:07.7; Shot 04 ±00:19.5 | Buah lonjong kuning/hijau menggantung dari pohon | Sedang–tinggi |
| Kelapa | Shot 04 ±00:19.5 | Pohon tinggi dengan tandan buah pada tajuk | Tinggi |
| Pohon dengan buah merah muda berkelompok | Shot 02 ±00:10.6 | Gugusan kecil bergantung di antara daun | Jenis belum pasti |
| Buah hijau bulat pada pohon | Shot 04 ±00:19.5 | Tumbuh berkelompok pada pohon kiri | Jenis belum pasti |
| Selada/sayur daun; tanaman rambat | Semua shot, terutama 01, 03, 04 | Hamparan daun rendah, rambatan pada bambu, beberapa bunga kuning | Bentuk jelas; sebagian identifikasi spesies belum pasti |
| Batas bedengan dan jalan | Seluruh video | Tepi bata merah, jalur tanah/bata lembap | Tinggi |
| Kolam dan tanaman air | Shot 03 ±00:13.2–00:15.9 | Air terbuka, daun bundar mengapung, beberapa bunga | Tinggi |

**Struktur lapisan:** [OBSERVASI] Sayur daun/tomat/terong rendah di depan → tanaman rambat/jagung dan buah pada pohon kecil di tengah → pohon durian, mangga, kelapa dan vegetasi lebih tinggi di belakang/atas.

**Ciri penataan penting:** Tanaman sengaja dikelompokkan menjadi bedengan berbatas; pada beberapa shot, pohon buah tumbuh berdekatan dengan tanaman sayuran sehingga visual terasa penuh tanpa kehilangan jalur perawatan.

## 5. Weather, Atmosphere & Lighting

- **Waktu:** [BELUM PASTI] Siang/pagi/sore tidak bisa ditentukan pasti hanya dari gambar.
- **Cuaca:** [OBSERVASI] Langit cenderung pucat/berawan; bayangan tidak keras; tanah dan sejumlah permukaan terlihat basah.
- **Konteks sebelumnya:** [KONTEKS PENGGUNA] Pengguna sebelumnya menjelaskan suasana sesudah hujan deras dan masih gerimis. Pernyataan ini **konteks pengguna**, bukan hasil pengukuran hujan melalui video.
- **Light quality:** [OBSERVASI] Cahaya alami lembut/terdifusi dengan dominasi warna hijau; tidak tampak sinar matahari langsung yang kuat.
- **Wet surfaces:** [OBSERVASI] Jalan tanah/bata lembap dan kadang memantulkan cahaya; beberapa daun terlihat basah.
- **Water source:** [OBSERVASI] Shot 02: selang dipegang orang yang menyiram. Shot 03: sprinkler menyemburkan air dari titik yang tetap. Kolam merupakan badan air terpisah.
- **Gerimis alami:** [BELUM PASTI] Sulit dibuktikan dari gambar terpisah, terutama karena ada air dari selang/sprinkler. **Jangan menyamakan semprotan alat dengan gerimis.**
- **Atmosphere / mood:** [INTERPRETASI] Sejuk, subur, terasa habis disiram atau hujan, penuh kehidupan.
- **Relevant motion:** Air menyemprot, sedikit gerak daun, riak permukaan kolam.

## 6. Animals, Humans & Other Objects

| Subjek / objek | Jumlah teramati | Shot / posisi | Aktivitas / interaksi | Peran |
|---|---|---|---|---|
| Orang memakai caping, baju abu-abu dan celana ungu | Setidaknya 1 sosok jelas | Shot 02 ±00:07.7, dekat jalur | Memegang selang dan menyiram area tanaman | Pendukung |
| Orang bercaping di kejauhan | Sosok tambahan terlihat; apakah orang berbeda belum pasti | Shot 02 ±09–11, belakang bedengan | Berada di area kebun, dekat semprotan air | Latar |
| Ayam cokelat/krem | Setidaknya 2 terlihat pada beberapa frame; jumlah unik tidak dipastikan | Shot 02 ±00:07.7 dan 00:10.6, di tanah | Berjalan/menjelajah dekat jalur dan pepohonan | Pendukung |
| Bentuk jingga menyerupai ikan | Tidak pasti | Shot 03 ±00:15.9, di kolam | Terlihat di bawah/permukaan air; spesies dan gerak belum diverifikasi | Detail latar, belum pasti |
| Selang air | 1 jalur selang tampak, jumlah alat tidak dipastikan | Shot 02 | Menyuplai semburan saat orang menyiram | Pendukung |
| Sprinkler | Setidaknya satu titik semprotan aktif | Shot 03 | Pancaran kipas air menuju tanaman | Pendukung |
| Rangka bambu/kayu | Beberapa | Shot 01–04 | Menopang rambatan, menjadi garis vertikal | Struktur visual |

**Realism notes:** Orang dan ayam berada pada tanah/jalur; air dari selang dan sprinkler mempunyai arah semprotan konsisten. Tidak tampak interaksi yang membuktikan identitas orang maupun hubungan dengan hewan. Keberadaan hewan dan orang **bukan elemen wajib** untuk ide Gardenku lain.

## 7. Audio, Editing & Pacing

- **Audio checked:** [OBSERVASI TEKNIS] Ada stream audio AAC stereo 44,1 kHz di dalam file. **Isi suara belum diverifikasi secara auditori.**
- **Natural sound:** **Belum dapat dipastikan.** Tidak menyatakan ada/tidaknya suara hujan, burung, ayam, langkah, atau air hanya dari gambar.
- **Voice / music:** **Belum dapat dipastikan** tanpa mendengarkan/menganalisis track audio secara auditori.
- **Shot rhythm:** [OBSERVASI] 4 shot, masing-masing sekitar 5–6 detik; susunan dimulai dengan hook buah, beralih ke aktivitas dan pohon buah, lalu air/kolam, dan berakhir dengan tata bedengan.
- **Transitions:** [OBSERVASI] Perpindahan lembut pada ±00:05.6, 00:11.6, 00:16.6; bagian akhir menjadi layar hitam ±00:22.57. [INTERPRETASI] Efeknya mirip dissolve singkat, tetapi durasi eksak transisi belum dihitung frame demi frame.
- **What makes editing effective:** [INTERPRETASI] Setiap shot memperkenalkan kombinasi visual berbeda tanpa harus mengulang jalur kamera yang sama; objek cerah di foreground menjadi hook dan pohon buah di background memberikan skala serta kedalaman.

## 8. Visual Characteristics & Reusable Inspiration

**Karakter visual terpenting (maks. 5):**
1. **Layered edible garden:** sayur, rambatan, dan pohon buah tinggi muncul dalam komposisi yang sama (Shot 01, 04).
2. **Fruit-first framing:** durian, tomat, pepaya, mangga, serta terong menjadi penarik perhatian dengan bentuk/warna jelas (Shot 01–04).
3. **Organized lushness:** bedengan bata dan koridor sempit membuat kebun sangat penuh tetap terbaca rapi (Shot 01, 02, 04).
4. **Water and wet-ground atmosphere:** tanah basah, selang, sprinkler, kolam memperkuat rasa kebun hidup (Shot 02–03).
5. **Slow visual reveal:** pergeseran/pan kamera menyorot kelompok tanaman berbeda secara bertahap; antarklip memiliki objek utama yang berlainan (Shot 01–04).

**Teknik yang dapat digunakan kembali:**
- Mulai shot dengan buah yang kuat secara bentuk/warna dalam foreground, sambil mempertahankan pohon buah sebagai skala (Shot 01).
- Bergerak pelan ke samping untuk menyingkap tanaman dan struktur baru, tanpa selalu berjalan maju (Shot 01–03).
- Gunakan aktivitas manusia/ayam sebagai konteks alami di tengah kerimbunan, bukan adegan utama wajib (Shot 02).
- Jadikan air dari sprinkler dan kolam unsur gerak sekunder, dengan sumber air yang logis (Shot 03).
- Bingkai jalur bedengan sebagai leading lines menuju pohon yang sarat buah (Shot 04).

**Elemen opsional, bukan ciri wajib:** Durian, orang memakai caping, ayam, kolam, sprinkler, pepaya dan buah spesifik. Tidak perlu digabungkan seluruhnya dalam satu video baru.

**Hal yang perlu dihindari:** [INTERPRETASI] Kelebihan jumlah objek/varietas dalam kebun sempit, perpindahan shot yang mengubah identitas lokasi tanpa kontinuitas, serta penyamaan sprinkler dengan gerimis alami.

**Search tags (dengan bukti visual):** `open-field`, `lush-garden`, `mixed-edible-garden`, `brick-bordered-beds`, `wet-path`, `soft-diffused-light`, `durian`, `tomato`, `eggplant`, `papaya`, `coconut`, `sprinkler`, `pond`, `human-watering`, `chickens`, `slow-camera-reveal`.

## 9. Notes & Uncertainty

- **Sumber historis:** Pada 2026-10-28 MP4 unggahan chat (19.234.334 byte, SHA Git blob `5bc8ff90e091ca7233b633774ac288171edb1465`) cocok dengan MP4 yang **ketika itu** tersimpan di repo. Setelah migrasi, MP4 tidak lagi ada di tree branch; pemilik menyimpan file asli di PC.
- **Two-Pass:** Kontainer MP4 berdurasi **22,870 detik**; trek gambar **22,733 detik** (682 frame pada 30 FPS), sedangkan audio 22,870 detik. Sampling timeline dan peninjauan ulang tiap shot/transisi dilakukan sekitar 05.6, 11.6, 16.6 detik; batas transisi tetap perkiraan.
- **Gerak kamera:** Pergeseran komposisi dominan perlahan ke samping; pan vs tracking tidak selalu dapat dipastikan, karenanya tetap berlabel `[INTERPRETASI]`.
- **Ketidakpastian lain:** Identifikasi sebagian buah merah muda/hijau dan bentuk jingga di kolam belum pasti. Tanah basah dan sprinkler tidak cukup untuk mengonfirmasi gerimis alami. Sumber publikasi dan izin penggunaan frame belum diketahui.
- **Audio:** Audio AAC ada, tetapi isi suara **belum diperiksa secara auditori**; Gate A hanya untuk cakupan analisis visual.
- **Kualitas gambar:** Semua panel diekstrak dari MP4 720×1280 dan disusun sebagai contact sheet standar berpanel **540×960** (rasio 9:16), dalam rentang keterbacaan target 480–720 px menurut aturan Opsi B+. Karena pengecilan wajar ini untuk tata letak dan kualitasnya sudah diuji lokal, nama `shot-XX.jpg` benar; **bukan** file preview berkualitas rendah. Kanvas 1676×2116, label waktu berada di luar gambar, dan file berhasil didekode secara lokal.

**Contact Sheet Manifest — empat JPG terverifikasi di GitHub (satu per shot, total 22 panel):**

| Shot | Contact sheet | Timestamp panel kronologis | Panel | Dimensi kanvas / panel | Byte | SHA Git blob |
|---|---|---|---:|---|---:|---|
| 01 | [`shot-01.jpg`](../frames/muyon-01/shot-01.jpg) | 00:00.20; 00:01.10; 00:02.10; 00:03.10; 00:04.10; 00:05.20 | 6 | 1676×2116 / 540×960 | 1.265.088 | `8a04eab91ce1f4e6120e47d005b4832c27a7cbac` |
| 02 | [`shot-02.jpg`](../frames/muyon-01/shot-02.jpg) | 00:06.20; 00:07.20; 00:08.30; 00:09.30; 00:10.30; 00:11.40 | 6 | 1676×2116 / 540×960 | 1.163.762 | `a69eb2afedeb1ade3fb50d919a787b1dcc4f3aeb` |
| 03 | [`shot-03.jpg`](../frames/muyon-01/shot-03.jpg) | 00:12.20; 00:13.30; 00:14.40; 00:15.40; 00:16.20 | 5 | 1676×2116 / 540×960 | 953.713 | `4b504aa895ddc5f2dbd6bb3b908aafad394bad22` |
| 04 | [`shot-04.jpg`](../frames/muyon-01/shot-04.jpg) | 00:17.30; 00:18.40; 00:19.50; 00:20.60; 00:21.70 | 5 | 1676×2116 / 540×960 | 1.112.812 | `14d20db8968421b3869fe726f04bd982062b9aa7` |

**Verifikasi:** SHA Git blob dan byte dari keempat file pada tree GitHub cocok **persis** dengan JPEG lokal yang berhasil didekode. Karena cocok secara kriptografis, konten biner GitHub identik dengan file yang dapat dibuka lokal. Namun **pratinjau langsung lewat UI GitHub belum bisa diperiksa** oleh konektor; jangan mengklaim telah menguji tampilan web.

Tiga preview kecil lama telah digantikan empat contact sheet baru pada tree branch; semua tautan analisis mengarah ke JPG baru. File lama mungkin tetap tersedia dalam riwayat Git. Pengguna masih dapat meninjau dan mengoreksi identifikasi spesies yang belum pasti tanpa mengubah status `draft` secara otomatis.

## 10. Quality Checklist

**Gate A — Visual Accuracy: PASS (cakupan visual)**
- [x] Video asli di chat dapat diproses; metadata, seluruh timeline, Shot Map, dan transisi diperiksa dua tahap.
- [x] Empat shot utama serta penutup hitam dicatat; batas dissolve ditandai perkiraan.
- [x] Setiap shot mempunyai contact sheet 5–6 panel informatif (total 22) sesuai urutan waktu.
- [x] Gerak kamera, perubahan awal–tengah–akhir, tanaman, orang/hewan, kondisi air/cuaca, dan ketidakpastian dilacak ke shot/MP4.
- [x] Audio tidak diklaim telah didengarkan; interpretasi yang ambigu diberi label.

**Gate B — Repository Integrity: PASS**
- [x] Empat JPG valid, berhasil dibuka lokal, masing-masing 1676×2116; teks timestamp dan panel terbaca.
- [x] Keempat SHA Git blob serta ukuran byte pada GitHub **identik** dengan JPEG lokal yang diuji.
- [x] Manifest dan Shot Map menautkan empat JPG yang ada; tiga preview lama yang digantikan telah dikeluarkan dari tree.
- [x] Dokumen tetap 10 bagian, katalog INDEX konsisten dengan status `draft`, tanpa MP4 dalam tree branch.
- [x] Commit dan branch HEAD diverifikasi setelah penyimpanan.

**Overall Gate: PASS (untuk analisis visual dan integritas GitHub).** Status referensi **tetap `draft`**, bukan `approved`.

**Batas pemeriksaan:** Audio belum diaudit, identifikasi tertentu masih `[BELUM PASTI]`, batas transisi perkiraan; pratinjau gambar **langsung melalui UI GitHub** belum diuji, tetapi byte GitHub cocok dengan file JPEG yang terbukti valid secara lokal. Hak distribusi belum diverifikasi.

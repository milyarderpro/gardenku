# Video Analysis — Muyon / muyon-15

> **Gardenku Opsi B+ v1.3 — FASE 2 (Tahap 6–7), Document-First Save.**  
> Berdasarkan analisis Fase 1 dari MP4 asli, pengguna memberi izin eksplisit `save now` pada 2026-10-29. Hanya dokumen analisis dan INDEX disimpan di `main`; MP4 tidak masuk repository, dan JPG dikelola pengguna. Temuan `[OBSERVASI]` berasal dari MP4/frame; dugaan diberi penanda.

## 1. Reference Information

| Field | Isi |
|---|---|
| Video ID | `muyon-15` (terdaftar di INDEX; status setelah penyimpanan: `draft`) |
| Creator / Source | `muyon` = label koleksi di repository; identitas kreator asli **belum diverifikasi** |
| Input MP4 (chat) | `muyon-15.mp4`, `/mnt/data/muyon-15.mp4` (salinan kerja lokal) |
| Video storage | MP4 asli milik pengguna; **tidak disimpan ke GitHub** |
| Evidence input | MP4 lokal berhasil didekode, 618/618 frame trek video; pass pertama sampling timeline, pass kedua frame awal–tengah–akhir dan pergerakan lintas frame per shot |
| File metadata | 10.665.557 byte; SHA-256: `75b9382ee37f163e3d806ea7a5eef5e18fe41a91eaea7aa479f5b23017e54adb` |
| Contact sheet path | `references/muyon/frames/muyon-15/` (lokasi arsip JPG yang dikelola pengguna; tidak diunggah AI) |
| Source URL | Belum diketahui |
| Rights / Permission | Belum diketahui; distribusi JPG ke repo publik perlu izin yang sesuai |
| Analysis date | 2026-10-29 (Asia/Jakarta) |
| Workflow phase | `Fase 2 — save & verify (Tahap 6–7)` |
| Save authorization | `save now` — 2026-10-29 (Asia/Jakarta); pengguna menyatakan semua JPG telah diunggah |
| Repository save | `main`: `references/muyon/analysis/muyon-15.md` dan `references/INDEX.md` saja; commit SHA/HEAD dilaporkan dalam hasil verifikasi |
| Analysis status | `draft` — analisis telah disimpan untuk review, belum `approved` |
| Gate A / Gate B / Overall | `PASS` / `PASS` / `PASS` — menurut verifikasi Fase 2; bukti repository dan HEAD dicantumkan pada balasan |
| Evidence checked | MP4 asli secara berurutan melalui decoding 618 frame, sampling ±0,5–1 detik dan visual frame terpilih; dua batas cut dipastikan memakai selisih frame berurutan |
| Duration | Trek video **20,600 detik**; audio **20,688 detik**; kontainer **20,688 detik** |
| Resolution / FPS | **720 × 1280**, H.264, **30 FPS**, **618 frame** |
| Aspect ratio | **9:16** vertikal |
| Shot count | **3 shot kontinu**, dua hard cut ±00:07.07 dan ±00:13.07 |
| Audio review | Audio **AAC HE-AAC stereo 44,1 kHz terdeteksi**; **belum didengarkan**, tidak ada klaim tentang isinya |

## 2. Overall Description

[OBSERVASI] Video menunjukkan tiga rangkaian kebun yang rimbun dan intensif: lorong bedengan sayur di bawah para-para dengan banyak buah, tepi kolam berbingkai batu yang dilalui bebek, lalu area kebun dengan pohon berbuah besar di batang, ayam, dan seseorang memakai topi kerucut. Pergerakan pandangan secara umum bergeser ke kanan, menyingkap elemen baru dari bagian kiri menuju kanan pada setiap shot. Warna hijau daun kuat, diselingi merah tomat/buah kecil, jingga-kuning pepaya dan buah lain, serta cokelat tanah. Cahaya merata dengan langit putih keabu-abuan; **tidak cukup bukti** untuk menyebut jam tertentu atau hujan aktif.

- **Garden type:** kebun campuran sayur–buah intensif dengan bedengan dan area ternak kecil; kemungkinan halaman/pekarangan luas relatif terhadap frame; keberadaan rumah pada shot 02 membuat sebutan `open-field` murni kurang tepat.
- **Garden size / space:** sedang–luas secara relatif terhadap beberapa jalur, pohon, dan kolam; ukuran fisik tidak diketahui.
- **Visual hook awal:** perspektif lorong tanah di bawah trellis dengan buah merah dan hijau menggantung, gugusan buah cokelat besar di atas kanan, serta sosok bertopi kerucut di ujung jalur (00:00–00:02).
- **Visual density:** tinggi; hampir seluruh foreground dan midground dipenuhi bedengan, tanaman memanjat, pohon buah, atau hewan.
- **Overall camera style:** pergeseran pandangan dominan ke kanan, cukup halus dengan sedikit perubahan posisi/framing; pan vs lateral tracking tidak dapat dipisahkan secara pasti dari video saja.
- **Distinctive character:** (1) banyak jenis tanaman buah dan sayur dalam satu ruang, (2) interaksi manusia–ayam/bebek di tengah kebun, (3) kolam berbatas batu dan kanal air.

## 3. Shot Breakdown

### Shot Map — Pass 1, dikonfirmasi Pass 2

| Shot | Mulai–akhir pada trek gambar | Durasi | Transisi | Ketepatan / bukti | Cakupan |
|---|---|---:|---|---|---|
| 01 | 00:00.00–00:07.07 | ±7,07 dtk | awal file → hard cut | Batas frame 212 pada 30 FPS; perubahan gambar besar pada 7,067 s | awal, tengah, akhir diperiksa |
| 02 | 00:07.07–00:13.07 | 6,00 dtk | hard cut → hard cut | Frame 212–391; cut frame 392 pada 13,067 s | awal, tengah, akhir diperiksa |
| 03 | 00:13.07–00:20.60 | ±7,53 dtk | hard cut → akhir gambar | Frame 392–617; frame terakhir sebelum 20,600 s | awal, tengah, akhir diperiksa |

**Catatan waktu:** batas dilaporkan sampai dua desimal (pembulatan dari indeks frame), bukan transisi dissolving. Durasi kontainer 20,688 dtk lebih panjang dari trek video 20,600 dtk karena audio.

### Shot 01 — Lorong trellis, gugus buah dan pepaya (00:00.00–00:07.07)

- **Hero subject:** lorong kebun di bawah trellis/para-para, berganti menjadi gugusan buah kecil cokelat dan buah pepaya berwarna hijau–jingga di kanan.
- **Supporting subjects:** buah bulat merah menggantung (mirip tomat), buah panjang hijau menggantung (sebagian mirip pare/mentimun), daun sayuran pada bedengan, orang bertopi kerucut/pakaian cokelat di midground, beberapa ayam di atas tanah sisi kanan, batang/pagar kayu pendek dan jaring.
- **Visual hook:** hamparan trellis berbuah di atas lorong sekaligus gugusan buah kecil yang menggantung sangat rapat (00:00.17–00:02.70).
- **Camera movement:** [OBSERVASI] elemen trellis bergeser keluar kiri, gugus buah kanan bergerak melintasi frame, dan pohon pepaya semakin dominan; [INTERPRETASI, keyakinan sedang] **slow pan right** dengan kemungkinan perpindahan lateral atau maju sedikit. Bukan bukti zoom murni.
- **Speed / stability:** lambat–sedang; relatif stabil, dengan perubahan cepat di sekitar 00:02.8–00:03.7 yang diperiksa sebagai pergerakan tampilan, **bukan cut baru**.
- **Framing / angle:** vertical wide ke medium-wide; sudut pandang kira-kira setinggi mata, sedikit mengarah ke atas ketika tajuk/kanopi memenuhi bagian atas.
- **Composition:** foreground = jalan tanah di tengah dan bedengan daun hijau–ungu kiri; midground = trellis, jaring pendek, orang dan ayam; background = pepohonan buah dan langit terang. Gugus cokelat kanan atas menyeimbangkan deret buah merah kiri atas.
- **Garden layout:** jalur tanah sempit membelah bedengan berundak; tiang bambu/kayu dan para-para di kiri–atas; pohon buah di kanan jalur, batas kayu/jaring di sebelahnya.
- **Lighting / colors:** cahaya luar ruangan terbaur, hijau pekat, merah, jingga-kuning dan cokelat buah/tanah; tidak tampak bayangan tajam.
- **Weather / surfaces:** langit putih berawan; tanah terlihat cokelat dengan tekstur tidak seragam; **kelembapan tanah, gerimis, dan jam tidak terverifikasi**.
- **Action:** orang tampak mengangkat tangan ke arah dedaunan/percabangan (sekitar 00:01–00:06); ayam berkeliaran dan berpindah posisi di tanah kanan (00:04–00:07). Tidak dapat dipastikan orang sedang memanen.
- **Audio:** ada trek audio, **belum didengarkan**.
- **Transition:** hard cut di ±00:07.07 menuju kolam dan bedengan lain.

**Perkembangan:** **Awal (00:00.17):** lorong di bawah para-para dengan buah merah/hijau dan gugusan cokelat di kanan atas. **Tengah (00:03.90):** gugusan kecil cokelat memenuhi atas frame; pohon pepaya mulai jelas di kanan, orang dan ayam lebih terlihat. **Akhir (00:06.90):** pepaya jingga–hijau menjadi foreground kanan; ayam pada tanah kanan, orang tertahan di sisi kiri.

**Bukti & keyakinan:** [OBSERVASI] pepaya hijau–jingga pada 00:05.30–00:06.90 (tinggi); ayam 00:03.90–00:06.90 (tinggi). [INTERPRETASI] buah kecil cokelat mirip kelengkeng pada 00:02.70–00:05.30 (sedang); jenis buah memanjang yang menggantung pada trellis belum pasti (sedang/rendah). [BELUM PASTI] nama spesies gugusan buah, aktivitas memetik, dan pan dibanding tracking.

**Teknik yang bisa dipelajari:** susunan jalur sebagai leading line, transisi dari buah pada trellis menuju pohon pepaya, foreground berwarna hangat sebagai fokus visual.

### Shot 02 — Bedengan warna-warni dan tepi kolam berisi bebek (00:07.07–00:13.07)

- **Hero subject:** bedengan sayuran beraneka warna menuju kolam berbatas batu, dengan bebek yang bergerak di sepanjang tepian.
- **Supporting subjects:** sayuran daun hijau, ungu dan merah marun; trellis kiri dengan buah panjang hijau; pohon pepaya/pisang; sosok berpakaian biru dan bertopi kerucut di tepi seberang; rumah atap segitiga di background; tanaman air terapung dan lingkaran daun mirip teratai di kanan kolam.
- **Visual hook:** kontras warna bedengan padat dan kelompok bebek yang berjalan di sisi kolam (00:07.17–00:09.43).
- **Camera movement:** [OBSERVASI] bidang pandang menggeser fokus ke kanan, trellis dan bedengan kiri keluar, air kolam semakin banyak terlihat; [INTERPRETASI, keyakinan sedang–tinggi] pan right, mungkin dengan pergeseran posisi kamera kecil. Gerak gambar tidak mendukung zoom dominan.
- **Speed / stability:** pan lambat dan relatif mulus; percepatan ringan mendekati 00:11–00:12 ketika area air mendominasi.
- **Framing / angle:** medium-wide vertikal, sudut sedikit ke bawah untuk memperlihatkan bedengan, lintasan bebek dan air; rumah dan pepohonan menjadi latar atas.
- **Composition:** foreground = sayur daun merah/ungu/hijau dan jalan tanah, kemudian bebek dekat tepi; middle = kolam berbatu, sayur di tepi dan orang biru; background = pepohonan dan rumah.
- **Garden layout:** jalan tanah melengkung mengitari bibir kolam; bibir disusun dari batu-batu berukuran sedang; barisan sayur mengikuti kontur; air kolam beriak, terdapat tanaman air terapung dan daun bulat pada permukaan.
- **Lighting / colors:** cahaya lembut, tajuk hijau dan rumah pucat; pantulan air abu-abu kehijauan, tanpa bayangan langsung yang kuat.
- **Weather / surfaces:** background agak berkabut/pucat (bisa karena atmosfer maupun kualitas gambar); tidak ada bukti pasti gerimis aktif. Riak permukaan kolam tampak pada 00:11.8–00:12.9 tetapi **penyebab spesifik riak belum pasti**.
- **Action:** beberapa bebek cokelat dan putih bergerak menyusuri tepi kolam dari midground menuju foreground bawah (00:08–00:12.93); orang berbusana biru dengan wadah cerah terlihat di seberang (00:07.17–00:11.0), aktivitas tepat tidak pasti.
- **Audio:** trek terdeteksi, belum didengarkan.
- **Transition:** hard cut pada ±00:13.07 ke kebun pohon nangka.

**Perkembangan:** **Awal (00:07.17):** bedengan aneka sayur dan trellis menggantung di kiri, kolam mulai muncul di kanan dan bebek pada jalur. **Tengah (00:10.73):** tepi kolam dan bebek lebih sentral; orang berbusana biru di seberang, rumah di belakang. **Akhir (00:12.93):** permukaan air mendominasi kanan, sepasang bebek putih–cokelat di tepi bawah, tanaman air terlihat di kanan.

**Bukti & keyakinan:** [OBSERVASI] bebek di tepi kolam (tinggi; 00:08.17–00:12.93), batas batu dan riak air (tinggi; 00:10.73–00:12.93), orang biru bertopi kerucut (tinggi; 00:07.17–00:11). [BELUM PASTI] bentuk jingga/pucat di bawah air dekat 00:12.93 mungkin ikan, tetapi tidak cukup jelas untuk klaim jenis/jumlah; fungsi wadah yang dibawa orang dan sumber riak.

**Teknik yang bisa dipelajari:** pan dari bedengan ke air yang membuka lanskap sedikit demi sedikit; kurva jalur/batu mengarahkan mata; kehadiran bebek menambahkan gerakan lapisan depan.

### Shot 03 — Pohon nangka, ayam dan aktivitas di pangkal pohon (00:13.07–00:20.60)

- **Hero subject:** pohon berbuah nangka kuning-hijau yang tumbuh sepanjang batang, serta seseorang berpakaian biru dan bertopi kerucut di dekat pangkalnya.
- **Supporting subjects:** banyak ayam dengan bulu jingga-cokelat, hitam, dan campuran; pohon di belakang dengan buah kuning lonjong menggantung (mirip mangga); pepaya hijau pada kanan; tanaman merambat di penyangga bambu; buah ungu gelap menggantung pada tanaman di pot/bedengan (mirip terong); kumpulan buah kecil jingga-merah dekat kiri bawah; air di parit/kanal sempit pada sisi kiri.
- **Visual hook:** beberapa nangka besar menempel pada batang di bagian tengah/kiri, aktivitas manusia dan ayam di bawahnya (00:13.17–00:15.77).
- **Camera movement:** [OBSERVASI] pohon nangka bergeser dari sekitar tengah ke kiri, ayam dan manusia lebih besar/jelas; kamera tetap bergerak relatif halus. [INTERPRETASI, keyakinan sedang] pergeseran/pan ke kanan dengan sedikit pendekatan ke subjek, bukan bukti zoom optik.
- **Speed / stability:** pelan, stabil dengan penyesuaian framing; perubahan sudut kecil saat mendekati area aktivitas.
- **Framing / angle:** medium-wide vertikal menjadi framing lebih dekat pada orang dan pohon; perspektif agak menunduk untuk menampilkan jalan berbatu, bedengan dan ayam.
- **Composition:** foreground = kerikil jalan, sayuran, buah jingga-merah, daun kecil dan pipa irigasi hitam; middle = pohon nangka, orang, ayam; background = pohon buah lain, batang/tiang kayu dan vegetasi rapat.
- **Garden layout:** jalan kerikil di tengah; bedengan dan pot/batas hitam di sisi kanan-kiri; kanal kecil berbingkai beton di kiri; struktur ajir/para-para untuk tanaman rambat; pipa air hitam melintang dekat batas tanah dan bedengan.
- **Lighting / colors:** pencahayaan lembut, kuning pada nangka dan gugusan buah, hijau daun sangat padat; warna tanah cokelat/jerami.
- **Weather / surfaces:** kanal berair terlihat; tak ada bukti hujan/gerimis pada shot ini. Perlu dibedakan air kanal dari genangan hujan.
- **Action:** orang membungkuk dan menggerakkan tangan di dekat pangkal pohon dan ayam (00:13.17–00:18.83); pada 00:18.83–00:20.43 tampak memegang wadah, ayam bergerak/berkumpul di tanah. [INTERPRETASI] mungkin memberi pakan atau merawat area tersebut, tetapi butiran pakan maupun tujuan pasti tidak terverifikasi.
- **Audio:** belum didengarkan.
- **Transition:** tidak ada; berakhir pada frame terakhir trek video ±00:20.60.

**Perkembangan:** **Awal (00:13.17):** pohon nangka dominan tengah, orang biru membungkuk, kanal air dan tanaman rambat kiri. **Tengah (00:17.13):** batang dan gugusan nangka mulai ke kiri, orang lebih menonjol, ayam bergerak di belakang/kaki. **Akhir (00:20.43):** orang dan ayam lebih dekat dan dominan pada bagian bawah kanan; pohon nangka berada lebih kiri, banyak pepaya hijau menggantung pada kanan frame.

**Bukti & keyakinan:** [OBSERVASI] nangka pada batang (tinggi; 00:13.17–00:20.43), ayam (tinggi; 00:14.47–00:20.43), kanal kiri (tinggi; 00:13.17–00:15.77), wadah pada orang (sedang–tinggi; 00:18.83–00:20.43). [INTERPRETASI] memberi pakan (sedang/rendah); tanaman berbuah lonjong kuning mirip mangga (sedang), buah ungu mirip terong (sedang). [BELUM PASTI] identitas spesies beberapa buah dan apakah orang pada ketiga shot sama.

**Teknik yang bisa dipelajari:** menggabungkan pemandangan agrikultur dan subjek manusia/ayam; lapisan buah pada batang menciptakan titik fokus vertikal; pemakaian jalur kerikil sebagai garis penuntun.

## 4. Plants, Fruits & Garden Layout

| Elemen | Di mana? | Susunan / ciri visual | Keyakinan |
|---|---|---|---|
| Tomat atau buah bulat merah serupa | Shot 01, 00:00–00:02.7 | Deret merah kecil menggantung pada para-para kiri atas | Sedang–tinggi (identifikasi jenis bisa dibatasi dari frame) |
| Buah panjang hijau / kemungkinan pare atau mentimun | Shot 01 dan 02, 00:00–00:02 serta 00:07–00:09 | Buah memanjang menggantung dari rangka bambu; beberapa bergerigi | Sedang untuk kelompok; spesies belum pasti |
| Gugusan buah kecil cokelat / mirip kelengkeng | Shot 01, 00:00–00:05.3 | Tandan padat menggantung pada tajuk di kanan atas | Sedang |
| Pepaya hijau–kuning/jingga | Shot 01, 00:04–00:07; pepaya hijau shot 03 00:17–00:20.4 | Buah mengelompok di dekat ujung batang tegak | Tinggi |
| Sayuran daun hijau, ungu, merah marun | Shot 01 & 02 | Bedengan rapat di sepanjang jalur tanah dan tepi kolam | Tinggi pada bentuk; spesies sebagian belum pasti |
| Buah besar pada batang (nangka) | Shot 03, 00:13–00:20.4 | Buah berduri tumpul berwarna kuning-hijau menempel sepanjang batang | Tinggi |
| Buah lonjong kuning menggantung pada pohon | Shot 03, 00:13–00:20.4 | Menggantung bergerombol di pohon belakang; mirip mangga | Sedang |
| Buah ungu gelap / kemungkinan terong | Shot 03, 00:13–00:15.8 | Gantung dekat bedengan/pot rendah pada kanan foreground | Sedang |
| Buah kecil jingga-merah / kemungkinan jenis cabai | Shot 03, 00:13–00:15 | Berkelompok pada tanaman rendah sisi kiri | Sedang |
| Bedengan / kerikil / tiang penyangga | Ketiga shot | Bedengan di sisi jalur; bambu/kayu para-para, ajir penyangga | Tinggi |
| Kolam berbatas batu dan tanaman air | Shot 02, 00:07–00:13 | Kolam melengkung dan tepi sayur hijau; permukaan beriak | Tinggi |
| Kanal beton berair dan pipa hitam | Shot 03, 00:13–00:20 | Kanal sempit di sisi kiri, pipa melintang dekat permukaan tanah | Tinggi |

**Struktur lapisan:** sayur daun rendah di depan → tanaman rambat dan trellis di sisi/atas → pepaya dan pohon buah di tengah–belakang. **Ciri penataan:** tanaman sayur dan buah dibuat sangat berdekatan, dipisahkan jalan kecil untuk akses; area air/ternak terintegrasi dengan bedengan.

## 5. Weather, Atmosphere & Lighting

- **Waktu:** **belum pasti**. Langit cukup terang tetapi tidak menunjukkan jam tertentu.
- **Cuaca:** langit putih keabu-abuan pada shot 01, kesan latar agak berkabut pada shot 02; **tidak cukup bukti untuk menyebut hujan aktif, gerimis, atau kondisi pascahujan**.
- **Light quality:** [OBSERVASI] pencahayaan lembut/tersebar, bayangan objek relatif lemah; [INTERPRETASI] dapat berupa mendung tipis atau kondisi cahaya difus lainnya.
- **Wet surfaces:** [OBSERVASI] permukaan kolam dan air kanal terlihat; tanah tidak dapat dipastikan basah hanya karena berwarna cokelat.
- **Water source:** kolam air shot 02; kanal air shot 03. **Tidak tampak sumber hujan/sprinkler yang bisa diidentifikasi**.
- **Atmosphere / mood:** [INTERPRETASI] subur, damai, penuh aktivitas kebun dan unggas; warna hijau menyegarkan.
- **Relevant motion:** bebek dan ayam bergerak; riak air kolam terlihat pada shot 02; daun/gugus buah berubah letak terutama karena gerakan kamera.
- **Evidence notes:** 00:00.17 langit pucat; 00:11.8–00:12.9 riak kolam; 00:13.17–00:15.77 air kanal.

## 6. Animals, Humans & Other Objects

| Subjek | Jumlah tampak | Shot dan posisi | Aktivitas / interaksi | Peran |
|---|---|---|---|---|
| Manusia bertopi kerucut dengan pakaian cokelat | Setidaknya 1 tampak | Shot 01, midground ujung jalur | Mengangkat tangan ke arah cabang/daun; detail aktivitas tidak pasti | Pendukung |
| Ayam warna cokelat/jingga dan gelap | Beberapa ekor; jumlah tepat tidak dapat dipastikan dari gerak/overlap | Shot 01 sisi kanan, shot 03 sekitar orang/pohon | Berjalan/berkerumun di tanah; ada yang mendekati orang | Pendukung penting |
| Bebek cokelat, krem dan putih | Beberapa ekor (setidaknya 3 terlihat dalam shot) | Shot 02 jalur dan tepi kolam | Bergerak menyusuri tepian berbatu; sejumlah bebek dekat air | Hero aktivitas shot 02 |
| Manusia baju biru dan bertopi kerucut | Setidaknya 1 per shot; **tidak diasumsikan identik antarsot** | Shot 02 di seberang kolam; shot 03 di bawah nangka | Terlihat membawa/memegang wadah; shot 03 membungkuk dan menggerakkan tangan ke tanah | Pendukung shot 02, hero bersama nangka shot 03 |
| Rumah, ajir, jaring, batu, pipa dan kanal | Beragam, jumlah tak dihitung | Ketiga shot | Elemen lingkungan, tidak bergerak sendiri | Latar/struktur |
| Ikan | **Belum terkonfirmasi** | Shot 02, dekat 00:12.93 ada bentuk samar di bawah permukaan | Gerak/jenis/jumlah tidak cukup jelas | Belum dicatat sebagai objek terverifikasi |

**Realism notes:** unggas terlihat berdiri/bergerak di atas tanah dan dekat kolam; kontak fisik dan detail benda kecil perlu kehati-hatian. Identitas atau profesi manusia **tidak diketahui**. Tidak menyimpulkan pemberian pakan sebagai fakta jika butiran pakan tidak teramati.

## 7. Audio, Editing & Pacing

- **Audio checked:** **tidak**; hanya metadata AAC HE-AAC stereo 44.100 Hz terdeteksi.
- **Natural sound:** belum diperiksa.
- **Voice / music:** belum diperiksa.
- **Shot rhythm:** tiga shot relatif panjang **7,07 → 6,00 → 7,53 detik**; tempo tenang dengan gerakan kamera internal berkesinambungan.
- **Transitions:** **dua hard cut**, sekitar 00:07.07 (trellis/pepaya → kolam), 00:13.07 (kolam → nangka/ayam); tidak terlihat fade/dissolve di batas ini.
- **Editing effectiveness:** [INTERPRETASI] variasi fokus objek dari **buah di atas → bebek dan air → manusia–ayam di bawah pohon** memberi pergantian perhatian tanpa edit yang terlalu cepat.

## 8. Visual Characteristics & Reusable Inspiration

**Karakter visual terpenting:**
1. Sayur rendah dan buah menggantung bertumpuk dalam frame vertikal (shot 01, 00:00–00:07).
2. Pergeseran pandangan ke kanan membuka subjek baru secara bertahap (ketiga shot).
3. Kontras hijau rimbun dengan kuning-jingga buah dan ungu-merah sayur (shot 01 dan 03).
4. Jalan sempit, batu tepi kolam, dan kanal air sebagai leading lines (shot 01–03).
5. Aktivitas ayam dan bebek di sekitar manusia sebagai lapisan kehidupan kebun (shot 02–03).

**Teknik reusable:** mulai dengan foreground buah menggantung lalu bergerak menyingkap objek berikut; ikuti garis jalur melengkung untuk reveal kolam; masukkan aktivitas orang–unggas sebagai subjek skala/gerakan pada midground. Ini **catatan teknik**, bukan pembuatan konsep atau prompt.

**Elemen opsional:** nangka, pepaya, ayam, bebek, kolam, orang bertopi kerucut, kanal, rumah.

**Hal yang sebaiknya tidak ditiru secara membabi buta:** kepadatan buah/objek yang sangat tinggi dapat mengaburkan skala atau detail kecil; identifikasi tanaman ambigu dan aktivitas manusia jangan dijadikan klaim spesifik.

**Search tags berbasis bukti:** `mixed-vegetable-fruit-garden`, `bamboo-trellis`, `garden-path`, `papaya`, `jackfruit`, `chickens`, `ducks`, `stone-edged-pond`, `canal`, `soft-diffuse-light`, `rightward-camera-reveal`. **Tidak diberi tag** `rain`, `after-rain`, atau `fish` karena belum terverifikasi.

## 9. Notes & Uncertainty

- **Belum bisa diverifikasi:** identitas kreator di luar label koleksi `muyon`, URL asli, hak distribusi, jam pengambilan, lokasi fisik/ukuran lahan, audio, identitas orang, dan identifikasi spesies beberapa gugus buah.
- **Asumsi perlu diuji ulang:** kombinasi `pan right` dibanding lateral tracking; aktivitas orang berupa memberi pakan/memanen; bentuk samar di bawah permukaan kolam apakah ikan; gugus buah cokelat mirip kelengkeng dan buah lonjong kuning mirip mangga.
- **Sumber informasi pengguna:** file `muyon-15.mp4`, instruksi Fase 1, dan `save now` pada 2026-10-29; pengguna menyatakan JPG sudah diunggah. Tidak ada keterangan cuaca/lokasi tambahan.

### Contact Sheet Manifest

**Lokal:** masing-masing JPG selesai dibuat dari frame asli, label waktu berada di luar gambar, aspek 9:16 terjaga, sumber 720×1280 → panel 540×960, tanpa upscale. Layout 3 kolom × 2 baris; kanvas 1676×2116. Path GitHub di bawah hanya **lokasi arsip yang akan dikelola pengguna**, bukan klaim upload.

| Shot | Nama/path JPG standar (tujuan arsip) | Timestamp panel | Panel | Kanvas / panel / sumber | Kategori | Byte lokal |
|---|---|---|---:|---|---|---:|
| 01 | `references/muyon/frames/muyon-15/shot-01.jpg` | `00:00.17; 00:01.50; 00:02.70; 00:03.90; 00:05.30; 00:06.90` | 6 | 1676×2116 / 540×960 / 720×1280 | `contact-sheet` | 1.931.441 |
| 02 | `references/muyon/frames/muyon-15/shot-02.jpg` | `00:07.17; 00:08.17; 00:09.43; 00:10.73; 00:12.03; 00:12.93` | 6 | 1676×2116 / 540×960 / 720×1280 | `contact-sheet` | 1.682.777 |
| 03 | `references/muyon/frames/muyon-15/shot-03.jpg` | `00:13.17; 00:14.47; 00:15.77; 00:17.13; 00:18.83; 00:20.43` | 6 | 1676×2116 / 540×960 / 720×1280 | `contact-sheet` | 2.072.331 |

### Evidence Cross-Check — Tahap 5 (sudah dilakukan)

- **Cakupan shot:** dari frame pertama 00:00.00 hingga frame terakhir sebelum 00:20.60; semua 3 shot terwakili, 6 panel/shot; 2 cut teridentifikasi dari lonjakan selisih piksel pada 7,067 dan 13,067 s. Tidak ada indikasi hard cut lain dengan perbedaan sebesar batas tersebut.
- **Awal–tengah–akhir:** setiap shot memuat panel sebelum, saat perkembangan, dan mendekati akhir; isi panel konsisten dengan ringkasan gerakan.
- **Gerakan kamera:** arah perubahan pandangan dikonfirmasi melalui urutan frame dan estimasi optical flow (komponen perpindahan horizontal dominan ke kiri pada objek, selaras dengan reveal kanan); pan dibanding tracking tetap ditandai **interpretasi** karena memerlukan pembuktian posisi kamera.
- **Titik ambigu:** lonjakan perubahan visual saat 00:02.8–00:03.7 dalam shot 01 tidak sama dengan hard cut; buah pada trellis, ikan kolam, aktivitas orang, dan cuaca tidak diberi kepastian berlebih.
- **Kualitas JPG:** ketiga JPG disimpan dan dibuka, 1676×2116 dengan panel yang terbaca 540×960 dan label di luar area gambar; **kategori standar contact-sheet**. Tidak ada klaim file JPG di GitHub.
- **Audio:** track AAC ada tetapi **belum diperiksa secara auditori**. Tidak ada klaim suara alam, musik, dialog, atau hewan.

## 10. Quality Checklist

| Gate | Status Fase 2 | Bukti |
|---|---|---|
| Gate A — Visual Accuracy | **PASS** | MP4 asli 720×1280 30 FPS, 618 frame, trek gambar 20,600 detik; dua-pass inspection; 3 shot, 2 hard cut; 3 contact sheet JPG asli (masing-masing 6 panel), timestamp, objek, gerak kamera, cuaca dan ketidakpastian sudah dicocokkan |
| Gate B — Document & Repository Integrity | **PASS** | Analisis 10 bagian dan satu baris `muyon-15` pada INDEX disimpan bersama dalam satu commit `main`; dokumen, INDEX, tautan yang digunakan dan HEAD dicek ulang; commit SHA dilaporkan dalam balasan |
| Overall Gate | **PASS** | Gate A dan Gate B memenuhi persyaratan; keberadaan JPG di GitHub bukan bagian dari Gate B |

**Bukti Gate A:** MP4 `muyon-15.mp4` (10.665.557 byte; SHA-256 `75b9382ee37f163e3d806ea7a5eef5e18fe41a91eaea7aa479f5b23017e54adb`), 618 frame video, cut ±00:07.07 dan ±00:13.07; `shot-01.jpg`, `shot-02.jpg`, `shot-03.jpg` masing-masing berkanvas 1676×2116 dengan enam panel 540×960 (sumber 720×1280). Track audio terdeteksi tetapi **belum didengarkan**.

**Bukti Gate B:** `references/muyon/analysis/muyon-15.md` dan `references/INDEX.md`; commit SHA dan HEAD `main` dikonfirmasi sesudah commit serta dilaporkan dalam chat. Nama JPG pada manifest hanya penunjuk lokasi arsip pengguna, bukan hyperlink atau klaim upload oleh AI.

**Status:** `draft`; `save now` tidak bermakna persetujuan `approved`.

**Ketidakpastian tetap:** sumber asli/izin tidak diketahui; audio belum diaudit; spesies buah tertentu, gerak fisik pan/tracking, aktivitas orang, hujan, dan ikan belum pasti.

- [x] MP4 asli diperiksa dengan Shot Map Pass 1 dan Deep Shot Analysis Pass 2.
- [x] Tiga shot dibuktikan melalui perkembangan awal–tengah–akhir dan batas cut.
- [x] Tiga contact sheet JPG per shot dicatat lengkap dalam Manifest.
- [x] Evidence Cross-Check dari Fase 1 terdokumentasi.
- [x] Dokumen Markdown dan INDEX disimpan serta diverifikasi langsung pada `main`.
- [x] Tidak mengunggah JPG/MP4, tidak membuat branch ataupun PR.

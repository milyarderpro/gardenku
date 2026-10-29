# Video Analysis — Muyon / muyon-14

> **Gardenku Opsi B+ v1.3 — FASE 2, Tahap 6–7 (Document-First Save).** Analisis Fase 1 terbaru disimpan berdasarkan izin eksplisit `save now` pada 2026-10-29. Hanya dokumen analisis dan INDEX yang diperbarui di `main`; JPG dikelola pengguna. MP4 asli tetap milik pengguna. Analisis dibuat berdasarkan MP4 terunggah, inspeksi seluruh 588 frame untuk deteksi perubahan visual, sampling timeline, pemeriksaan frame awal–tengah–akhir, dan verifikasi gerak antarframe. Audio tidak diaudit.

## 1. Reference Information

| Field | Isi |
|---|---|
| Video ID | `muyon-14` |
| Creator / Source | Koleksi `muyon`; identitas kreator dan asal sumber belum terverifikasi |
| Input MP4 (chat) | `muyon-14.mp4` |
| Video storage | Milik pengguna, tidak disimpan di repository |
| Evidence input | MP4 asli unggahan chat, seluruh timeline dan sampel gerak diperiksa |
| Input metadata | 10.308.161 byte; SHA-256 `8c2af5edfb7b68475a54828404443aa9684f32d78544f5d06fe3207ee8ae58e6` |
| Contact sheet path | `../frames/muyon-14/` (path arsip yang disiapkan, bukan file di GitHub) |
| Source URL | Belum diketahui |
| Rights / Permission | Belum diketahui |
| Analysis date | 2026-10-29 |
| Workflow phase | `Fase 2 — save & verify` |
| Save authorization | `save now` — 2026-10-29; pengguna menyatakan ketiga JPG telah diunggah |
| Repository save | `main`: `references/muyon/analysis/muyon-14.md` + `references/INDEX.md`; commit SHA dan HEAD diverifikasi setelah penyimpanan, dilaporkan pada percakapan |
| Analysis status | `draft` — hasil analisis AI, belum `approved` |
| Gate A / Gate B / Overall | `PASS` / `PASS` / `PASS` (setelah verifikasi commit dan HEAD; bukti tercantum dalam balasan) |
| Evidence checked | Video asli, sampled frames, frame-adjacent cut boundaries, motion comparison |
| Duration | Trek video 19,600 dtk; trek audio ~19,689 dtk; kontainer sekitar 19,69 dtk (angka terakhir tergantung pembacaan format) |
| Resolution / FPS | 720×1280, 30 fps, 588 frame; H.264 |
| Aspect ratio | 9:16 |
| Shot count | 3 (dua hard cut terdeteksi) |
| Audio review | Track AAC stereo ada; isi suara **belum diperiksa** |

## 2. Overall Description

[OBSERVASI] Video vertikal menunjukkan kebun yang tertata dalam konteks hunian, berisi bedengan sayur, pohon berbuah, tanaman merambat pada penyangga, jalur kerikil, serta area kolam. Pada bagian pertama terlihat ikan cerah, daun tanaman air mengapung, cabai, bedengan dan pohon berbuah oranye dengan rumah beratap genteng. Pada bagian kedua terlihat sayuran hijau dalam barisan, buah merah pada tanaman rendah, dan banyak buah hijau panjang tergantung di para-para; bagian terakhir membuka kolam luas dan tanaman pisang di dekat rumah lain. [INTERPRETASI] Desain visual menggabungkan kebun pangan padat dengan taman dekoratif, dengan pemindahan fokus dari detail dekat ke lanskap air.

- **Garden type:** `residential-garden`, `raised-beds`, `pond-garden`; tidak bisa dipastikan berada pada satu persil/kebun yang sama.
- **Garden size / space:** ruang tampak berlapis dan relatif luas untuk pekarangan; ukuran lahan tidak terukur.
- **Visual hook awal:** ikan oranye/putih di kolam, daun air dan bunga di depan, bedengan segar serta rumah di belakang (00:00.20).
- **Visual density:** tinggi; sebagian besar frame terisi sayuran, pohon buah, rambatan, dan tumbuhan tepi kolam.
- **Overall camera style:** penyapuan horizontal/gerak lateral pada shot 1 dan 3; gerak mendekat pada shot 2 (klasifikasi mekanisme tepat tidak sepenuhnya pasti).
- **Distinctive character:** kombinasi kolam–bedengan, pohon buah oranye yang sangat lebat, buah panjang tergantung di rambatan.

## 3. Shot Breakdown

**Shot Map — Pass 1, diperiksa ulang terhadap batas frame Pass 2**

| Shot | Mulai–akhir video | Durasi | Transisi | Ketepatan dan bukti waktu | Cakupan |
|---|---|---:|---|---|---|
| 01 | 00:00.000–00:06.633 | 6,633 dtk | Video mulai → hard cut ke 02 | Batas pada frame 198/199; ±1 frame dari pengodean | Semua rentang ditinjau |
| 02 | 00:06.633–00:13.067 | 6,433 dtk | Hard cut → hard cut ke 03 | Frame 391/392; ±1 frame | Semua rentang ditinjau |
| 03 | 00:13.067–00:19.600 | 6,533 dtk | Hard cut → akhir video | Frame 392–587 | Semua rentang ditinjau |

### Shot 01 — Kolam ikan, bedengan, dan pohon buah jingga

- **Timestamp / duration:** 00:00.000–00:06.633 / 6,633 dtk.
- **Hero subject:** [OBSERVASI] kolam dan tanaman air di awal; kemudian pohon berbuah kecil jingga dalam jumlah banyak (00:04–00:06.43).
- **Supporting subjects:** ikan cerah, bunga air putih/pink, bedengan selada/sayuran daun, tanaman berbuah merah dan cabai, pohon dengan tandan buah lonjong hijau-kuning mirip pepaya, bunga ungu menggantung, rumah beratap genteng, jalur batu/kerikil.
- **Visual hook:** air kolam dengan ikan dan daun mengapung di 00:00.20; bergeser menuju pohon buah jingga yang penuh warna.
- **Camera movement:** [OBSERVASI] susunan latar bergeser ke kiri layar dan objek di kanan semakin dominan. [INTERPRETASI] pan/rightward lateral reveal dengan sedikit pendekatan/parallax; tingkat keyakinan **sedang**, pemisahan pan versus tracking fisik belum pasti. Bukan bukti zoom murni.
- **Speed and stability:** lambat–sedang, pergeseran relatif halus.
- **Angle and framing:** medium-wide lanskap kebun dari ketinggian sekitar mata; sebagian arah pandang sedikit menurun ke kolam dan bedengan.
- **Composition:** foreground kolam, daun air, ikan dan batu; middle ground bedengan/kebun cabai/jalur; background pepohonan, buah dan rumah; kemudian pohon jingga menjadi foreground/middle-ground utama.
- **Garden layout:** kolam di depan kiri; batu pijakan pada tepi; bedengan kayu memanjang; jalur kerikil melengkung di antara tanaman; batu kecil mengelilingi pangkal pohon.
- **Lighting and colors:** siang terang alami secara visual, dominan hijau, kuning-jingga, merah dan bunga ungu; bayangan keras tidak dominan.
- **Weather and surfaces:** langit sebagian berawan; kondisi hujan atau bekas hujan **belum pasti**; kolam jelas berair, tidak membuktikan curah hujan.
- **Action/interaction:** ikan tampak berada/bergerak di dalam kolam (00:00.20–00:01.38); tidak tampak manusia.
- **Audio:** audio belum diperiksa.
- **Transition to next:** hard cut pada 00:06.633.

**Perkembangan awal → tengah → akhir:**
- **Awal 00:00.20:** kolam dengan ikan berwarna terang dan tanaman air di bawah bedengan; rumah serta tanaman tinggi sebagai latar.
- **Tengah 00:02.66–00:03.95:** sisi kolam keluar dari frame; jalur kerikil melengkung dan cabai merah/kuning serta kelompok buah jingga tampil lebih sentral.
- **Akhir 00:05.24–00:06.43:** pohon berbuah jingga memenuhi kanan dan tengah layar; bunga ungu menggantung terlihat di belakang/kanan; jalan kerikil masih tampak di kiri.

**Bukti dan ketidakpastian:** [OBSERVASI] warna, bentuk buah dan posisi di timestamp di atas; [INTERPRETASI] pohon jingga tampak seperti jeruk, pohon berbuah lonjong tampak seperti pepaya; penetapan spesies pasti [BELUM PASTI]. [KONTEKS PENGGUNA] hanya file MP4 yang disediakan; belum ada keterangan tambahan tentang cuaca/lokasi.

**Teknik yang dapat dipelajari:** pembukaan berlapis kolam → bedengan → pohon berbuah; jalur melengkung sebagai leading line; penyapuan perlahan memperkenalkan warna buah.

### Shot 02 — Bedengan sayur dan rambatan buah panjang

- **Timestamp / duration:** 00:06.633–00:13.067 / 6,433 dtk.
- **Hero subject:** baris bedengan pangan dengan rambatan horizontal dan buah hijau panjang yang menggantung, makin dominan mendekati akhir (00:10.42–00:12.87).
- **Supporting subjects:** buah merah dalam kelompok (tampak seperti tomat), cabai merah, sayuran hijau menyerupai selada/kubis, rumpun daun tegak menyerupai daun bawang, semak/pohon kecil, rumah bata dan atap di belakang, selang irigasi hitam.
- **Visual hook:** deretan sayuran segar, buah merah di sisi kanan serta struktur rambat berbuah pada awal 00:06.83.
- **Camera movement:** [OBSERVASI] objek depan/penyangga tumbuh lebih besar di frame, menjelang para-para; ada sedikit pergeseran horizontal. [INTERPRETASI] gerak mendekat (*push-in*) dominan dengan koreksi arah pandang, **keyakinan sedang–tinggi** terhadap pendekatan, tetapi apakah optik/digital zoom ikut digunakan [BELUM PASTI].
- **Speed and stability:** halus, lambat–sedang, tanpa getaran besar yang jelas pada sampel.
- **Angle and framing:** awal medium-wide ke bedengan; semakin dekat medium terhadap buah gantung dan sayuran; pandangan agak menurun ke tanah di awal, setinggi para-para menjelang akhir.
- **Composition:** foreground sayuran daun dan rumpun hijau panjang; middle ground tomat/cabai dan bedengan; background para-para buah hijau, pohon dan bangunan.
- **Garden layout:** bedengan tanah dipisah jalur sempit, beberapa tepi kayu; penyangga rambat horizontal yang tampak seperti bambu/kayu; selang hitam berada di atas tanah sepanjang baris.
- **Lighting and colors:** cahaya lembut terang, hijau tanaman dominan dan aksen merah tomat/cabai; langit bercampur awan.
- **Weather and surfaces:** tanah terlihat terbuka; kelembapan tanah dan adanya hujan tidak dapat dibuktikan; tidak tampak semprotan sprinkler.
- **Action/interaction:** tidak tampak aktivitas orang/hewan; gerakan utama berasal dari perubahan posisi kamera.
- **Audio:** belum diperiksa.
- **Transition to next:** hard cut pada 00:13.067.

**Perkembangan awal → tengah → akhir:**
- **Awal 00:06.83:** buah merah di kanan, rumah di kanan atas, baris bedengan dan rangka horizontal membentang pada bagian tengah atas.
- **Tengah 00:09.23–00:10.42:** kelompok buah merah mulai terpotong di tepi kanan; rumpun tegak dan sayuran mengisi tengah, buah-buah gantung makin terlihat jelas.
- **Akhir 00:11.78–00:12.87:** rangka dan deretan buah silindris memanjang menjadi fokus; sayuran hijau bertingkat tetap di bagian bawah.

**Bukti dan ketidakpastian:** [OBSERVASI] sejumlah buah hijau panjang menggantung vertikal, ukuran bervariasi; [INTERPRETASI] kemungkinan jenis labu, tetapi spesies belum terkonfirmasi. Gerak mendorong masuk disimpulkan dari pembesaran objek antarframe, bukan kepastian lintasan kamera fisik.

**Teknik yang dapat dipelajari:** *push-in/reveal* menuju hasil panen yang menggantung; framing bertingkat antara daun dekat, bedengan tengah dan bangunan jauh; kontras buah merah dengan daun hijau.

### Shot 03 — Perambat foreground membuka kolam luas

- **Timestamp / duration:** 00:13.067–00:19.600 / 6,533 dtk.
- **Hero subject:** kolam luas dengan beberapa kelompok tanaman air di atas permukaan, tanaman pisang dan pohon di tepi, serta bangunan pada latar.
- **Supporting subjects:** perambat di bagian atas berbuah hijau kecil memanjang dengan bunga kuning, tiang rambatan vertikal, cabai/tomat merah serta sayuran daun di bagian bawah dekat, kubis di sisi kanan, jalur tanah menuju kolam, rumah beratap merah muda/merah-bata di seberang air.
- **Visual hook:** bukaan antara rambatan dan sayuran menuju rumah di tepi air (00:13.27).
- **Camera movement:** [OBSERVASI] tiang/daun perambat dekat menyapu cepat melintasi frame sementara bangunan dan pohon jauh bergeser lebih lambat; pemandangan kanan kolam semakin terbuka. [INTERPRETASI] gerak lateral ke kanan dengan **parallax foreground yang kuat**, mungkin disertai pan kanan; keyakinan **tinggi** bahwa terdapat komponen pergeseran sudut/posisi, tetapi mekanisme fisik tepat tidak pasti.
- **Speed and stability:** sedang di awal, lebih tenang pada akhir, cukup halus.
- **Angle and framing:** medium-wide transisi menuju wide pada pemandangan kolam dari ketinggian sekitar mata, sedikit menurun ke permukaan air.
- **Composition:** awal foreground rambatan/daun menutup sisi kanan; middle ground sayuran dan tepi kolam; background rumah dan pepohonan. Akhir menonjolkan bidang air di tengah, tanaman air terapung di bawah, pohon pisang pada kanan-tengah.
- **Garden layout:** baris sayuran depan, tepi kolam yang ditanami rapat, badan air luas, tanaman air berkelompok, pohon dan hunian di seberang.
- **Lighting and colors:** cahaya siang tersebar dengan langit terlihat cerah pucat/berawan; banyak hijau, atap merah/pink, air keabu-abuan.
- **Weather and surfaces:** permukaan air memiliki tekstur/riak halus; [BELUM PASTI] apakah riak berasal dari angin, gerimis, atau sumber lain. Tidak cukup bukti untuk klaim hujan aktif.
- **Action/interaction:** perambat bergerak melintasi bidang pandang relatif terhadap latar akibat kamera; aktivitas manusia/hewan tidak tampak di shot ini.
- **Audio:** belum diperiksa.
- **Transition to next:** tidak ada; video selesai pada 00:19.600.

**Perkembangan awal → tengah → akhir:**
- **Awal 00:13.27:** foreground penuh sayur dan sulur, buah kecil gantung atas, jalur kecil mengarah ke kolam dan rumah di tengah belakang.
- **Tengah 00:14.39–00:16.90:** tiang dan daun dekat melewati tengah frame; rumah berpindah ke kiri, area kolam dan tanaman pisang di kanan lebih jelas.
- **Akhir 00:18.18–00:19.46:** sudut lebih terbuka, kolam menguasai tengah-bawah dengan tanaman air terpisah dalam beberapa kelompok dan pohon pisang di tepi; rumah berada di kiri.

**Bukti dan ketidakpastian:** [OBSERVASI] parallax tiang/daun dekat versus rumah jauh; [INTERPRETASI] lateral tracking kanan lebih masuk akal daripada zoom tunggal; skala/arah gerakan sebenarnya tidak diukur secara fisik. [BELUM PASTI] sumber riak permukaan dan jenis tanaman air yang tepat.

**Teknik yang dapat dipelajari:** *foreground wipe* alami dari rambatan, parallax untuk rasa kedalaman, dan reveal kolam sebagai penutup.

## 4. Plants, Fruits & Garden Layout

| Elemen | Shot dan timestamp bukti | Susunan / ciri visual | Keyakinan |
|---|---|---|---|
| Sayuran daun (selada/kubis-like) | 01: 00:00.20–00:02.66; 02: 00:06.83–00:12.87; 03: 00:13.27–00:19.46 | Roset hijau muda, beberapa kepala bulat berlapis; berbaris dalam bedengan | Tinggi bentuk; sedang spesies |
| Cabai merah/kuning | 01: 00:02.66–00:03.95; 02: 00:06.83; 03: 00:13.27 | Buah kecil meruncing di atas semak pendek | Tinggi bentuk |
| Buah bulat merah mirip tomat | 02: 00:06.83–00:09.23; 03: 00:13.27 | Buah bergerombol merah/jingga pada tanaman rendah/berpenyangga | Tinggi bentuk; sedang spesies |
| Buah oval hijau-kuning mirip pepaya | 01: 00:00.20–00:05.24 | Tandan pada batang tinggi di antara daun besar menjari | Tinggi bentuk; sedang spesies |
| Pohon berbuah kecil jingga mirip jeruk | 01: 00:03.95–00:06.43 | Tajuk padat, buah berlimpah, pembatas batu pada pangkal | Tinggi bentuk; sedang spesies |
| Rambatan buah silindris hijau panjang | 02: 00:09.23–00:12.87 | Banyak buah menjuntai dari rangka horizontal | Tinggi bentuk; rendah spesies |
| Buah hijau kecil gantung dan sulur | 03: 00:13.27–00:15.63 | Sulur, bunga kuning, daun besar menjari | Tinggi keberadaan; rendah spesies |
| Pohon pisang | 03: 00:15.63–00:19.46 | Pelepah/lempeng daun besar dekat kolam | Tinggi |
| Tanaman air dan bunga | 01: 00:00.20–00:02.66; 03: 00:16.90–00:19.46 | Daun mengapung; pada shot 01 bunga putih/pink; shot 03 kelompok hijau terpisah | Tinggi keberadaan; sedang jenis |
| Struktur bedengan, rambatan, jalur | 01–03, sepanjang shot | Kayu pembatas bedengan, jalur kerikil/ tanah, rangka vertikal dan horizontal | Tinggi |
| Kolam | 01: 00:00.20; 03: 00:13.27–00:19.46 | Kolam kecil dekoratif pada 01 dan bentang air lebih luas pada 03 | Tinggi; hubungan fisik antarkolam belum pasti |

**Struktur lapisan:** tanaman rendah → bedengan/semak berbuah → rambatan dan pohon berbuah → rumah/pohon latar. **Penataan yang layak dipelajari:** perpaduan utilitas bedengan dan komposisi taman, serta jalur melengkung yang mengarahkan pandangan.

## 5. Weather, Atmosphere & Lighting

- **Waktu:** [BELUM PASTI] jam pengambilan gambar tidak dapat ditentukan dari terang/warna langit.
- **Cuaca:** [OBSERVASI] cahaya siang alami secara tampilan, langit sebagian berawan; [BELUM PASTI] apakah gerimis atau baru selesai hujan.
- **Light quality:** sebagian besar terang dan tersebar (*soft diffused*), warna tanaman sangat jenuh; arah matahari tidak pasti.
- **Wet surfaces:** air kolam jelas; tanah tidak cukup menjadi bukti pasti hujan.
- **Water source:** kolam 01 dan 03. [BELUM PASTI] asal riak di permukaan air shot 03; tidak memaksakan klaim hujan/sprinkler.
- **Atmosphere:** [INTERPRETASI] subur, tenang, rapi, dan menyegarkan.
- **Relevant motion:** ikan tampak bergerak pada kolam 01; perbedaan gerak tanaman dekat dan latar paling kuat berasal dari gerakan kamera.

## 6. Animals, Humans & Other Objects

| Objek | Jumlah tampak | Shot dan posisi | Gerak/interaksi | Peran |
|---|---|---|---|---|
| Ikan berwarna jingga/putih | Beberapa; jumlah pasti tidak dihitung | 01, kolam depan 00:00.20–00:01.38 | Terlihat di bawah permukaan/bergerak di air | Pendukung hook awal |
| Manusia | Tidak terlihat | 01–03 | Tidak terlihat | Tidak ada |
| Hewan lain | Tidak terlihat | 01–03 | Tidak terlihat | Tidak ada |
| Bangunan hunian | Setidaknya satu tampilan bangunan per latar, tidak dipastikan sama | 01 belakang; 02 kanan atas; 03 seberang kolam | Statis | Latar/konteks taman |
| Selang irigasi | Setidaknya satu jalur hitam | 02, sepanjang tanah 00:07.96–00:12.87 | Tidak tampak air menyembur | Pendukung layout |

**Realism notes:** gerak relatif foreground dan background mengikuti perubahan sudut pandang; hubungan fisik lokasi ketiga shot tidak dapat dipastikan. Identitas manusia atau spesies hewan tidak ditebak.

## 7. Audio, Editing & Pacing

- **Audio checked:** tidak; yang terverifikasi hanyalah adanya trek audio AAC stereo, bukan isi suara.
- **Natural sound:** belum diperiksa.
- **Voice/music:** belum diperiksa.
- **Shot rhythm:** 3 shot berdurasi mirip, 6,633 / 6,433 / 6,533 dtk, masing-masing memperkenalkan area taman baru.
- **Transitions:** dua hard cut tepat sebelum frame 199 dan frame 392; tidak tampak dissolve pada batas yang diperiksa.
- **What makes editing effective:** [INTERPRETASI] variasi pembukaan kolam–buah jingga → hasil kebun gantung → wide kolam membuat perkembangan visual tanpa cut cepat.

## 8. Visual Characteristics & Reusable Inspiration

**Karakter visual penting:** (1) susunan kebun bertingkat dan sangat padat; (2) integrasi kolam dan bedengan; (3) warna kontras buah merah, jingga, hijau; (4) jalur kerikil berkelok dan struktur rambat; (5) reveal visual pelan dengan pergeseran parallax.

**Teknik yang dapat digunakan kembali:**
- Shot 01: mulailah pada subjek air dekat kamera, kemudian sapu perlahan ke tanaman berbuah.
- Shot 02: perlahan mendekat ke struktur gantung sambil mempertahankan sayuran sebagai alas frame.
- Shot 03: gunakan tiang/sulur terdekat sebagai *foreground wipe* alami menuju pemandangan kolam luas.

**Elemen opsional:** ikan, kolam, bunga ungu, pohon berbuah jingga, bentuk rumah; semua merupakan ciri referensi ini, bukan elemen wajib kebun lain.

**Hal yang sebaiknya tidak ditiru secara membabi buta:** menganggap semua perpindahan sebagai zoom atau kamera maju; mengklaim hujan aktif dari riak kolam saja; menetapkan spesies buah gantung tanpa bukti.

**Search tags:** `residential-garden`, `raised-beds`, `pond`, `ornamental-fish`, `gravel-path`, `trellis`, `hanging-fruit`, `vegetable-garden`, `slow-reveal`, `lateral-movement`.

## 9. Notes & Uncertainty

- **Belum diverifikasi:** asal platform/creator asli, hak penggunaan, lokasi kebun, jam perekaman, hubungan fisik tiga shot, spesies pasti pohon/buah panjang, sumber riak dan apakah hujan terjadi, isi audio, serta mekanisme gerak kamera fisik (pan/tracking/push-in/zoom) jika saling tumpang tindih.
- **Asumsi yang perlu diuji ulang:** buah jingga mirip jeruk; oval hijau-kuning mirip pepaya; buah panjang mirip labu; bunga ungu belum diidentifikasi.
- **Sumber informasi dari pengguna:** hanya unggahan MP4 dan instruksi analisis Gardenku; tidak ada pernyataan lokasi/cuaca yang terpisah.

**Contact Sheet Manifest — berkas JPG lokal nyata, satu per shot**

| Shot | Nama/path arsip JPG standar (bukan link GitHub) | Semua timestamp panel | Panel | Kanvas / panel / sumber | Kategori | Ukuran byte lokal |
|---|---|---|---:|---|---|---:|
| 01 | `../frames/muyon-14/shot-01.jpg` | 00:00.20; 00:01.38; 00:02.66; 00:03.95; 00:05.24; 00:06.43 | 6 | 1710×2092 / 540×960 / 720×1280 | `contact-sheet` | 1.701.993 |
| 02 | `../frames/muyon-14/shot-02.jpg` | 00:06.83; 00:07.96; 00:09.23; 00:10.42; 00:11.78; 00:12.87 | 6 | 1710×2092 / 540×960 / 720×1280 | `contact-sheet` | 1.655.756 |
| 03 | `../frames/muyon-14/shot-03.jpg` | 00:13.27; 00:14.39; 00:15.63; 00:16.90; 00:18.18; 00:19.46 | 6 | 1710×2092 / 540×960 / 720×1280 | `contact-sheet` | 1.470.421 |

**Evidence Cross-Check — Tahap 5 (pemeriksaan awal, bukan Gate A/B):**
- Shot yang belum terwakili: **tidak ada**. Semua 3 shot memiliki awal, tengah, akhir pada enam panel.
- Frame boundary: perubahan langsung 198→199 (00:06.633), 391→392 (00:13.067) dikonfirmasi melalui pembandingan frame bertetangga; tidak ada indikasi dissolve.
- Motion check: pemeriksaan perpindahan fitur antarframe mendukung arah sapuan layar kiri pada shot 01 dan 03 serta pembesaran objek dalam shot 02. Perbedaan pan fisik vs lateral tracking dan zoom vs pendekatan tetap diberi label interpretasi.
- Kualitas JPG: tiga JPG asli telah disimpan sementara secara lokal dan dapat dibaca ulang; panel 540×960, warna/rasio sumber dipertahankan; label timestamp berada di luar area gambar. Tidak digunakan gambar AI.
- Audio: track ada, **isi belum diperiksa**, sehingga tidak ada klaim tentang musik, suara burung, hujan atau percakapan.

## 10. Quality Checklist

| Gate | Status Fase 2 | Dasar penilaian |
|---|---|---|
| Gate A — Visual Accuracy | **PASS** | MP4 588 frame (19,600 detik); dua-pass inspection; tiga shot dengan dua hard cut; perkembangan awal–tengah–akhir, 3 contact sheet asli dan ketidakpastian gerak/identifikasi sesuai bukti |
| Gate B — Document & Repository Integrity | **PASS** | Analisis 10 bagian dan baris INDEX disimpan dalam satu commit pada `main`; dokumen, INDEX, dan HEAD dibaca ulang dan dibandingkan dengan konten yang ditulis. SHA dicantumkan dalam laporan verifikasi penyimpanan |
| Overall Gate | **PASS** | Gate A dan B keduanya PASS; keberadaan JPG remote bukan syarat Gate B |

**Bukti Visual (Gate A):** sumber `muyon-14.mp4` (720×1280, 30 fps, durasi trek video 19,600 s, SHA-256 `8c2af5edfb7b68475a54828404443aa9684f32d78544f5d06fe3207ee8ae58e6`); batas shot terperiksa pada frame 198/199 dan 391/392; 3 contact sheet asli 6 panel masing-masing, dimensi 1710×2092 dan panel 540×960. Audio track ditemukan tetapi isi audio tidak diaudit dan tidak dibuat klaim suara.

**Bukti Repository (Gate B):** path dokumen `references/muyon/analysis/muyon-14.md` dan indeks `references/INDEX.md`; SHA commit serta HEAD `main` dilaporkan dalam jawaban penyimpanan setelah verifikasi baca ulang. Path JPG di manifest merupakan lokasi arsip, bukan klaim unggah atau hyperlink remote.

**Status:** `draft`; perintah `save now` mengizinkan penyimpanan, **bukan** persetujuan `approved`.

**Ketidakpastian yang dipertahankan:** suara belum diperiksa, nama spesies tertentu belum pasti, gerak kamera fisik pan/tracking/push-in/zoom tidak selalu bisa dipisahkan, sumber riak air dan riwayat hujan tidak dibuktikan.

- [x] Video asli diperiksa; struktur 3 shot dan timestamp dicatat tanpa menebak.
- [x] Deep shot analysis berisi observasi, interpretasi, serta awal–tengah–akhir.
- [x] Contact Sheet Manifest mencantumkan tiga JPG beserta timestamp, dimensi dan ukuran byte.
- [x] Pemeriksaan silang bukti Fase 1 terdokumentasi.
- [x] Dokumen Markdown dan INDEX disimpan serta diverifikasi pada `main`.
- [x] Tanpa mengunggah JPG/MP4, tanpa branch dan tanpa Pull Request.

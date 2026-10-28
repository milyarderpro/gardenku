# Aturan Analisis Video Referensi — Gardenku
**Versi:** 1.3 — Opsi B+ Two-Phase Workflow + Manual Upload Fallback (Analyze & Review → Save & Verify)  
**Berlaku untuk:** `references/<creator>/analysis/<video-id>.md`  
**Tujuan:** Mengubah video asli menjadi catatan visual yang akurat dan bisa dipakai ulang oleh AI untuk mengembangkan konsep video kebun.

> Dokumen ini berisi **aturan kerja**, bukan hasil analisis video tertentu. Format berkas analisis baku tersedia di `templates/video-analysis.md`.

## 1. Kapan aturan ini digunakan?
Gunakan saat pengguna meminta AI menonton, mengamati, memecah shot, atau menganalisis **video referensi kebun**. **Jangan membuat ide atau prompt video** apabila pengguna hanya meminta analisis.

Baca `AGENTS.md`, lalu cek [INDEX](../references/INDEX.md) dan file analisis yang ada. Sumber video **selalu MP4 unggahan chat dari pengguna** (aslinya disimpan pengguna di PC). GitHub **tidak menyimpan MP4**; hanya analisis dan JPG ekstraksi. Contoh:
- Input: pengguna mengunggah `muyon-01.mp4` di chat (nama input dapat berbeda).
- Analisis: `references/muyon/analysis/muyon-01.md`.
- JPG bukti: `references/muyon/frames/muyon-01/`.

Katalog mencatat **referensi**, bukan lokasi MP4 yang dapat diunduh. Saat membuka sesi baru, minta unggahan MP4 hanya bila belum tersedia/dapat dibaca di sesi tersebut.

## 2. Prinsip wajib
1. **Utamakan yang benar-benar terlihat atau terdengar.** Bila video tidak dapat dibuka, jelaskan keterbatasannya; jangan menyusun analisis lengkap seolah sudah menonton.
2. **Pisahkan sumber informasi:**
   - `[OBSERVASI]` — terlihat/terdengar pada video atau frame asli.
   - `[KONTEKS PENGGUNA]` — informasi yang disampaikan pengguna, misalnya "setelah hujan deras".
   - `[INTERPRETASI]` — perkiraan atau penilaian teknis AI.
   - `[BELUM PASTI]` — detail belum dapat diperiksa atau bukti kurang kuat.
3. **Cantumkan timestamp** untuk temuan penting. Gunakan kata "perkiraan" untuk batas shot/waktu yang tidak diukur secara presisi.
4. **Jangan menebak** nama tanaman, jenis buah, jam pengambilan gambar, identitas orang, alat kamera, ukuran lahan, jumlah shot, atau jenis suara tanpa bukti.
5. **Jaga konteks:** referensi kebun terbuka, pekarangan depan, backyard, rooftop, dan kebun dalam pot **bisa sangat berbeda**. Jangan memaksakan karakter kebun luas pada referensi lahan kecil.
6. **Hewan, manusia, kolam, alat, dan cuaca adalah elemen opsional**: periksa keberadaannya, tetapi tulis "tidak terlihat" bila tidak ada.
7. **MP4 asli disimpan di PC pengguna; jangan mengubah atau menghapus salinan pribadi.** Tidak perlu menyimpan/mengunggah MP4 ke GitHub. JPG yang diperoleh dengan ekstraksi tetap karya turunan dari video; periksa hak penggunaan saat repo publik.

## 3. Urutan analisis

**Two-Pass Video Inspection wajib:** (1) *Pass 1 / Video Structure Mapping* telusuri seluruh timeline, sampling awal sekitar 0,5–1 detik lalu lebih rapat dekat cut/dissolve, buat Shot Map; (2) *Pass 2 / Deep Shot Analysis* periksa tiap shot dan gerak video asli dari awal hingga akhir. Interval sampling bukan pengganti melihat video bergerak. Waktu yang belum presisi wajib ditandai `perkiraan`.

### A. Identitas dan gambaran keseluruhan
Catat identitas sumber/kreator, nama video, lokasi file, durasi, resolusi, aspek rasio, dan FPS **jika dapat diverifikasi**. Catat tautan sumber asli dan izin penggunaan bila tersedia; bila tidak, tulis "belum diketahui".

Tuliskan ringkasan 3–5 kalimat mengenai:
- Jenis kebun dan perkiraan karakter ruang: kebun terbuka luas, front-yard kecil, backyard, pot, hydroponic, dan sebagainya.
- Tingkat kerimbunan, jenis tanaman dominan, keberadaan bedengan/lorong/trellis/kolam.
- Gaya kamera dan suasana utama.
- Apa yang membuat video menarik sejak detik awal (*visual hook*).

### B. Pecah menjadi shot
**Shot** = gambar kontinu di antara dua cut. **Scene** = kesatuan tempat/kejadian; dapat memuat beberapa shot. **Clip** = segmen/file digital. Jangan menyamakan ketiganya.

Untuk **setiap shot**, catat:
- Nomor shot, waktu mulai–akhir, dan durasi (tepat atau perkiraan).
- **Hero subject:** tanaman, buah, aktivitas, atau detail yang paling menonjol.
- Subjek pendukung dan apa yang terlihat di awal, tengah, akhir.
- **Camera movement:** static, pan left/right, tilt up/down, tracking lateral, push-in/dolly-in, pull-back, zoom; tulis gabungan hanya jika tampak nyata.
- **Framing dan angle:** wide/medium/close-up, jarak relatif, posisi kamera tinggi/rendah, arah pandang.
- **Komposisi:** foreground, middle ground, background; cara warna buah/daun dan elemen lain mengarahkan perhatian.
- **Garden layout:** bedengan, jalan setapak, batas bata/kayu/batu, pot, trellis, pohon buah, aliran air, kolam, rumah/pagar.
- Cuaca, kualitas cahaya, warna dan kondisi permukaan.
- Jenis transisi menuju shot berikut jika terlihat.

**Perbedaan gerak kamera:** pan = kamera berputar kiri/kanan; tilt = berputar atas/bawah; tracking = kamera berpindah posisi menyamping; push-in = posisi kamera mendekati objek; zoom = pembesaran optik/digital. Jangan menyebut semua gerak sebagai "kamera maju". **Verifikasi gerak dari MP4**, bukan dari JPG saja. Jika pan, tracking atau zoom sulit dibedakan, tulis `[INTERPRETASI]` dan tingkat keyakinannya. Catat perkembangan visual **awal → tengah → akhir** tiap shot.

### C. Detail lingkungan, cuaca, dan air
Periksa bila relevan:
- Kondisi waktu: pagi, siang, sore **hanya jika ada bukti**; langit mendung sendiri tidak membuktikan jam.
- Cahaya: hangat/dingin, langsung/tersebar, arah cahaya, bayangan, warna keseluruhan.
- Hujan: sebelum/setelah hujan, gerimis aktif, tetes di daun, permukaan basah, genangan, kabut.
- **Bedakan gerimis alami, sprinkler, selang, air terjun/kolam, dan percikan dari hewan.** Jika sumber air tidak jelas, tandai `[BELUM PASTI]`.
- Gerakan alam: daun, angin, air mengalir, riak kolam.

Jika pengguna menyebut "setelah hujan deras, masih gerimis", cantumkan sebagai `[KONTEKS PENGGUNA]` dan cari bukti visual yang mendukung; jangan mengklaim bahwa intensitas gerimis terukur jika tidak terlihat.

### D. Hewan, manusia, alat, dan aktivitas
Untuk objek yang **memang tampak**, catat: jenis umum, jumlah yang terlihat, posisi dalam frame, timestamp, gerakan, interaksi dengan kebun, serta peran visual (**utama / pendukung / latar**).

Contoh: ayam mematuk tanah di samping bedengan, bebek berenang di tepi kolam, ikan menghasilkan riak air, manusia memakai caping sedang memanen cabai, keranjang diletakkan di jalan. Ini adalah **contoh kategori**, bukan klaim mengenai referensi tertentu.

Jangan menebak identitas orang, hubungan keluarga, atau niat/emosi hewan. Catat penampilan umum hanya sebatas yang relevan secara visual.

### E. Audio, editing, dan ritme
Jika audio benar-benar dapat diperiksa, catat suara air/hujan/angin/burung/hewan/langkah, percakapan, musik, serta hubungannya dengan gambar. Jika tidak, tulis **"audio belum diperiksa"**. Bedakan suara asli video dengan musik tambahan bila memungkinkan.

Catat jumlah shot, kisaran durasi shot, pola urutan subjek, hard cut/dissolve (jika dapat diamati), dan tempo perubahan visual.

## 4. Kesimpulan untuk pustaka AI
Akhiri analisis dengan empat bagian:
1. **Karakter visual utama:** maksimal 5 ciri khas yang benar-benar terdukung.
2. **Teknik yang dapat digunakan kembali:** misalnya transisi fokus dari tomat dekat kamera menuju pohon pepaya di belakang, atau slow pan melintasi bedengan setelah hujan.
3. **Elemen khas tetapi tidak wajib ditiru:** misalnya manusia, bebek, kolam, atau jenis buah tertentu.
4. **Keterbatasan / ketidakpastian:** data mana yang masih memerlukan pemeriksaan.

Tambahkan **tag pencarian** bila faktanya didukung, misalnya `front-yard`, `open-field`, `after-rain`, `light-drizzle`, `slow-pan`, `bamboo-trellis`, `pond-fish`. Jangan membuat tag berdasarkan dugaan.



## 5. Workflow Opsi B+ — 7 tahap resmi

**Metode:** Evidence-Driven Video Analysis + Adaptive Per-Shot Contact Sheet + Dual Verification Gate. **Ketujuh tahap tetap berlaku tetapi dibagi menjadi dua fase dengan batas izin yang wajib.** MP4 **dikirim melalui chat dan disimpan pengguna di PC**, tidak diunggah ke GitHub. Repository hanya menyimpan hasil analisis dan contact sheet yang sudah mendapat izin simpan. Bagian ini sumber **aturan baku**; AGENTS adalah navigasi dan template adalah format keluaran.

### Batas izin dua fase (WAJIB)

**FASE 1 — Analyze & Review (Tahap 1–5)**

- **Pemicu:** pengguna mengunggah MP4 dan meminta analisis. AI **boleh membaca** aturan, template, INDEX dan analisis lama dari repo, serta memproses MP4 dan membuat file JPG/contact sheet **sementara secara lokal** untuk diperlihatkan kepada pengguna.
- Kerjakan kelima tahap sampai **Evidence Cross-Check**. Tampilkan hasil analisis lengkap, Shot Map, **file JPG contact sheet asli per shot yang dapat diunduh secara individual**, catatan ketidakpastian, dan versi yang siap direview. Catat nama JPG, timestamp panel, dimensi, ukuran byte, serta **SHA Git blob lokal jika dapat dihitung**, agar JPG **yang sama** dapat diunggah ke GitHub pada Fase 2 tanpa ekspor/kemasan ulang. **Berhenti setelah Tahap 5** untuk menunggu umpan balik atau perintah simpan.
- **Larangan selama Fase 1:** tidak boleh menambah/mengubah/menghapus file GitHub, membuat `pending` baru, mengunggah JPG, memperbarui INDEX, membuat branch/commit/PR, atau mengubah status repo, **meskipun video baru belum ada dalam katalog**. Seluruh data Fase 1 adalah **draft lokal/percakapan**, bukan data yang sudah tersimpan pada repository.
- Pengguna boleh meminta revisi berulang. Perbarui **analisis dan contact sheet versi terbaru** sesuai bukti tanpa mengubah repository. **Review pengguna tidak otomatis membuat status `approved`**. Laporkan kesiapan Fase 1 secara deskriptif, **bukan** dengan Gate A/B/overall PASS.
- Pada Fase 1 **Gate A/B/overall berstatus `belum dijalankan`**. Evidence Cross-Check adalah pemeriksaan awal, **bukan** Dual Verification Gate resmi. Jika MP4 gagal dibaca, laporkan bahwa analisis belum bisa dilanjutkan; jangan mengarang dan jangan menulis status Gate resmi `FAIL` sebelum Fase 2.
- Usahakan tetap berada pada **chat yang sama** sampai disimpan: MP4, contact sheet, dan berkas sementara mungkin tidak bertahan pada sesi lain. Tidak boleh mengklaim artefak lokal tetap tersedia bila belum diperiksa.

**HUMAN REVIEW — STOP**: **`save now`** (tidak peka huruf besar/kecil) adalah perintah eksplisit untuk melewati batas menuju Fase 2 bagi **analisis video terakhir yang sedang direview dalam percakapan**. Kata umum seperti `lanjut`, `oke`, atau sekadar revisi **bukan** izin menyimpan. Jika ada beberapa video atau versi yang benar-benar ambigu, pastikan target sebelum menulis. Jika pengguna secara jelas meminta penyimpanan dengan kata lain, hormati instruksi eksplisitnya; jangan menafsirkan persetujuan umum sebagai izin.

**FASE 2 — Save & Verify (Tahap 6–7)**

- **Pemicu:** pengguna mengetik **`save now`** (atau memberi instruksi penyimpanan yang sama jelasnya) **setelah Fase 1 untuk target yang diketahui**. Gunakan **hasil revisi terakhir** dan contact sheet yang sesuai; jangan menggunakan draft lama.
- Sebelum upload, pastikan JPG lokal, video/bukti yang diperlukan, versi analisis final, dan ID target masih dapat diakses. Jika sumber/berkas sementara hilang atau tidak utuh, **hentikan penulisan yang terkait**, jelaskan kekurangan dan minta pengguna mengunggah ulang file yang diperlukan; jangan menciptakan frame/metadata sebagai pengganti.
- Simpan `analysis/<id>.md`, contact sheet JPG, dan `references/INDEX.md` sebagai **satu paket perubahan yang konsisten dalam branch khusus**. Idealnya satu commit; **jika memakai fallback upload manual, media diunggah lebih dahulu dalam commit staging pada branch tersebut**, kemudian Markdown dan INDEX di-commit **hanya setelah keempat/semua JPG lolos verifikasi**. Jangan membuka PR sebelum paket lengkap. Referensi baru dibuat dan dimasukkan INDEX **hanya pada fase ini**; status laporan AI menjadi `draft` kecuali ada persetujuan eksplisit berbeda.
- **Default keamanan GitHub:** commit pada **branch kerja khusus**, buka Pull Request ke `main` untuk tinjauan; **jangan merge otomatis**. Jika pengguna menentukan branch tujuan secara eksplisit, ikuti instruksinya. Bedakan dengan jelas **tersimpan di branch/PR** dan **sudah masuk `main`**.
- Setelah penyimpanan, jalankan **Gate A — Visual Accuracy** dan **Gate B — Repository Integrity** sebagai pemeriksaan resmi. Laporkan keduanya dan **overall PASS/PARTIAL/FAIL**, sertakan bukti commit, tautan, serta keterbatasan. Bila penyimpanan parsial/gagal, jangan mengklaim sudah selesai semua.
- Perintah **`save now` bukan persetujuan `approved` ataupun izin untuk merge PR**. Sesudah Fase 2 selesai, perubahan lain perlu instruksi baru.

### Fallback wajib jika konektor tidak bisa mengirim JPG biner (bagian Tahap 6, bukan fase ketiga)

**Tujuan:** mencegah Fase 2 terhenti hanya karena batas transfer JPG. Utamakan upload otomatis jika alat benar-benar mendukung byte biner dan hasil dapat diverifikasi. Jika tidak didukung, upload gagal, atau ukuran payload melampaui batas, **beralih ke manual upload fallback; jangan mengulang Fase 1 atau mengurangi kualitas JPG semata-mata untuk meloloskan konektor.**

1. **Preflight setelah `save now`:** pastikan ID, draft analisis **versi paling baru**, JPG lokal per shot, jumlah panel, ukuran byte, format/dimensi JPEG dan checksum **Git blob SHA-1** tiap JPG. Hash biasa (SHA-256) bukan pengganti Git blob SHA-1; bila belum dapat dihitung tandai belum diverifikasi dan hitung sebelum finalisasi. Bedakan *file di chat/lokal* dari file GitHub.
2. **Buat branch staging khusus dari `main`** (contoh `save/muyon-02-contacts`). Pada fallback, branch ini boleh sementara berisi **JPG saja**. **Tidak boleh menulis/menautkan Markdown analisis final atau mengubah INDEX sebelum semua JPG diverifikasi.** Tidak membuat PR atau merge selama staging belum lengkap.
3. **Gunakan JPG hasil Fase 1, tanpa membuat ZIP:** file `shot-XX.jpg` yang sudah ditampilkan dan dapat diunduh pada Fase 1 adalah **file final untuk upload**. **Tidak perlu mengemas ulang, mengekspor ulang, membuat ZIP, atau mengirim salinan kedua** selama file asli tersebut masih tersedia. Tunjukkan **lokasi/tautan yang sudah ada dari Fase 1** dan daftar nama/path tujuan persis `references/<creator>/frames/<video-id>/shot-XX.jpg`; gunakan Contact Sheet Manifest yang telah dibuat pada Fase 1 sebagai acuan nama, panel, timestamp, dimensi, byte dan SHA Git blob lokal yang benar-benar terukur. Petunjuk bagi pengguna: unduh JPG individual **yang sama** dari Fase 1 jika belum ada di perangkat → pilih **branch staging** → folder target → **Add file → Upload files** → unggah JPG → commit pada **branch staging yang sama**. Jangan mengarahkan pengguna ke `main` dan jangan mengunggah arsip sebagai pengganti JPG.
4. **Tunggu konfirmasi pengguna** seperti `4 JPG sudah di-upload`. Konfirmasi ini **hanya melanjutkan Fase 2 yang sudah diizinkan dengan `save now`**, bukan izin baru untuk merge atau approve. Jika file JPG lebih banyak/lebih sedikit, sesuaikan jumlahnya dengan Shot Map dan Manifest, **bukan selalu empat**.
5. **Verifikasi upload yang sebenarnya:** baca tree branch GitHub, cocokkan **seluruh path/nama, jumlah JPG, ukuran byte, Git blob SHA** dengan **JPG/Contact Sheet Manifest Fase 1**; pastikan file yang sebelumnya valid secara lokal identik dengan GitHub. Jika SHA cocok, identitas binernya terbukti, tetapi **jangan mengaku telah melihat render UI GitHub** jika belum dilakukan. Bila ada file kurang, salah branch, nama berbeda, ukuran/SHA tidak cocok, **STOP dan minta perbaikan; jangan commit Markdown atau INDEX**. Tidak perlu mengulang analisis jika bukti lokal masih utuh.
6. **Finalisasi setelah seluruh JPG cocok:** buat/ubah analisis 10 bagian dengan link nyata, Contact Sheet Manifest, hasil review paling baru, dan INDEX pada **satu commit Markdown/INDEX terkoordinasi di branch staging**. Periksa ulang HEAD/tree/tautan, lalu buka PR untuk ditinjau, **tanpa merge otomatis**; sesudah itu lakukan Gate A/B dan laporkan overall. PR/branch staging saja **belum berarti masuk `main`**.
7. **Bila pengguna belum upload atau koneksi masih gagal:** beri status `Fase 2 — menunggu upload manual` atau `terhambat`, dan rincikan file yang masih kurang. **Gate B dan overall tidak boleh PASS**, data di `main` tidak berubah. Jangan melakukan commit parsial Markdown yang merujuk JPG belum ada. **Jangan hapus branch staging atau file pengguna tanpa instruksi**. Saat pengguna kembali dengan konfirmasi, verifikasi keadaan repo lagi, lalu lanjutkan Fase 2 tanpa meminta `save now` ulang untuk target sama.
8. **Jika konteks atau file lokal hilang di chat baru:** jangan mengarang ukuran/hash/timestamp dan jangan mengaku masih memiliki MP4. Utamakan **JPG individual dari Fase 1 yang telah disimpan pengguna** + draft/manifest sebagai sumber pemulihan; jika tidak tersedia, jelaskan file mana yang perlu dikirim ulang. **Jangan membuat ZIP baru** untuk menggantikan JPG yang sudah diberikan; minta MP4 hanya bila diperlukan untuk ekstraksi ulang yang memang tidak dapat dihindari atau untuk memeriksa ulang klaim visual. Laporan Gate A harus menyebut cakupan bukti yang masih dapat dibuktikan.

**Hasil setelah `save now`:** (a) jika upload otomatis berhasil, gunakan jalur normal; (b) jika tidak, **AI mengarahkan pengguna mengunggah JPG yang telah diberikan di Fase 1 dan kemudian memverifikasinya**, lalu AI menyelesaikan Markdown/INDEX/PR/Gate. **Tidak perlu membuat ZIP atau mendistribusikan ulang JPG yang sama.** Mekanisme staging dan bantuan upload **tidak mengubah larangan penulisan apa pun saat Fase 1**.

**Ringkasan:** `MP4 dari chat → Tahap 1–5 → review/revisi → STOP → "save now" → Tahap 6–7 → laporan Gate`.

### Tahap 1 — Video Input & Validation

- Tetapkan ID unik; periksa [INDEX](../references/INDEX.md) dan analisis sebelumnya. Gunakan MP4 yang **benar-benar dapat dibaca dari chat**; nama file atau metadata saja tidak membuktikan isi video.
- Catat nama input, tanggal pemeriksaan, durasi, FPS, resolusi, rasio aspek, ukuran byte/hash **jika tersedia**, serta cakupan yang berhasil diperiksa. **Jika berbeda, bedakan durasi kontainer, trek video, dan trek audio; jangan menghitung durasi gambar hanya dari durasi kontainer × FPS.** Jika **pengguna meminta analisis sekarang** tetapi input tidak dapat diakses, jangan mengarang temuan atau membuat frame palsu; nyatakan **Fase 1 belum dapat diselesaikan**. Gate A/B/overall **belum dijalankan** hingga perintah simpan dan proses verifikasi resmi. Dokumen administratif `pending` juga tetap memiliki Gate `belum dijalankan`.
- Audio: bedakan keberadaan audio track dari suara yang benar-benar didengar. Bila tidak diaudit, tulis `audio belum diperiksa`; tidak boleh mengarang audio.
- Jangan meminta upload ulang bila video sudah dapat diakses pada sesi ini.

### Tahap 2 — Video Structure Mapping (Pass 1)

- Telusuri **seluruh timeline** dengan sampling awal sekitar **0,5–1 detik** atau adaptif; deteksi jumlah shot kontinu, cut/dissolve, objek atau tempat yang berubah, dan bagian hitam.
- Periksa **lebih rapat** dekat batas transisi, bukan menebak batas presisi dari interval sampling. Susun **Shot Map** (ID, start–end, durasi, transisi, ketepatan waktu, cakupan), lalu periksa kembali pada Pass 2.
- Jika bagian video belum dapat diperiksa, sebutkan rentangnya; jangan menyatakan seluruh video telah ditinjau.

### Tahap 3 — Deep Shot Analysis (Pass 2)

- Periksa gerakan **MP4 asli** per shot: hero subject, tanaman/buah, susunan foreground/middle/background, kerapatan, bedengan/jalur/trellis/kolam, cuaca/cahaya, sumber air, hewan/manusia, aktivitas, transisi dan audio bila diperiksa.
- Jelaskan perkembangan **awal → tengah → akhir**, termasuk objek yang muncul/hilang dan perubahan komposisi. Bedakan pan, tilt, tracking, push-in, zoom dan gerakan objek; jika ambigu beri label `[INTERPRETASI]` atau `[BELUM PASTI]` plus tingkat keyakinan.
- Setiap klaim penting memiliki shot/timestamp dan dipisahkan menjadi `[OBSERVASI]`, `[KONTEKS PENGGUNA]`, `[INTERPRETASI]`, `[BELUM PASTI]`. Jangan menyamakan sprinkler/selang dengan hujan.

### Tahap 4 — Adaptive Per-Shot Contact Sheet

**Aturan utama: satu shot = satu JPG contact sheet `shot-XX.jpg`**, di `references/<creator>/frames/<video-id>/`. Setiap JPG berisi beberapa **panel frame sumber** berurutan, bukan JPG individual untuk setiap detik.

- **Target 3–6 panel per shot**, adaptif: shot pendek/statis boleh 2–3; shot panjang/kompleks bisa 6–10+ bila memang perlu. Jumlah **bukan kuota kaku**; satu shot satu JPG adalah format utama, dengan pengecualian `shot-XX-part-01.jpg` dll. hanya jika satu lembar terlalu padat untuk dibaca dan alasannya dicatat.
- Seleksi dari **awal, perkembangan, akhir**, serta perubahan kamera/objek/komposisi yang benar-benar informatif. Hindari hampir-duplikat, blur, dan frame di tengah dissolve (kecuali untuk bukti transisi).
- Urutkan panel menurut **timestamp sumber** dari kiri ke kanan, lalu atas ke bawah. Setiap panel diberi label waktu **di luar area gambar**, contoh `00:02.10`; layout enam panel vertikal lazimnya **3 kolom × 2 baris**.
- **Panel berasal dari MP4 asli**, tanpa generasi AI, upscale, perubahan objek, atau pemotongan yang menyesatkan. Pertahankan rasio aspek dan warna sumber. Target lebar tiap panel **480–720 px jika resolusi sumber/transfer memungkinkan** dan label mudah dibaca. **Target kualitas ini harus diuji, bukan diasumsikan berhasil**.
- **Perbedaan ukuran sumber vs contact sheet:** panel dapat diperkecil **secara wajar** dari resolusi frame asli untuk memenuhi target keterbacaan 480–720 px; ini tetap **`shot-XX.jpg` (contact sheet standar)** jika panel jelas, proporsi/isi tidak berubah, dan ukuran sumber, ukuran panel, serta kanvas dicatat. Contoh: sumber 720×1280 menjadi panel 540×960 **tidak otomatis** disebut preview. **Wajib gunakan `shot-XX-preview.jpg`** jika resolusi diturunkan **di bawah target keterbacaan** karena batas transfer/alat, atau hasil tidak cukup detail untuk analisis; catat penurunan mutu secara terbuka. Jangan meng-upscale atau mengklaim panel beresolusi sumber jika sudah diperkecil. Frame individual boleh dipakai **sementara secara lokal** tetapi tidak diunggah sebagai standar utama.
- **Contact Sheet Manifest** (satu baris per shot/JPG): Shot ID, nama file lokal/tautan JPG **hanya jika sudah terunggah**, semua timestamp panel, jumlah panel, dimensi kanvas dan panel, tipe contact-sheet/preview, dan status penyimpanan. **Fase 1:** gunakan `lokal — belum diunggah`; **sertakan JPG individual yang dapat diunduh** dan catat SHA Git blob **lokal** serta ukuran byte bila terukur. Jangan mengisi SHA GitHub, commit, atau URL repo yang belum ada. **Fase 2:** gunakan **JPG yang sudah diberikan di Fase 1**, bukan menghasilkan ZIP atau salinan baru; setelah verifikasi upload, lengkapi SHA Git blob GitHub, byte, link repo dan hasil pemeriksaan render/path.

### Tahap 5 — Evidence Cross-Check

- Cocokkan Shot Map, MP4 bergerak, laporan per shot, timestamp panel, contact sheet, dan tag. Pastikan semua shot penting tercakup, **perubahan awal–akhir benar**, serta klaim objek/gerakan sesuai bukti.
- Ambiguitas kamera diuji ulang melalui MP4, objek kecil melalui frame sumber resolusi lebih baik. Catat confidence; jangan menyimpulkan spesies/gerimis atau suara bila bukti tidak cukup.
- Bedakan `tidak terlihat`, `belum diperiksa`, dan `belum pasti`. Jangan menambah gambar AI atau tautan belum ada. **Setelah tahap ini, sajikan hasil untuk review, tunggu revisi atau `save now`, dan jangan menjalankan Tahap 6–7 tanpa izin.**

### Tahap 6 — Repository Save

**HANYA SETELAH `save now`/izin simpan eksplisit untuk target yang jelas. Tidak dijalankan saat Fase 1.**

- Siapkan `analysis/<id>.md` dengan **10 bagian template + Shot Map + Contact Sheet Manifest**, JPG terverifikasi, dan baris INDEX yang konsisten. Usahakan **satu commit terkoordinasi** pada branch yang disetujui pengguna.
- Gunakan **Git blob biner** untuk JPG, bukan teks Base64 bernama JPG. Jika konektor tidak bisa mengirim byte, **gunakan fallback upload manual pada branch staging** yang dijelaskan di atas. Sebelum commit Markdown/INDEX, uji JPEG/dimensi secara lokal dan cocokkan SHA Git blob, byte serta path dengan **JPG yang benar-benar sudah diunggah**. Jika berbeda, **jangan commit Markdown/INDEX**.
- **Sesudah push:** periksa HEAD, tree, link Markdown, resolusi, jumlah gambar/panel, status INDEX, dan bahwa **tidak ada MP4 dalam tree repo**. Jika render jarak jauh tidak dapat diperiksa, nyatakan batasannya.
- Jangan hapus **legacy preview** sebelum contact sheet pengganti **terunggah dan diverifikasi**. Bila transfer gambar berkualitas tinggi gagal, simpan JPG lokal untuk pengguna dan tandai `belum diunggah` di manifest; **jangan mengklaim Gate B PASS**.

### Tahap 7 — Dual Verification Gate

**HANYA PADA FASE 2 setelah Repository Save; selama Fase 1 status Gate A/B/overall adalah `belum dijalankan`.**

**Gate A — Visual Accuracy** wajib memeriksa:
1. Sumber MP4 dan cakupan video benar-benar diperiksa, Pass 1 + Pass 2 serta Shot Map lengkap/ketidaklengkapannya dinyatakan.
2. Shot penting terwakili dan panel memperlihatkan perubahan signifikan, berurutan dengan timestamp yang benar.
3. Setiap klaim, kamera, buah/tanaman, cuaca/air, dan aktivitas memiliki bukti shot/timestamp serta confidence saat tidak pasti.
4. Audio dinyatakan sesuai cakupan (tidak otomatis gagal bila audio di luar permintaan analisis visual, tetapi tidak mengarang suara).

**Gate B — Repository Integrity** wajib memeriksa:
1. Contact sheet JPG **valid dan terbaca** dengan panel/timestamp sesuai Manifest, rasio/dimensi memadai; file dari MP4 asli, bukan gambar AI.
2. SHA Git blob, byte, path, jumlah file/panel, tautan, commit dan branch HEAD benar. Bila render melalui UI GitHub tak dapat diperiksa, batasan dilaporkan; **SHA Git blob dan byte yang cocok dengan JPEG yang sudah berhasil dibuka lokal dapat membuktikan identitas biner, tetapi bukan bukti bahwa UI GitHub telah ditinjau langsung**.
3. Analisis **10 bagian**, Shot Map/Manifest dan INDEX konsisten; tidak ada MP4 di tree. Penggantian legacy JPG tidak menyisakan link rusak.

**Hasil:** `belum dijalankan` selama **Fase 1** (termasuk referensi `pending` maupun draft lokal yang sedang direview); `PASS` bila kriteria wajib Fase 2 dalam cakupan terpenuhi; `PARTIAL` bila pemeriksaan/unggah/coverage masih kurang tetapi data yang ada valid; `FAIL` bila verifikasi resmi Fase 2 menemukan sumber tak dapat diperiksa, isi direka, gambar salah/rusak atau keberhasilan penyimpanan tidak dapat dipastikan. **Overall**: `PASS` hanya jika A dan B PASS; `FAIL` jika salah satu FAIL; sisanya `PARTIAL`. Simpan A/B/overall, alasan, dan bukti commit.

**Status terpisah dari Gate:** `pending` (belum dianalisis), `draft` (AI telah menganalisis tetapi belum disetujui), `reviewed` (ditinjau pengguna), `approved` (persetujuan **eksplisit** pengguna). Gate PASS **tidak membuat status otomatis approved**. INDEX adalah sumber status ringkas; README tidak menyalin angka status.

**Hak dan riwayat:** Repo publik tidak otomatis mengizinkan distribusi frame. MP4 yang dihapus dari tree Git masih mungkin ada dalam riwayat commit lama; pembersihan sejarah Git bukan bagian analisis rutin.

## 6. Pemeriksaan sebelum selesai

**Periksa dua kali sesuai fase:** akhir Fase 1 hanya **kesiapan review lokal** dan larangan menulis ke repo; setelah `save now` periksa Gate A+B serta hasil commit. Jangan menandai Gate telah PASS sebelum penyimpanan diverifikasi.

- [ ] Fase 1 berhenti sesudah tahap 5, menampilkan hasil dan contact sheet lokal tanpa perubahan apa pun di GitHub.
- [ ] Fase 2 dimulai hanya setelah `save now`/instruksi simpan jelas untuk target dan versi analisis terbaru.
- [ ] Benar-benar mengakses video/frame asli, atau dengan jelas melaporkan jika tidak bisa.
- [ ] Setiap shot memiliki perkiraan timestamp, subjek, kamera, komposisi, dan layout.
- [ ] Cuaca, sumber air, manusia, hewan, suara dicatat sesuai bukti atau sebagai belum pasti/tidak terlihat.
- [ ] Ada ciri visual dan pelajaran yang bisa digunakan ulang.
- [ ] Sumber MP4 unggahan chat dan cakupan pemeriksaan dicatat; **tidak ada kewajiban MP4 di GitHub**.
- [ ] Shot Map (Pass 1) dan Deep Shot Analysis (Pass 2) mencakup video atau gap dicatat.
- [ ] Satu contact sheet JPG per shot berisi panel kronologis yang informatif dan label timestamp terbaca.
- [ ] Manifest memuat semua timestamp panel, dimensi, SHA Git blob, byte, path dan status upload nyata.
- [ ] Evidence Cross-Check memeriksa gerak kamera, objek, sumber air, dan perubahan visual terhadap MP4.
- [ ] Gate A Visual Accuracy dan Gate B Repository Integrity masing-masing dinyatakan PASS / PARTIAL / FAIL dan overall konsisten.
- [ ] Jika upload biner otomatis gagal, fallback **branch staging → JPG asli yang sudah diberikan di Fase 1 → upload pengguna → verifikasi SHA/byte/path → commit Markdown/INDEX → PR → Gate** diterapkan tanpa mengulang Fase 1 dan tanpa ZIP baru.
- [ ] Tidak ada MP4 di repo; INDEX/status/link cocok dan tidak ada klaim JPG yang belum diunggah.
- [ ] Tidak membuat ide maupun prompt sebelum diminta.

**Prioritas utama: analisis yang jujur, terstruktur, dan bisa dilacak kembali ke referensi aslinya.**

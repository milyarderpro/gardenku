# Video Analysis — [Creator] / [Video ID]

> **TEMPLATE — belum berisi temuan nyata.** Gunakan sebagai **draft lokal untuk review Fase 1**, lalu simpan sebagai `references/<creator>/analysis/<video-id>.md` **hanya pada Fase 2 setelah `save now`/izin penyimpanan eksplisit**. Ikuti [aturan analisis](../rules/analysis.md). Jangan isi berdasarkan dugaan atau nama file saja.

## 1. Reference Information

| Field | Isi |
|---|---|
| Video ID | `[creator-01]` |
| Creator / Source | [nama kreator atau sumber] |
| Input MP4 (chat) | [nama file yang diunggah pengguna / belum diterima] |
| Video storage | PC pengguna; **tidak disimpan di repo** |
| Evidence input | [MP4 chat yang diperiksa / hanya frame / sebagian / belum diperiksa] |
| Input metadata | [ukuran byte dan hash file bila tersedia; **bukan** hash yang ditebak] |
| Contact sheet path | `../frames/[creator-01]/` — lokasi JPG yang dikelola pengguna lewat repo lokal; tidak mengharuskan JPG sudah ada di remote |
| Source URL | [tautan asli atau **belum diketahui**] |
| Rights / Permission | [izin/status hak penggunaan atau **belum diketahui**] |
| Analysis date | [YYYY-MM-DD atau belum dianalisis] |
| Workflow phase | `Fase 1 — review lokal` / `Fase 2 — save & verify` |
| Save authorization | `belum ada` / `save now` (atau instruksi eksplisit lain) + waktu/versi jika diketahui |
| Repository save | `belum disimpan` / `main` + commit SHA yang benar-benar diverifikasi; **hanya Markdown + INDEX** |
| Analysis status | `pending` (belum dianalisis) / `draft` / `reviewed` / `approved`; **Fase 1 bukan perubahan status repo** |
| Gate A / Gate B / Overall | Fase 1: `belum dijalankan`; Fase 2: `PASS` / `PARTIAL` / `FAIL` sesuai akurasi analisis (A) dan integritas dokumen/INDEX di `main` (B); **JPG remote di luar cakupan** |
| Evidence checked | [video asli / frame asli / informasi pengguna / **belum diperiksa**] |
| Duration | [durasi kontainer, dan durasi trek video jika berbeda; hanya nilai terverifikasi] |
| Resolution / FPS | [jika terverifikasi] |
| Aspect ratio | [9:16, 16:9, atau belum pasti] |
| Shot count | [jumlah atau **belum diperiksa**] |
| Audio review | [didengarkan / hanya track terdeteksi / belum diperiksa] |

**Aturan status:** Fase 1 menghasilkan **draft sementara untuk review**, bukan commit atau perubahan `pending`/`draft` di GitHub. Setelah `save now`, tulis status hasil AI `draft` (atau pertahankan status terdahulu jika sesuai bukti dan persetujuan). `approved` hanya setelah persetujuan pengguna yang jelas; `save now` **bukan** persetujuan `approved` atau izin merge.

## 2. Overall Description

**Ringkasan visual (3–5 kalimat):**  
[Deskripsikan apa yang benar-benar terlihat: jenis kebun, ukuran relatif, kerimbunan, buah/sayuran dominan, suasana, dan gaya kamera.]

- **Garden type:** [`open-field` / `front-yard` / `backyard` / `courtyard` / `rooftop` / lainnya / belum pasti]
- **Garden size / space:** [kecil/sedang/luas relatif terhadap isi frame; jangan mengarang ukuran meter]
- **Visual hook awal:** [objek atau suasana yang menarik dalam 1–2 detik pertama]
- **Visual density:** [rendah/sedang/tinggi + alasannya]
- **Overall camera style:** [pan/tracking/handheld/statis/dll., sesuai bukti]
- **Distinctive character:** [maksimal tiga ciri khas]

## 3. Shot Breakdown

**Shot Map (Pass 1, pemeriksaan ulang batas via Pass 2):**

| Shot | Mulai–akhir | Durasi | Transisi | Ketepatan dan bukti waktu | Cakupan |
|---|---|---|---|---|---|
| Shot 01 | [00:00.00–00:05.60] | [5,6s] | [awal/dissolve] | [pasti/perkiraan, alasan] | [diperiksa/belum] |

**Deep Shot Analysis (Pass 2):** setiap shot mencatat observasi MP4 bergerak, perubahan **awal → tengah → akhir**, dan jika gerak kamera ambigu tulis tingkat keyakinan/alternatif.

> **Salin bagian Shot 01 ini untuk tiap shot yang benar-benar terlihat.** Timestamp merujuk pada **video referensi asli**, bukan durasi target generate 8 detik. Pisahkan shot berdasarkan cut; perubahan objek dalam satu gerakan kamera belum tentu cut.

### Shot 01 — [Judul singkat]

- **Timestamp:** [00:00.0–00:00.0; tulis **perkiraan** jika belum presisi]
- **Duration:** [detik / perkiraan]
- **Hero subject:** [subjek dominan]
- **Supporting subjects:** [tanaman/buah/hewan/orang/objek relevan; atau "tidak terlihat"]
- **Visual hook:** [hal paling menarik]
- **Camera movement:** [static / slow pan left/right / tilt / lateral tracking / push-in / pull-back / zoom; jika ragu, jelaskan yang terlihat]
- **Speed and stability:** [lambat/sedang/cepat; handheld halus/stabil, dll.]
- **Camera angle and framing:** [low/eye/high; wide/medium/close-up]
- **Composition:** foreground [..] | middle ground [..] | background [..]
- **Garden layout:** [bedengan, pot, trellis, jalur, rumah, kolam, pagar, posisi relatif]
- **Lighting and colors:** [cahaya dan kontras objek; atau belum pasti]
- **Weather and surfaces:** [mendung/cerah/gerimis; daun, tanah, genangan; atau belum pasti]
- **Action / interaction:** [peristiwa atau gerak yang terlihat; jika tidak ada, "tidak terlihat"]
- **Audio:** [hasil pemeriksaan nyata, atau "audio belum diperiksa"]
- **Transition to next shot:** [hard cut/dissolve/tidak ada/belum pasti]

**Perkembangan gambar dalam shot asli:**
- **Awal:** [objek pertama dalam frame]
- **Tengah:** [apa yang diungkap kamera]
- **Akhir:** [komposisi penutup]

**Bukti & tingkat keyakinan:**  
- [OBSERVASI] [temuan + timestamp]
- [KONTEKS PENGGUNA] [bila ada]
- [INTERPRETASI] [bila ada, jelaskan alasannya]
- [BELUM PASTI] [jika ada]

**Teknik yang bisa dipelajari:** [1–3 hal, misalnya pan lambat memperlihatkan kelompok buah satu per satu]

<!-- Duplikasi bagian Shot 01 untuk Shot 02, Shot 03, dst. sesuai jumlah shot yang diamati. -->

## 4. Plants, Fruits & Garden Layout

| Elemen | Terlihat di bagian mana? | Susunan / ciri visual | Keyakinan |
|---|---|---|---|
| Tanaman sayur | [shot/timestamp] | [jenis, posisi, warna, kerimbunan] | [tinggi/sedang/rendah] |
| Pohon buah | [shot/timestamp] | [jenis bila jelas, letak buah, skala] | [...] |
| Bedengan / pot | [shot/timestamp] | [material dan pola] | [...] |
| Jalur / trellis / struktur | [shot/timestamp] | [hubungan dengan tanaman] | [...] |
| Kolam / saluran air | [shot/timestamp/tidak terlihat] | [bentuk dan posisi] | [...] |

**Struktur lapisan:** [tanaman rendah → semak/perambat → pohon tinggi; jika memang terlihat]  
**Ciri penataan yang patut dipelajari:** [...]

## 5. Weather, Atmosphere & Lighting

- **Waktu:** [pagi/siang/sore/**belum pasti**; sebut sumber bukti]
- **Cuaca:** [cerah/mendung/setelah hujan/gerimis; bedakan OBSERVASI dan KONTEKS PENGGUNA]
- **Light quality:** [soft diffused / direct sunlight / warm / cool / belum pasti]
- **Wet surfaces:** [daun basah, tanah lembap, genangan: bukti/timestamp atau tidak terlihat]
- **Water source:** [hujan alami / sprinkler / selang / kolam / belum pasti]
- **Atmosphere / mood:** [kesan sejuk, tenang, hangat, dll. sebagai INTERPRETASI]
- **Relevant motion:** [angin, daun, hujan, air/riak; atau tidak terlihat]
- **Evidence notes:** [...]

**Jangan menyamakan semprotan sprinkler dengan gerimis.** Langit mendung saja tidak membuktikan jam pengambilan gambar.

## 6. Animals, Humans & Other Objects

> Jika tidak ada subjek selain tanaman, tulis **"tidak terlihat"**. Jangan menambahkan ayam, bebek, ikan, manusia, alat, atau kolam hanya agar analisis terlihat lengkap.

| Subjek / objek | Jumlah tampak | Shot dan posisi | Aktivitas, arah gerak & interaksi | Peran visual |
|---|---|---|---|---|
| [ayam/bebek/ikan/manusia/keranjang/dll., jika ada] | [...] | [...] | [...] | [utama/pendukung/latar] |

**Realism notes:** [ukuran, gerak, kontak air/tanah, dan kontinuitas yang terlihat; jangan menebak identitas orang]

## 7. Audio, Editing & Pacing

- **Audio checked:** [ya/tidak]
- **Natural sound:** [hujan/air/angin/burung/hewan/langkah/lainnya; atau belum diperiksa]
- **Voice / music:** [jika benar-benar terdeteksi; atau belum diperiksa]
- **Shot rhythm:** [durasi dan tempo pergantian gambar]
- **Transitions:** [cut/transisi berdasarkan bukti]
- **What makes the editing effective:** [INTERPRETASI, dengan alasan]

## 8. Visual Characteristics & Reusable Inspiration

**Karakter visual terpenting (maks. 5):**
1. [...]
2. [...]
3. [...]

**Teknik yang dapat digunakan ulang untuk konsep baru:**
- [kamera/komposisi/layout/atmosfer yang disukai + shot sumber]
- [...]

**Elemen opsional, bukan ciri wajib:** [misalnya kolam, hewan, manusia, tanaman spesifik]  
**Hal yang sebaiknya tidak ditiru:** [kesalahan visual/masalah realisme jika ada]  
**Search tags:** `[garden-type]`, `[weather]`, `[camera-style]` — **hanya tag yang didukung bukti**.

## 9. Notes & Uncertainty

- **Belum bisa diverifikasi:** [...]
- **Asumsi yang harus diuji ulang:** [...]
- **Sumber informasi dari pengguna:** [...]
**Contact Sheet Manifest — satu baris untuk satu JPG contact sheet yang diberikan pada Fase 1:**

| Shot | Nama/path JPG yang dikelola pengguna | Semua timestamp panel (urut) | Panel | Dimensi kanvas / panel | Kategori | Ukuran byte lokal (jika diketahui) |
|---|---|---|---:|---|---|---|
| 01 | `../frames/[creator-01]/shot-01.jpg` | [00:00.20; 00:01.10; 00:02.10; ...] | [6] | [1676×2116 / 540×960; sumber 720×1280] | [`contact-sheet` / `contact-sheet-preview`] | [byte sebenarnya, jika tersedia] |

**Petunjuk:** nama/path JPG ditulis sebagai **lokasi arsip baku**, bukan hyperlink aktif atau bukti file telah tersimpan di GitHub. **Tidak perlu menulis status JPG `pending`**, SHA GitHub, atau hasil verifikasi render remote. AI sudah memberikan JPG individual pada Fase 1; pengguna menyimpannya sendiri melalui repo lokal kapan saja. Satu JPG berisi beberapa panel timestamp (target 3–6 adaptif); tidak perlu ZIP, upload oleh AI, atau menunggu JPG berada di GitHub. Pengecilan panel yang wajar dan terbaca tetap `shot-XX.jpg`, bukan otomatis preview; pakai `shot-XX-preview.jpg` jika kualitas turun di bawah target keterbacaan seperti dijelaskan dalam [aturan utama](../rules/analysis.md). Hapus contoh ini saat digunakan.

**Evidence Cross-Check (akhir Fase 1, sebelum STOP/review):**
- **Shot yang belum terwakili / perubahan visual yang terlewat:** [...]
- **Gerakan kamera/transisi/objek ambigu yang diperiksa ulang pada MP4:** [...]
- **Kualitas contact sheet:** [hasil JPG Fase 1 yang benar-benar dibuat/diperiksa; **keberadaan file JPG di GitHub bukan bagian dari verifikasi Fase 2**]
- **Audio belum diperiksa bila relevan:** [...]

## 10. Quality Checklist

**Gate A — Visual Accuracy:** [Fase 1: belum dijalankan; Fase 2: PASS/PARTIAL/FAIL berdasarkan cakupan MP4, Shot Map, gerak kamera, bukti timestamp dan audio]  
**Gate B — Document & Repository Integrity:** [Fase 1: belum dijalankan; Fase 2: PASS/PARTIAL/FAIL berdasarkan analisis 10 bagian + INDEX + status + commit/HEAD `main` + tautan Markdown aktif; **bukan** upload/keberadaan JPG]  
**Overall Gate:** [Fase 1: belum dijalankan; Fase 2: PASS bila A dan B PASS, FAIL bila salah satu FAIL, selain itu PARTIAL; **JPG belum di-push tidak menurunkan nilai**]  
**Bukti verifikasi:** [tanggal/cakupan visual, commit SHA, HEAD `main`, link dokumen/INDEX, path standar JPG]  
**Kendala terbuka:** [kendala analisis atau dokumen; **bukan jadwal upload JPG pengguna**]


- [ ] Referensi benar-benar diperiksa; bila tidak, keterbatasan tertulis jelas.
- [ ] Jumlah dan waktu shot tidak dikarang.
- [ ] Camera movement, framing, komposisi, layout, cuaca, dan ritme tercatat.
- [ ] Sumber air, manusia/hewan/objek, dan audio dibedakan sesuai bukti.
- [ ] Tag dan kesimpulan didukung timestamp atau sumber yang jelas.
- [ ] Nama MP4 unggahan chat, sumber, serta cakupan pemeriksaan jelas; tidak mengklaim MP4 tersedia di repo.
- [ ] Shot Map Pass 1 dan pemeriksaan MP4 Pass 2 mencakup shot yang relevan.
- [ ] Satu JPG contact sheet per shot sebagai target, dengan timestamp tiap panel berurutan dan dapat dibaca.
- [ ] Contact Sheet Manifest satu baris per shot/JPG, nama/path standar, semua timestamp panel, dimensi dan byte lokal jika ada; **tanpa syarat JPG telah di-push**.
- [ ] **Fase 1:** Evidence Cross-Check selesai; **JPG contact sheet individual diberikan ke pengguna** untuk dikelola lewat repo lokal, hasil siap review; AI berhenti tanpa mengubah GitHub.
- [ ] **Fase 2:** setelah `save now`, simpan **Markdown analisis + INDEX langsung di `main`** dalam commit terkoordinasi; verifikasi HEAD/isi dan Gate A/B. **Tidak perlu mengirim atau memeriksa JPG GitHub**.
- [ ] Status analisis dan INDEX konsisten setelah Fase 2; `save now` bukan otomatis `approved`.
- [ ] **Belum membuat ide atau prompt** jika pengguna hanya meminta analisis.

# Video Concept — [Judul Konsep]

> **TEMPLATE — bukan ide yang sudah disetujui.** Gunakan untuk menyusun konsep **setelah pengguna meminta ide atau memilih sebuah ide**. Ikuti `rules/ideas.md`. Jangan menganggap contoh atau placeholder sebagai temuan video asli.

## 1. Concept Information

| Field | Isi |
|---|---|
| Project ID | `garden-001` atau [ID proyek sebenarnya] |
| Concept title | [judul menarik, spesifik] |
| Concept status | `draft` / `selected` / `ready-for-prompts` |
| Target platform | [Google Veo / Google Flow / lainnya] |
| Final format | [9:16 vertikal secara default; sesuaikan pengguna] |
| Planned shots | [2–3 shot secara default; sesuaikan pengguna] |
| Duration per shot | [8 detik secara default; sesuaikan pengguna] |
| Requested mood / style | [...] |

**Ringkasan satu paragraf:**  
[Jelaskan kebun yang ingin divisualisasikan, daya tarik utamanya, dan kesan saat ditonton.]

## 2. Reference Inspirations

> Pilih referensi yang **benar-benar tersedia**. Jelaskan apakah bukti berasal dari video, analisis yang disetujui, atau keterangan pengguna. Referensi berstatus `draft` tidak boleh disajikan sebagai fakta terverifikasi.

| Reference ID / path | Status analisis | Unsur yang dipelajari | Yang diadaptasi dalam konsep |
|---|---|---|---|
| [contoh: muyon-01 / link bila ada] | [approved/draft/belum tersedia] | [layout/cuaca/kamera/dll.] | [adaptasi orisinal] |

**Apa yang dibuat berbeda dari referensi:** [bukan menyalin urutan semua shot atau komposisi yang identik]

## 3. Garden Design

- **Garden type:** [`open-field` / `front-yard` / `backyard` / `courtyard` / `rooftop` / lainnya]
- **Space & scale:** [kecil/sedang/luas; hubungan dengan rumah dan akses jalan]
- **Overall lushness:** [tingkat kerimbunan dan cara membuatnya masuk akal]
- **Foreground:** [tanaman/tekstur/objek dekat kamera]
- **Middle ground:** [bedengan, tomat, cabai, rambatan, kolam, dll.]
- **Background:** [pohon buah, pagar, dinding rumah, pemandangan lain]
- **Beds, paths & structures:** [jumlah relatif, posisi, bahan, pola kebun]
- **Hero plants / fruits:** [pilih yang benar-benar diperlukan]
- **Supporting plants:** [sesuai ruang dan pola tanam yang masuk akal]

## 4. Atmosphere & Activities

- **Time of day:** [...]
- **Weather:** [...]
- **Lighting & colors:** [...]
- **Soil, leaves & water:** [...]
- **Ambient sound:** [...]
- **Animals / humans / tools (optional):** [jenis, jumlah, posisi dan kegiatan; tulis "tidak ada" jika tidak dipakai]
- **Visual hook:** [apa yang memikat perhatian penonton dalam 1–2 detik pertama]

Jangan memaksa kolam besar, pohon tinggi, dan tanaman berjumlah sangat banyak ke pekarangan sempit. Untuk suasana hujan, air dan cahaya harus konsisten secara fisik.

## 5. Continuity Bible — Identitas Kebun yang Tetap

> **Salin nilai-nilai penting ini ke setiap prompt shot.** Setiap generate berdiri sendiri dan dapat kehilangan kontinuitas bila identitas kebun tidak diulang.

| Elemen yang harus sama antargenerate | Deskripsi konkret |
|---|---|
| Garden location & scale | [...] |
| Beds / paths / trellis / fences | [...] |
| Dominant plants & fruit trees | [...] |
| Weather, time & lighting | [...] |
| Colors / materials / wet surfaces | [...] |
| Overall camera feel | [...] |
| Ambient sound | [...] |
| Human / animal continuity, if any | [...] |

**Boleh berbeda di setiap shot:** tanaman yang difokuskan, komposisi, sudut pandang, dan satu gerakan kamera utama.

## 6. Shot Plan

> Default **2–3 shot independen, sekitar 8 detik per shot**. Tabel ini merupakan rencana editing, **bukan** tiga cut di dalam satu prompt. Jika pengguna meminta durasi lain, sesuaikan.

| Shot | Durasi target | Hero subject | Visual hook / composition | Camera movement | Hubungan dengan shot lain |
|---|---|---|---|---|---|
| Shot 01 | [8 s] | [...] | [...] | [slow pan/tracking/dll.] | [pembuka, lokasi konsisten] |
| Shot 02 | [8 s] | [...] | [...] | [...] | [bagian kebun lain] |
| Shot 03 (opsional) | [8 s] | [...] | [...] | [...] | [penutup] |

### Shot 01 — Deskripsi adegan
[Apa yang ditonjolkan dalam satu shot kontinu dan mengapa kamera memilih gerakan ini.]

### Shot 02 — Deskripsi adegan
[...]

### Shot 03 — Deskripsi adegan (opsional)
[...]

## 7. Quality & Realism Checks

- [ ] Konsep realistis untuk ukuran dan jenis kebun yang dipilih.
- [ ] Buah tumbuh pada tanaman yang benar; kepadatan tidak tampak palsu.
- [ ] Cuaca dan unsur air relevan serta tidak menutupi fokus kebun.
- [ ] Kamera memperlihatkan tanaman menarik, bukan selalu berjalan maju.
- [ ] Manusia/hewan/alat, bila ada, memiliki aksi dan posisi jelas.
- [ ] Tiap shot berbeda namun kebun, cahaya, dan struktur tetap terasa satu lokasi.
- [ ] Unsur inspirasi memiliki referensi yang dapat ditelusuri.
- [ ] **Belum menulis prompt final** kecuali pengguna telah memintanya.

## 8. Next Step (hanya bila diminta)

Buat **satu file prompt untuk setiap shot** di `projects/<project-id>/prompts/shot-01.md`, `shot-02.md`, dan seterusnya, mengikuti `templates/video-prompt.md`.

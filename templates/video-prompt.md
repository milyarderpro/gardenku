# Video Prompt — [Project ID] / Shot [01]

> **TEMPLATE — belum siap dipakai sebelum placeholder diisi.** Ikuti `rules/prompts.md` dan konsep yang telah dipilih. **Satu file ini berisi SATU prompt untuk SATU continuous shot**, bukan beberapa shot dengan cut.

## 1. Shot Information

| Field | Isi |
|---|---|
| Project | `[garden-001]` |
| Source concept | `../concept.md` (periksa lokasi aktual) |
| Shot ID | `shot-01` |
| Shot purpose | [hook / eksplorasi / penutup] |
| Target generator | [Google Veo / Google Flow] |
| Input mode | [text-to-video / image-to-video] |
| Reference image (jika ada) | [path atau "tidak ada"] |
| Aspect ratio | [9:16 secara default] |
| Duration | [8 detik secara default] |
| Hero subject | [objek utama] |
| Main camera movement | [pilih satu gerakan utama] |

## 2. Continuity — Harus Sama dengan Shot Lain

> Isikan ulang dari bagian `Continuity Bible` pada `concept.md`. **Jangan menulis "sama seperti shot sebelumnya" di dalam prompt siap salin** karena proses generate berdiri sendiri.

- **Garden location & scale:** [...]
- **Beds, paths, fences, trellis / pond (jika ada):** [...]
- **Plants, fruit trees & planting density:** [...]
- **Weather, time & lighting:** [...]
- **Materials, colors & wet surfaces:** [...]
- **Camera look & ambient sound:** [...]
- **Humans / animals (jika dipakai pada shot ini):** [...]

## 3. Ready-to-Copy Prompt — Google Veo / Flow

> Isi semua tanda `[...]`, lalu salin **hanya teks prompt di bawah** ke generator. Jangan menambahkan bagian yang tidak relevan. Gunakan bahasa Indonesia dengan istilah teknis Inggris bila lebih jelas.

```text
Buat video fotorealistik berdurasi [8] detik, format [vertikal 9:16], tampak seperti rekaman nyata dari kamera [smartphone/handheld stabil sesuai konsep], tanpa teks atau watermark.

LOKASI DAN DESAIN KEBUN:
[Uraikan kebun secara lengkap dan mandiri: jenis serta luas relatif kebun, bedengan, jalur, pagar/rumah, trellis, kolam bila ada, lapisan tanaman dari depan hingga belakang. Gunakan Continuity Bible yang sama untuk semua shot.]

SUBJEK UTAMA DAN KOMPOSISI:
[Hero subject di shot ini, warna/ukuran buah yang wajar dan posisi tanamannya.]
Foreground: [...]
Middle ground: [...]
Background: [...]
[Jika ada manusia, ayam, bebek, ikan atau alat, sebut jumlah, posisi, aksi serta interaksi secara jelas; jika tidak relevan, hilangkan.]

SUASANA, CUACA, DAN CAHAYA:
[Waktu yang diinginkan, kondisi langit, kualitas cahaya, permukaan daun/tanah, hujan atau gerimis jika sesuai konsep. Air, refleksi dan riak bergerak alami.]

KAMERA:
Gunakan [satu gerakan kamera utama, misalnya slow pan right], dengan framing [wide/medium/close-up] dari sudut [..] dan kecepatan [..]. Kamera berfokus pada [..] dan mengungkap bagian kebun yang menarik secara bertahap. Gerak stabil, alami, tanpa cut.

TIMELINE SATU SHOT KONTINU:
0–2 detik: [visual hook langsung terlihat; posisi awal kamera dan objek.]
2–6 detik: [gerakan kamera kontinu mengungkap subjek berikutnya pada ruang yang sama.]
6–8 detik: [akhiri pada komposisi yang indah tanpa perpindahan lokasi atau cut.]

GERAK ALAMI DAN AUDIO:
[Gerak daun, angin, tetesan hujan/air, aktivitas hewan/manusia bila ada. Suara kebun yang sesuai jika generator mendukung audio; tidak ada narasi/musik kecuali diminta.]

BATASAN REALISME:
Tata letak kebun konsisten sepanjang shot. Tanaman tetap tumbuh dari tanah/pot dan buah tetap melekat pada batang yang benar. Tidak ada buah melayang, objek berubah bentuk atau muncul tiba-tiba, gerakan manusia/hewan yang tidak masuk akal, pencahayaan berganti mendadak, kamera meloncat, transisi, atau tampilan CGI.
```

**Jika image-to-video:** cocokkan posisi tanaman, bentuk buah, komposisi awal, dan struktur kebun dengan gambar input. Jangan meminta kamera memperlihatkan perubahan yang bertentangan dengan gambar awal.

**Jika target durasi bukan 8 detik:** ubah durasi **dan seluruh rentang timeline secara konsisten**; jangan membiarkan angka 0–8 detik untuk klip yang lebih pendek/panjang.

## 4. Pre-Generation Checklist

- [ ] Prompt ini **mandiri**; tidak menyebut "lanjutan shot sebelumnya" tanpa deskripsi ulang kebun.
- [ ] Satu shot kontinu; timeline bukan tiga cut atau tiga scene.
- [ ] Durasi, aspect ratio dan input mode sesuai permintaan pengguna/platform.
- [ ] Kamera utama jelas, stabil, dan relevan terhadap hero subject.
- [ ] Foreground, middle ground, background dan tata kebun sesuai konsep.
- [ ] Cahaya, cuaca, bahan struktur, dan posisi objek selaras dengan shot lain.
- [ ] Hewan/manusia/air dan audio hanya muncul bila diinginkan.
- [ ] Realisme fisik tanaman, buah, hewan/manusia, dan air dijaga.
- [ ] Tidak menjanjikan pengaturan generator yang mungkin tidak tersedia.

## 5. Notes (opsional, bukan bagian prompt siap salin)

- **Shot sebelum/sesudahnya:** [urutan editing; hard cut/transisi sederhana]
- **Reference frame:** [file jika benar-benar tersedia; atau tidak ada]
- **Hasil generate / masalah untuk dievaluasi:** [isi setelah dicoba, bukan sebelum]

# References — Pustaka Video Asli

Seluruh referensi dikelompokkan **berdasarkan kreator atau sumber** (`muyon/`, `creator-x/`, dan seterusnya). **Jangan membuat subfolder untuk cuaca atau jenis kebun:** keduanya adalah metadata analisis, karena satu sumber dapat memuat konsep kebun berbeda.

Lihat [`INDEX.md`](INDEX.md) untuk mencari koleksi dan status semua video.

## Menambahkan satu video baru

1. Tentukan nama folder kreator **lowercase-kebab-case** dan ID video yang tidak bentrok (contoh `creator-x-01`).
2. Jika menyimpan video baru, gunakan `<creator>/videos/<id>.mp4`; bila MP4 sudah tersedia, jangan mengunggah duplikat. Video yang dikirim lewat chat dapat menjadi sumber analisis jika isi MP4 repo tidak dapat diunduh. Cocokkan SHA Git blob/ukuran bila memungkinkan dan jangan mengubah MP4 asli tanpa izin.
3. Buat `<creator>/analysis/<id>.md` dengan status `pending`, menggunakan [template analisis](../templates/video-analysis.md) saat benar-benar dianalisis.
4. Tempatkan hanya **JPG yang diekstrak dari video asli** di `<creator>/frames/<id>/`, jika ada. Default 2–3 frame yang mewakili shot penting, resolusi sumber diutamakan; yang diperkecil harus memakai akhiran `-preview.jpg`. Catat daftar dan bukti verifikasi unggah dalam analisis. Detail teknis ada di [aturan analisis](../rules/analysis.md).
5. Tambahkan entri pada [katalog utama](INDEX.md), cek tautan, status, dan informasi sumber video/izin penggunaan yang diketahui.

**Status & hasil terbaru:** lihat [INDEX](INDEX.md) untuk status masing-masing video dan berkas analisisnya untuk frame/timestamp. Hindari menyalin angka status dan frame ke README. Penyimpanan di Facebook atau GitHub **tidak otomatis membuktikan hak distribusi**.

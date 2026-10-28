# References — Pustaka Video Asli

Seluruh referensi dikelompokkan **berdasarkan kreator atau sumber** (`muyon/`, `creator-x/`, dan seterusnya). **Jangan membuat subfolder untuk cuaca atau jenis kebun:** keduanya adalah metadata analisis, karena satu sumber dapat memuat konsep kebun berbeda.

Lihat [`INDEX.md`](INDEX.md) untuk mencari koleksi dan status semua video.

## Menambahkan satu video baru

1. Tentukan nama folder kreator **lowercase-kebab-case** dan ID video yang tidak bentrok (contoh `creator-x-01`).
2. Simpan video aslinya sebagai `<creator>/videos/<id>.mp4`. Jangan mengubah isi MP4 tanpa instruksi pemilik repo.
3. Buat `<creator>/analysis/<id>.md` dengan status `pending`, menggunakan [template analisis](../templates/video-analysis.md) saat benar-benar dianalisis.
4. Tempatkan hanya **frame JPG hasil ekstraksi asli** di `<creator>/frames/<id>/`, jika ada. Jangan menaruh storyboard AI sebagai frame referensi.
5. Tambahkan entri pada [katalog utama](INDEX.md), cek tautan, status, dan informasi sumber video/izin penggunaan yang diketahui.

**Status sekarang:** folder `muyon/` berisi 16 MP4; **`muyon-01` berstatus `draft`, 15 referensi lainnya `pending`**. [Satu JPG preview Muyon 01](muyon/frames/muyon-01/shot-03_15.9s-preview.jpg) sudah tersedia; frame lainnya belum diunggah. Penyimpanan video di Facebook atau GitHub **tidak otomatis membuktikan hak distribusi**.

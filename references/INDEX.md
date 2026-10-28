# Reference Index — Gardenku

**Katalog utama seluruh referensi.** Tiap sumber memakai **ID unik** seperti `muyon-01`, berpasangan dengan `muyon/analysis/muyon-01.md` dan (jika ada) JPG di `muyon/frames/muyon-01/`. **MP4 asli diterima lewat chat, disimpan pengguna di PC, dan tidak diunggah ke repository.**

**Status terkini:** lihat kolom **Status**. `draft` = observasi AI belum disetujui pengguna; `pending` = belum dianalisis. Kolom **Sumber MP4** mencatat apakah unggahan chat sudah pernah diperiksa, **bukan tautan ke file yang tersimpan permanen**. Dalam sesi baru, MP4 asli mungkin perlu diunggah ulang. Jumlah status tidak disalin ke README lain.

## Muyon — 16 referensi video (MP4 tidak disimpan di repo)

[Informasi koleksi Muyon](muyon/README.md)

| Referensi | Sumber MP4 untuk analisis | Jenis kebun | Cuaca | Kamera | Status |
|---|---|---|---|---|---|
| [`muyon-01`](muyon/analysis/muyon-01.md) | Unggahan chat (diperiksa 2026-10-28) | `open-field` (campuran sayur–buah) | Mendung, tanah basah; sprinkler terlihat; gerimis belum pasti | Slow pan / gerak lateral (interpretasi) | `draft` |
| [`muyon-02`](muyon/analysis/muyon-02.md) | Unggahan chat (diperiksa 2026-10-28) | `open-field` (campuran sayur–buah, kolam) | Cahaya terang lembut; hujan belum pasti | Slow pan / pergeseran kanan (interpretasi) | `draft` |
| [`muyon-03`](muyon/analysis/muyon-03.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-04`](muyon/analysis/muyon-04.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-05`](muyon/analysis/muyon-05.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-06`](muyon/analysis/muyon-06.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-07`](muyon/analysis/muyon-07.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-08`](muyon/analysis/muyon-08.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-09`](muyon/analysis/muyon-09.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-10`](muyon/analysis/muyon-10.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-11`](muyon/analysis/muyon-11.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-12`](muyon/analysis/muyon-12.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-13`](muyon/analysis/muyon-13.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-14`](muyon/analysis/muyon-14.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-15`](muyon/analysis/muyon-15.md) | Belum dikirim lewat chat | — | — | — | `pending` |
| [`muyon-16`](muyon/analysis/muyon-16.md) | Belum dikirim lewat chat | — | — | — | `pending` |

**Arti `—`:** belum dianalisis; bukan berarti objek/cuaca/gerak kamera tersebut tidak ada.

## Cara mencari dan memperbarui katalog

1. Cari berdasarkan **kreator**, **jenis kebun**, **cuaca**, atau **kamera** yang sudah dicatat berdasarkan analisis.
2. Klik ID untuk membuka analisis. **Hanya gunakan kesimpulan visual yang memiliki bukti/timestamp**, bukan deskripsi yang ditebak dari nama file.
3. Ketika analisis selesai atau direvisi, perbarui baris terkait **pada commit yang sama**: jenis kebun, cuaca, camera movement, dan status sesuai [`rules/analysis.md`](../rules/analysis.md). **Shot Map dan Contact Sheet Manifest tetap di file analisis**, bukan diduplikasi ke tabel.
4. Bila suatu detail sudah diperiksa tetapi tidak jelas, tulis **`belum pasti`**; jika belum diperiksa, tetap **`—`**.
5. Ketika ada kreator baru, tambahkan bagian dan tabel sejenis. Jangan mengganti ID atau membuat baris ganda. Pastikan tautan `analysis/` dan frame yang **benar-benar tersedia** valid. MP4 **tidak** boleh ditautkan ke GitHub.
6. Utamakan `approved` untuk menyusun [Style Library](../styles/README.md). `draft` perlu ditandai sebagai belum diverifikasi, sedangkan `pending` tidak boleh menjadi dasar kesimpulan visual.

**Status analisis:** `pending`, `draft`, `reviewed`, atau `approved`. Definisi, syarat perubahan, dan verifikasi terdapat di [aturan analisis](../rules/analysis.md). Status INDEX harus sama dengan berkas analisis terkait.

**Asal-usul:** `muyon` adalah label koleksi, belum merupakan verifikasi identitas kreator. URL Facebook asli dan hak penggunaan belum diketahui. Repository bersifat **publik**; verifikasi hak sebelum mendistribusikan video.

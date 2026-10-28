# References — Pustaka Analisis dan Frame

Folder ini menyimpan **pengetahuan hasil analisis** video referensi kebun, bukan file MP4. Video asli dikirim pengguna melalui chat untuk dianalisis dan **disimpan secara pribadi di PC pengguna**. GitHub menyimpan catatan Markdown dan JPG hasil ekstraksi yang terverifikasi.

Cari referensi, status, dan metadata ringkas di [INDEX](INDEX.md). Hasil dan Frame Manifest setiap video menjadi sumber rincian utama; README tidak mengulang angka status yang cepat berubah.

## Menambahkan atau menganalisis referensi

1. Tentukan folder koleksi berdasarkan sumber/kreator (misalnya `muyon/`) dan ID unik lowercase-kebab-case (misalnya `muyon-17`). Jangan membuat subfolder per cuaca atau jenis kebun.
2. Untuk referensi yang belum dikirim, buat `<creator>/analysis/<id>.md` berstatus `pending` dan masukkan ke [INDEX](INDEX.md) dengan sumber `Belum diterima di chat`.
3. Ketika pengguna **mengunggah MP4 di chat**, periksa video yang benar-benar dapat diakses. Simpan nama input/ukuran/hash **jika tersedia** di analisis; **jangan mengunggah MP4 ke GitHub** dan jangan membuat tautan repo untuk MP4 yang tidak ada.
4. Analisis mengikuti [rules/analysis.md](../rules/analysis.md) dan [template](../templates/video-analysis.md). Pisahkan observasi, konteks pengguna, interpretasi, serta ketidakpastian.
5. Pilih **2–3 frame JPG representatif secara default**, atau sesuaikan jumlah dengan shot/bukti; utamakan resolusi sumber. Unggah hanya frame **yang benar-benar diekstrak**, di `<creator>/frames/<id>/`. Gambar diperkecil wajib diberi akhiran `-preview.jpg`.
6. Simpan analisis dengan **Frame Manifest** dan perbarui baris INDEX secara konsisten. Jalankan **Verification Gate**: validasi SHA/byte/path, tautan, status, cakupan analisis, dan kondisi gagal/parsial sebelum mengklaim selesai.

**Jangan menyimpan storyboard AI atau gambar hasil pencarian sebagai frame referensi.** Repositori publik bukan bukti izin mendistribusikan JPG atau video. Penghapusan MP4 dari tree Git terbaru **tidak membersihkan riwayat Git lama**.

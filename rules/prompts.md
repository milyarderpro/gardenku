# Aturan Pembuatan Prompt Video — Gardenku
**Versi:** 1.0  
**Target utama:** Google Veo / Google Flow (image-to-video maupun text-to-video sesuai permintaan).  
**Tujuan:** Membuat prompt yang jelas, visual, realistis, dan konsisten dengan konsep pilihan pengguna serta pembelajaran dari referensi.

> Ini adalah **aturan kerja**. Format penulisan baku akan tersedia di `templates/video-prompt.md` pada Tahap 3. Arsip lama `prompt/mp-v01.md` bukan acuan utama untuk tugas baru bila ketentuannya bertentangan dengan dokumen ini.

## 1. Kapan membuat prompt?
Buat prompt **hanya** jika pengguna sudah meminta prompt atau memilih ide untuk dikembangkan. Jika pengguna hanya meminta analisis atau daftar ide, selesaikan tugas itu terlebih dahulu.

Sebelum menulis:
1. Baca ide/konsep yang dipilih dan `rules/ideas.md` bila pengembangan konsep masih dibutuhkan.
2. Baca analisis referensi dan style profile yang relevan jika tersedia; jangan mengklaim akses video yang tidak ada.
3. Tetapkan jenis/ukuran kebun, tanaman utama, penataan, cuaca, waktu, kamera, dan elemen opsional.
4. Jika pengguna memberi gambar awal/storyboard, jadikan gambar tersebut **acuan visual yang harus dipertahankan**, bukan izin untuk mengganti isi gambar secara bebas.

## 2. Format dasar video
**Default Gardenku**, kecuali pengguna menentukan lain:
- **Aspect ratio:** vertikal `9:16`.
- **Durasi:** **8 detik per generate / 1 continuous shot**.
- **Jumlah:** lazimnya **2–3 shot independen**, disatukan menjadi video akhir lewat editing.
- **Visual:** fotorealistik, seperti rekaman kamera/HP yang nyata, warna alami, tekstur tanaman dan air meyakinkan.
- **Audio:** suara lingkungan alami jika mode generator mendukungnya; tidak perlu narasi atau musik kecuali diminta.
- **Bahasa prompt:** **bahasa Indonesia**, kecuali istilah teknis Inggris yang lebih tepat.

Bila pengguna meminta durasi atau jumlah shot berbeda, **ikuti pengguna**. Jangan menjanjikan bahwa semua pilihan kamera/resolusi/frame rate dapat diatur di semua antarmuka Veo/Flow.

## 3. Satu prompt = satu shot utuh
Setiap prompt **harus bisa digunakan sendiri**, tanpa bergantung pada prompt shot sebelumnya.

Setiap prompt menjelaskan:
1. **Lokasi dan desain kebun:** open-field/front-yard/backyard/rooftop, bedengan, jalan, trellis, rumah/pagar, kolam bila relevan.
2. **Hero subject:** 1 kelompok tanaman/objek paling menarik, misalnya tomat merah di antara daun atau pare tergantung dari trellis bambu.
3. **Lapisan komposisi:** foreground, middle ground, background dan kedalaman yang jelas.
4. **Cuaca dan cahaya:** misalnya langit mendung setelah hujan, daun basah, genangan wajar, gerimis halus, soft diffused daylight.
5. **Arah kamera:** framing, angle, kecepatan dan **satu gerak utama** yang dipilih sesuai keindahan subjek.
6. **Progresi waktu 0–8 detik:** subjek awal, apa yang terungkap di tengah, komposisi akhir.
7. **Gerakan alami dan audio:** tanaman bergerak ringan, tetes air/riak ikan bila relevan, ambience lingkungan.
8. **Batasan realisme:** mencegah buah cacat, layout berubah, objek muncul mendadak, kamera meloncat atau hasil seperti CGI.

Tulis deskripsi yang cukup rinci untuk menuntun visual, tetapi jangan menumpuk perintah kamera yang saling bertentangan.

## 4. Kamera harus mengikuti subjek, bukan pola maju terus
Pilih gerakan berdasarkan tujuan shot:
- **Slow pan left/right:** menyingkap tanaman berbuah satu demi satu tanpa berpindah tempat jauh.
- **Lateral tracking:** menggeser kamera perlahan sepanjang bedengan atau tepi kolam.
- **Gentle push-in:** mendekati detail buah matang.
- **Slow tilt:** menampilkan sayuran rendah lalu buah pada pohon/trellis lebih tinggi.
- **Static / gentle handheld:** untuk adegan halus seperti rintik hujan, bebek, ikan, atau orang memanen.
- **Forward walkthrough:** hanya bila jalan setapak merupakan bagian penting dari konsep.

Satu shot boleh berisi penyesuaian kecil yang natural, tetapi **hindari cut internal, rotasi ekstrem, zoom tiba-tiba, dan gerak kamera yang tidak mungkin**.

## 5. Timeline mikro 8 detik
Gunakan perkembangan yang masuk akal, sebagai panduan bukan cut:
- **0–2 detik — Hook:** objek paling menarik langsung terlihat.
- **2–6 detik — Reveal:** gerak kamera perlahan membuka lapisan tanaman, buah, atau detail lingkungan.
- **6–8 detik — Ending:** akhir dengan komposisi jelas dan memuaskan.

Seluruh rentang ini adalah **satu continuous shot tanpa pergantian lokasi tiba-tiba**. Jangan mengartikan timeline sebagai tiga scene atau tiga video.

## 6. Konsistensi antargenerate (continuity)
Untuk semua shot dalam satu konsep, tulis ulang **paket identitas kebun** di setiap prompt:
- Jenis/ukuran kebun dan hubungan jalan–bedengan–trellis–rumah/kolam.
- Material dan warna struktur penting.
- Tanaman dominan, tingkat kerimbunan, warna dan suasana.
- Waktu, cuaca, kondisi daun/tanah, arah/kualitas cahaya.
- Tampilan umum kamera dan suara lingkungan.

**Yang boleh berubah per shot:** hero subject, jarak/angle kamera, arah pergerakan, bagian kebun yang ditonjolkan.

Jika ada manusia/hewan yang memang dipertahankan antar-shot, konsistenkan penampilan umum, pakaian, jumlah, skala, dan aktivitas. Jangan tiba-tiba menambahkan hewan/manusia ke shot berikutnya jika tidak sesuai konsep.

Catatan: mengulang deskripsi memperkuat konsistensi tetapi **tidak menjamin** setiap generate identik. Gambar awal, frame keluaran, atau fitur reference image di platform (jika tersedia) bisa membantu.

## 7. Realisme tanaman, cuaca, air, dan makhluk hidup
- Buah terikat pada tanaman yang benar, dengan batang, ukuran, tekstur dan orientasi masuk akal; tidak melayang, menggandakan diri atau berubah bentuk.
- Pekarangan kecil tidak tiba-tiba berubah menjadi perkebunan sangat luas.
- Air mengalir mengikuti kontur, genangan tidak muncul/hilang mendadak, hujan turun konsisten secara fisik, dan sprinkler tidak dianggap gerimis alami.
- Bila kondisi **setelah hujan dan masih gerimis**, tunjukkan petunjuk visual yang halus (daun basah, tanah lembap, rintik ringan), namun tanaman/buah tetap mudah terlihat.
- Ayam/bebek berjalan dan berpijak alami; ikan berenang dalam air dan menghasilkan riak sesuai gerakan; manusia memegang alat atau memetik buah dengan gerakan tubuh/tangan yang masuk akal.
- Jangan berlebihan dengan kabut, tetes air, saturasi hijau, jumlah buah, atau efek suara.

## 8. Cara menulis prompt
Berikan **satu blok prompt siap salin untuk setiap shot**. Untuk tiap blok, cantumkan:
- Judul shot + durasi `8 detik` (atau yang diminta).
- Deskripsi kebun yang lengkap dan tetap konsisten.
- Apa yang terlihat dan apa yang dilakukan subjek.
- Gerakan kamera utama dengan kecepatan yang masuk akal.
- Progresi 0–2 / 2–6 / 6–8 detik.
- Cahaya, cuaca, gerakan alami, audio, dan larangan visual yang relevan.

**Jangan membuat satu prompt berisi tiga perpindahan scene** hanya karena video akhir dirancang memiliki tiga shot. Tiga shot berarti tiga proses generate, lalu digabung dengan editing.

### Contoh singkat struktur (bukan prompt final)
**Shot 01 — Tomat selepas hujan, 8 detik:** kebun pekarangan belakang yang rimbun, bedengan bata dan trellis bambu, tomat merah di depan, pepaya di belakang, daun basah dan gerimis lembut. Kamera slow pan ke kanan melintasi tomat. 0–2 detik fokus tomat, 2–6 detik mengungkap cabai di sisinya, 6–8 detik menutup dengan komposisi bedengan. Suara gerimis halus. **Tidak ada cut, buah berubah bentuk, atau kamera melompat.**

Dalam produksi sesungguhnya, uraikan detail seperlunya sesuai konsep dan gambar referensi yang tersedia.

## 9. Periksa sebelum mengirim
- [ ] Prompt ditulis dalam bahasa Indonesia, aspek rasio dan durasi sesuai permintaan.
- [ ] Tiap generate berisi **satu shot kontinu** dan dapat digunakan mandiri.
- [ ] Kamera, hero subject, komposisi dan timeline tidak saling bertentangan.
- [ ] Layout dan cuaca konsisten antara shot.
- [ ] Manusia, hewan, air, dan audio hanya ada bila memang diminta atau relevan.
- [ ] Gerakan serta pertumbuhan tanaman realistis; tidak ada buah melayang/berubah.
- [ ] Tidak mengklaim pengaturan yang mungkin tidak tersedia pada platform pengguna.

**Sasaran akhir: beberapa shot pendek yang kaya visual, realistis, serta terasa direkam di kebun dan suasana yang sama.**

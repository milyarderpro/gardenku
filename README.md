# Gardenku

**Gardenku** adalah pustaka referensi video kebun untuk AI: mengamati video asli, menyimpan analisis yang dapat ditelusuri, mengembangkan ide baru, dan membuat prompt Google Veo/Flow per shot.

**Bahasa:** nama folder/file teknis memakai bahasa Inggris, isi dokumen dan prompt memakai bahasa Indonesia (istilah teknis kamera boleh berbahasa Inggris).

## Mulai dari sini

| Yang ingin dilakukan | Dokumen yang dibaca |
|---|---|
| Memahami aturan kerja AI | [AGENTS.md](AGENTS.md) |
| Mencari referensi | [references/INDEX.md](references/INDEX.md) |
| Menganalisis video | [Aturan analisis](rules/analysis.md) + [template analisis](templates/video-analysis.md) |
| Membuat ide atau konsep | [Aturan ide](rules/ideas.md) + [template konsep](templates/video-concept.md) |
| Membuat prompt Veo/Flow | [Aturan prompt](rules/prompts.md) + [template prompt](templates/video-prompt.md) |
| Mempelajari gaya visual | [styles/README.md](styles/README.md) |
| Menyimpan produksi dan hasil uji | [projects/README.md](projects/README.md) |

## Struktur folder

```text
gardenku/
├── README.md                 # Pengantar untuk pengguna
├── AGENTS.md                 # Navigasi dan prioritas kerja AI
├── rules/                    # Ketentuan bagaimana pekerjaan dilakukan
├── templates/                # Bentuk dokumen yang dihasilkan
├── references/               # Analisis dan contact sheet JPG menurut sumber; tanpa MP4
│   ├── INDEX.md              # Katalog seluruh kreator
│   └── muyon/
│       ├── README.md
│       ├── analysis/         # hasil per video (Shot Map + Contact Sheet Manifest)
│       └── frames/           # satu JPG contact sheet multi-panel untuk setiap shot
├── styles/                   # Rangkuman gaya berbasis bukti
└── projects/                 # Konsep, prompt, evaluasi, dan arsip
```

Satu kreator dapat memiliki berbagai jenis kebun (open-field, front-yard, backyard, rooftop, dan sebagainya). **Jenis kebun adalah metadata analisis, bukan subfolder tambahan.** ID seperti `muyon-01` menghubungkan video, analisis, dan folder frame.

## Referensi dan status terkini

- **Daftar referensi, metadata ringkas, dan status analisis terbaru:** [references/INDEX.md](references/INDEX.md).
- **Temuan per video, timestamp, dan JPG yang benar-benar tersimpan:** buka berkas dari [references/muyon/analysis/](references/muyon/analysis/); tiap analisis yang sudah dikerjakan memuat **Shot Map** dan **Contact Sheet Manifest** sesuai [template](templates/video-analysis.md).
- **Frame JPG asli hasil ekstraksi:** tersimpan di `references/<creator>/frames/<video-id>/` jika sudah diunggah. Status `draft` bukan berarti sudah disetujui.
- [Master prompt lama](projects/legacy/README.md) diarsipkan agar tidak bertentangan dengan aturan baru.
- URL Facebook asli dan izin penggunaan setiap video belum terverifikasi. **Repository ini publik:** hak untuk membagikan JPG juga perlu diperiksa. Penghapusan MP4 dari branch terbaru **tidak menghapus MP4 dari riwayat Git**; pembersihan riwayat memerlukan tindakan terpisah.

## Opsi B+ v1.3 — Workflow dua fase dengan fallback upload JPG

**Fase 1 — Analyze & Review (tahap 1–5):** unggah MP4 lewat chat → validasi → Shot Map (Pass 1) → Deep Shot Analysis (Pass 2) → **contact sheet JPG lokal per shot** (target 3–6 panel adaptif) → Evidence Cross-Check. AI menampilkan analisis, Shot Map, dan **JPG individual untuk diunduh** saat review; JPG itu pula yang digunakan saat Fase 2. **STOP: tidak ada penyimpanan/perubahan di GitHub selama fase ini.**

**Perintah `save now`:** setelah hasil sesuai, pengguna memberikan izin penyimpanan yang eksplisit. AI menyimpan **versi yang terakhir direvisi**, bukan draft sebelumnya.

**Fase 2 — Save & Verify (tahap 6–7):** AI mencoba mengunggah **JPG yang sudah diberikan pada Fase 1**. Jika pengiriman JPG biner lewat konektor gagal, **AI membuat branch staging dan memberi instruksi folder tujuan; pengguna mengunggah JPG Fase 1 yang sama ke branch tersebut, tanpa ZIP baru**. Setelah semua SHA/path/ukuran cocok, AI menyimpan analisis + `references/INDEX.md`, membuka PR, lalu menjalankan **Gate A Visual Accuracy + Gate B Repository Integrity**. Jika upload belum selesai, pekerjaan tetap `menunggu upload manual`, tidak perlu mengulang Fase 1. **Tidak otomatis merge atau mengubah status ke `approved`.**

MP4 asli tetap di PC pengguna, tidak disimpan di GitHub. Artefak sementara Fase 1 mungkin tidak tersedia jika berpindah percakapan; jangan menganggap file tersimpan permanen. [Aturan lengkap](rules/analysis.md). GitHub menyimpan pengetahuan, **bukan** melatih ulang model AI.

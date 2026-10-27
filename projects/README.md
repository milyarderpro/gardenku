# Projects — Produksi Video Baru

Folder `projects/` menyimpan **hasil karya baru**, bukan video referensi asli. Gunakan satu ID proyek seperti `garden-001` untuk satu konsep yang dipilih.

## Contoh susunan proyek (belum dibuat)

```text
projects/
└── garden-001/
    ├── concept.md          # Desain kebun + Continuity Bible + Shot Plan
    ├── prompts/
    │   ├── shot-01.md      # Satu prompt mandiri ~8 detik
    │   └── shot-02.md
    └── review.md           # Catatan hasil generate dan koreksi
```

**Tidak perlu `shot-plan.md` terpisah** untuk proyek biasa: pembagian shot sudah berada di bagian **Shot Plan** pada `concept.md`. Pisahkan menjadi file sendiri hanya jika proyek yang lebih kompleks benar-benar memerlukannya, dan jangan mempertahankan dua versi rencana berbeda.

- **Konsep:** gunakan [`templates/video-concept.md`](../templates/video-concept.md) setelah ide dipilih.
- **Prompt per shot:** gunakan [`templates/video-prompt.md`](../templates/video-prompt.md); satu file = satu shot tanpa cut.
- **Review:** setelah mencoba generate, catat masalah dan revisi. Jangan menganggap video sudah jadi sebelum ada hasil nyata.
- **Arsip:** [`legacy/`](legacy/README.md) menyimpan master prompt historis; bukan sumber aturan aktif.

Rujuk [`rules/ideas.md`](../rules/ideas.md) dan [`rules/prompts.md`](../rules/prompts.md) untuk ketentuan kreatif.

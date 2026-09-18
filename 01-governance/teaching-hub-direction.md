# Teaching Hub Direction

**Status:** DECISION  
**Recorded:** 2026-09-18

## Purpose

Website/portal untuk proyek `bahasa-inggris-smp` diarahkan terutama sebagai **Teacher Teaching Hub**.

Target pengguna utama adalah **guru/pemilik repo** untuk menyiapkan, mencari, membuka, dan menggunakan materi/bahan ajar saat pembelajaran berlangsung.

Siswa dapat menggunakan materi yang sesuai untuk mereka, tetapi **student-facing website bukan primary design target**.

## Architecture Direction

```text
GitHub repository
      ↓
authoritative Markdown content
      ↓
teaching-site presentation layer
      ↓
Teacher Teaching Hub
      └── selected student-appropriate content
```

GitHub repository tetap menjadi **authoritative source of truth**. Website adalah presentation/navigation layer dan tidak menggantikan governance, history, atau project state di repo.

## Preferred Platform Direction

Current preferred implementation candidate:

**MkDocs Material + GitHub + static deployment (e.g. Cloudflare Pages/GitHub Pages).**

Alasan utama:

- konten Markdown tetap berada di repo;
- Git history tetap menjadi history perubahan;
- navigasi dan search lebih praktis daripada membuka folder GitHub saat mengajar;
- nyaman digunakan dari laptop/HP;
- dapat menyajikan materi sebagai teaching portal, bukan developer documentation;
- deployment dapat dibuat otomatis setelah perubahan di repo.

Ini adalah **platform direction**, bukan deployment yang sudah diimplementasikan/frozen. Implementasi teknis harus diputuskan ketika workstream website dimulai.

## UX Principle

Navigasi utama website harus mengikuti **workflow guru**, bukan menyalin mentah struktur governance repo.

Contoh arah navigasi:

```text
Hari Ini
Materi
  ├── Semester 1
  └── Semester 2
Speaking Activities
Games & Activities
Latihan
Assessment
Progress Kelas
Teacher Reference
  ├── Curriculum Map
  ├── Prerequisite Map
  └── Textbook Reference
```

## Teaching Page Principle

Halaman materi idealnya dapat memuat:

- tujuan pembelajaran;
- alokasi waktu/JP;
- materi inti;
- contoh;
- vocabulary;
- drilling/speaking prompts;
- activity/game;
- latihan;
- teacher notes;
- anticipated/common errors;
- remediasi;
- next instructional step.

Tidak semua bagian harus selalu tampil kepada siswa.

## Teacher vs Student Content

Teacher-facing content dapat memuat instructional notes, timing, strategi, remediasi, dan decision support.

Student-appropriate content dapat digunakan/dibagikan kepada siswa bila sesuai, misalnya:

- materi inti;
- contoh;
- vocabulary;
- latihan;
- speaking practice;
- tugas.

Data baseline/progress siswa, gap analysis internal, governance, dan informasi lain yang tidak semestinya publik **tidak boleh otomatis dipublikasikan hanya karena berada di repo**.

## Boundary

Portal tidak boleh mengubah prinsip proyek:

**CP-aligned · student-level-adjusted · textbook-supported · evidence-driven**

Website membantu delivery dan retrieval bahan ajar. Ia bukan pacing authority dan tidak menggantikan evidence-based instructional decisions.

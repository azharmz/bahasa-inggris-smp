# Bahasa Inggris SMP — Project Control

> **Repository ini adalah ONLY AUTHORITATIVE SOURCE OF TRUTH untuk proyek pembelajaran ini.**
>
> Riwayat chat bukan project state. Setiap sesi baru harus membaca README ini terlebih dahulu, lalu mengikuti tautan ke dokumen authoritative yang relevan. Jika chat/memori bertentangan dengan repo, **repo yang berlaku**.

## 1. Project Purpose

Membangun sistem pembelajaran Bahasa Inggris Kelas VIII SMP yang terstruktur, realistis terhadap kemampuan aktual peserta didik, selaras dengan Capaian Pembelajaran (CP), dan menggunakan buku resmi sebagai sumber utama tanpa menjadikan urutan halaman buku sebagai pacing authority.

Prinsip kerja utama:

**CP-aligned · student-level-adjusted · textbook-supported · evidence-driven**

## 2. Teaching Context — CONFIRMED

- Kelas: VIII SMP
- Semester aktif: Ganjil
- 1 JP: 40 menit
- Total alokasi: 4 JP/pekan
- Intrakurikuler: 3 JP/pekan = 120 menit
- Kokurikuler: 1 JP/pekan = 40 menit
- Buku utama: *English for Nusantara untuk SMP/MTs Kelas VIII*, Kementerian Pendidikan, Kebudayaan, Riset, dan Teknologi, 2022
- Kondisi penting: pembelajaran sebelumnya belum mengikuti buku siswa secara sistematis.
- Baseline kemampuan siswa: **NOT YET FORMALLY ASSESSED**. Jangan menganggap percakapan atau impresi informal sebagai baseline final.

## 3. Authority Hierarchy

Urutan otoritas proyek:

1. CP/ketentuan kurikulum resmi yang berlaku.
2. Evidence kemampuan aktual peserta didik.
3. Keputusan kurikulum/pembelajaran yang telah didokumentasikan di repo.
4. Buku *English for Nusantara VIII* sebagai primary textbook/resource.
5. Materi pendukung lain yang secara eksplisit diterima dan dicatat di repo.

Buku adalah sumber utama pembelajaran, **bukan kewajiban pacing halaman demi halaman**. Foundation/bridge instruction boleh dan perlu diberikan bila prerequisite peserta didik belum memadai.

## 4. Curriculum Architecture

```text
Official CP
    ↓
Competency Map
    ↓
Textbook Audit / Map
    ↓
Prerequisite Map
    ↓
Student Baseline
    ↓
Gap Analysis
    ↓
Semester Scope & Sequence
    ↓
Weekly Teaching Package
    ↓
Assessment / Classroom Evidence
    ↓
Progress Review
    ↓
Next Instructional Decision
```

## 5. Instructional Status Vocabulary

Gunakan status berikut agar posisi pembelajaran jelas:

- `FOUNDATION` — membangun kemampuan dasar yang menjadi prerequisite.
- `BRIDGE` — menghubungkan kemampuan dasar ke target kelas VIII/buku.
- `TEXTBOOK-ALIGNED` — pembelajaran sudah langsung mengerjakan target/unit buku yang dipetakan.
- `ASSESSMENT` — pengumpulan evidence penguasaan/kemajuan.

Status ini bukan label kemampuan siswa secara permanen; ini label fungsi pembelajaran pada suatu tahap.

## 6. Repository Map

```text
README.md                         ← START HERE / project control
01-governance/
  source-of-truth.md              ← aturan otoritas dan update state
  teaching-principles.md          ← prinsip desain pembelajaran
02-sources/
  textbook-audit.md               ← audit authoritative buku utama
  curriculum-sources.md           ← sumber CP/kurikulum resmi
03-baseline/
  class-profile.md                ← konteks kelas yang diketahui
  student-entry-level.md          ← baseline berbasis evidence
  gap-analysis.md                 ← gap prerequisite → target
04-curriculum-map/
  competency-map.md               ← CP → kompetensi operasional
  prerequisite-map.md             ← dependency kemampuan
  semester-1-scope-sequence.md    ← roadmap semester authoritative
05-teaching/
  semester-1/                     ← paket pembelajaran per pekan
06-assessment/
  diagnostic/                     ← asesmen baseline
  formative/                      ← evidence selama proses
  summative/                      ← asesmen akhir/unit bila diperlukan
07-cocurricular/
  semester-1.md                   ← jalur 1 JP kokurikuler
08-progress/
  teaching-log.md                 ← apa yang benar-benar diajarkan
  student-progress.md             ← evidence kemajuan/agregat kelas
```

Direktori/file dibuat bertahap saat memang dibutuhkan. Struktur di atas adalah contract organisasi, bukan alasan membuat dokumen kosong.

## 7. Authoritative Textbook — CONFIRMED

**English for Nusantara untuk SMP/MTs Kelas VIII**  
Kementerian Pendidikan, Kebudayaan, Riset, dan Teknologi Republik Indonesia, 2022.  
ISBN jilid 2: `978-602-427-941-7`.

Struktur utama buku:

- Chapter 0 — *The Beginning*
- Chapter 1 — *Celebrating Independence Day*
- Chapter 2 — *Kindness Begins with Me*
- Progress Check 1
- Chapter 3 — *Love Our World*
- Chapter 4 — *No Littering*
- Chapter 5 — *Embrace Yourself*
- Progress Check 2

Buku menggunakan pendekatan berbasis genre dan mengintegrasikan listening, speaking, reading, viewing, writing, dan representing. Audit detail buku **belum selesai** dan tidak boleh dianggap selesai hanya berdasarkan daftar isi/scope-and-sequence awal.

## 8. Non-Negotiable Teaching Principles

1. **Jangan mengejar halaman buku demi mengejar ketertinggalan.**
2. CP menentukan arah; kemampuan aktual siswa menentukan titik mulai.
3. Jangan mengajarkan target kompleks sebelum prerequisite kritis tersedia.
4. Sederhanakan input/tugas bila perlu tanpa kehilangan arah kompetensi.
5. Grammar/vocabulary adalah alat untuk fungsi komunikasi, bukan satu-satunya tujuan kurikulum.
6. 3 JP intrakurikuler dan 1 JP kokurikuler direncanakan sebagai jalur berbeda tetapi saling mendukung.
7. Keputusan maju/remediasi harus semakin berbasis evidence kelas, bukan semata estimasi.
8. Jangan mengarang baseline, mastery, atau teaching history yang belum tercatat/evidenced.

## 9. CURRENT STATE

**Phase: P0 — REPOSITORY BOOTSTRAP / SOURCE AUDIT**

Confirmed:

- [x] Repo ditetapkan sebagai only authoritative source of truth.
- [x] Teaching context dasar ditetapkan.
- [x] Buku utama kelas VIII teridentifikasi dan tersedia untuk audit.
- [x] Arsitektur proyek ditetapkan.

Not yet completed:

- [ ] Ambil dan verifikasi CP Bahasa Inggris Fase D dari sumber resmi yang berlaku.
- [ ] Audit buku *English for Nusantara VIII* secara sistematis.
- [ ] Bangun competency map.
- [ ] Bangun prerequisite map.
- [ ] Rancang diagnostic baseline yang ringan dan feasible.
- [ ] Tetapkan baseline siswa dari evidence.
- [ ] Gap analysis.
- [ ] Susun Semester 1 Scope & Sequence.
- [ ] Susun jalur kokurikuler.
- [ ] Bangun weekly teaching packages.

**Penting:** semester scope & sequence belum boleh dianggap final sebelum source audit + prerequisite analysis + baseline/gap analysis cukup memadai.

## 10. NEXT ACTION

**P1 — Authoritative Source Audit**

1. Verifikasi CP Bahasa Inggris Fase D yang berlaku dari sumber pemerintah.
2. Audit *English for Nusantara VIII*: per chapter/unit petakan communicative function, language features, skills, output/task, dan prerequisite.
3. Simpan hasil ke `02-sources/`.
4. Dari evidence tersebut mulai `competency-map.md` dan `prerequisite-map.md`.

Setelah P1, rancang diagnostic baseline. Jangan langsung membuat kalender semester final.

## 11. Rules for Every Future ChatGPT Session

Saat diminta mengerjakan proyek ini:

1. Baca `README.md` terlebih dahulu.
2. Anggap repo sebagai project truth; jangan merekonstruksi state dari chat lama.
3. Buka hanya dokumen authoritative yang diperlukan dari Repository Map/CURRENT STATE/NEXT ACTION.
4. Bedakan dengan jelas `CONFIRMED`, `EVIDENCE`, `INFERENCE`, `TBD`, dan keputusan desain.
5. Jangan mengisi fakta yang tidak diketahui dengan asumsi.
6. Kerjakan `NEXT ACTION` kecuali user secara eksplisit mengubah prioritas.
7. Setelah perubahan bermakna, update dokumen terkait dan `CURRENT STATE`/`NEXT ACTION` di README.
8. Pekerjaan yang mengubah project state belum dianggap selesai jika README menjadi stale.

### Minimal prompt untuk chat baru

> **Cek repo `azharmz/bahasa-inggris-smp` dan lanjutkan.**

Prompt tersebut harus cukup untuk memulihkan state proyek tanpa handoff manual.

## 12. Change Discipline

Git history adalah decision/history trail. Jangan menghapus histori ketidakpastian dengan menulis ulang seolah keputusan sudah diketahui sejak awal. Bila evidence baru mengubah rencana, dokumentasikan perubahan dan alasannya.

---

**Last project-state update:** 2026-09-15  
**Current next action:** P1 — Authoritative Source Audit

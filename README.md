# Bahasa Inggris SMP — Project Control

> **Repository ini adalah ONLY AUTHORITATIVE SOURCE OF TRUTH untuk proyek pembelajaran ini.**
>
> Riwayat chat bukan project state. Setiap sesi baru harus membaca README ini terlebih dahulu, lalu mengikuti dokumen authoritative yang relevan. Jika chat/memori bertentangan dengan repo, **repo yang berlaku**.

## 1. Project Purpose

Membangun sistem pembelajaran Bahasa Inggris SMP yang terstruktur, realistis terhadap kemampuan aktual peserta didik, selaras dengan Capaian Pembelajaran (CP), dan menggunakan buku resmi sebagai sumber utama tanpa menjadikan urutan halaman buku sebagai pacing authority.

**Current active implementation:** Kelas VIII SMP.  
**Current implementation cycle:** Semester Ganjil / Semester 1.

Repo tidak dibatasi hanya untuk Semester 1. Semester berikutnya melanjutkan evidence dan state pembelajaran semester sebelumnya.

Prinsip utama:

**CP-aligned · student-level-adjusted · textbook-supported · evidence-driven**

## 2. Teaching Context — CONFIRMED

- Current active grade: VIII SMP
- Current semester: Ganjil / Semester 1
- 1 JP: 40 menit
- Total: 4 JP/pekan
- Intrakurikuler: 3 JP/pekan = 120 menit
- Kokurikuler: 1 JP/pekan = 40 menit
- Buku utama: *English for Nusantara untuk SMP/MTs Kelas VIII* (2022)
- Pembelajaran sebelumnya belum mengikuti buku siswa secara sistematis.
- Baseline kemampuan siswa: **NOT YET FORMALLY ASSESSED**.

Semester adalah timebox. End-state evidence Semester 1 menjadi entry state Semester 2.

## 3. Authority Hierarchy

1. CP/ketentuan kurikulum resmi yang berlaku.
2. Evidence kemampuan aktual peserta didik.
3. Keputusan yang telah didokumentasikan di repo.
4. *English for Nusantara VIII* sebagai primary textbook/resource.
5. Supporting sources yang diterima dan dicatat di repo.

Buku adalah sumber utama, **bukan pacing authority halaman demi halaman**.

## 4. Curriculum Architecture

```text
Official CP / Phase Target
    ↓
Grade-level Competency Map
    ↓
Textbook Audit / Map
    ↓
Prerequisite Map
    ↓
Diagnostic Evidence
    ↓
Student Baseline + Gap Analysis
    ↓
Semester Scope & Sequence
    ↓
Weekly Teaching Package
    ↓
Assessment / Classroom Evidence
    ↓
Progress Review → Next Instructional Decision
```

## 5. Instructional Status Vocabulary

- `FOUNDATION` — membangun prerequisite dasar.
- `BRIDGE` — menghubungkan kemampuan dasar ke target kelas VIII/buku.
- `TEXTBOOK-ALIGNED` — langsung mengerjakan target/unit buku yang dipetakan.
- `ASSESSMENT` — pengumpulan evidence.

## 6. Repository Map

```text
README.md
01-governance/
  source-of-truth.md
  teaching-principles.md
02-sources/
  curriculum-sources.md
  textbook-audit.md
03-baseline/
  class-profile.md
  student-entry-level.md          ← AFTER diagnostic administration
  gap-analysis.md                 ← AFTER diagnostic evidence
04-curriculum-map/
  competency-map.md
  prerequisite-map.md
  semester-1-scope-sequence.md    ← AFTER baseline/gap analysis
  semester-2-scope-sequence.md    ← later
05-teaching/
  semester-1/
  semester-2/
06-assessment/
  diagnostic/
    baseline-diagnostic.md        ← READY TO ADMINISTER
  formative/
  summative/
07-cocurricular/
  semester-1.md
  semester-2.md
08-progress/
  teaching-log.md
  student-progress.md
```

Direktori/file dibuat bertahap saat dibutuhkan.

## 7. Authoritative Sources — CURRENT

### Curriculum

2025 *Panduan Mata Pelajaran Bahasa Inggris: Fase B–F dan Fase F Tingkat Lanjut*, Pusat Kurikulum dan Pembelajaran / BSKAP, Kemendikdasmen. Phase D end target approximately CEFR A2. Detail: `02-sources/curriculum-sources.md`.

### Textbook

*English for Nusantara untuk SMP/MTs Kelas VIII* (2022), ISBN `978-602-427-941-7`. Detail: `02-sources/textbook-audit.md`.

## 8. Non-Negotiable Teaching Principles

1. Jangan mengejar halaman buku demi ketertinggalan.
2. CP menentukan arah; kemampuan aktual siswa menentukan titik mulai.
3. Jangan memaksakan target kompleks sebelum prerequisite kritis tersedia.
4. Sederhanakan input/tugas tanpa kehilangan arah kompetensi.
5. Grammar/vocabulary adalah alat komunikasi, bukan satu-satunya tujuan.
6. Intrakurikuler dan kokurikuler adalah jalur berbeda tetapi saling mendukung.
7. Keputusan maju/remediasi berbasis evidence kelas.
8. Jangan mengarang baseline, mastery, atau teaching history.
9. Pergantian semester tidak mereset learning state.

## 9. CURRENT STATE

**Active scope: Grade VIII — Semester 1**  
**Phase: P3 — DIAGNOSTIC ADMINISTRATION / EVIDENCE WAIT**

### P0 — Repository Bootstrap
- [x] Repo = only authoritative source of truth.
- [x] Teaching context recorded.
- [x] Semester-continuous architecture established.

### P1 — Authoritative Source Audit
- [x] Official Phase D curriculum source verified/documented.
- [x] Phase D element targets documented.
- [x] Textbook identity/approach/chapter scope mapped.
- [x] Actual textbook task demands sampled.
- [x] Competency map v0.1.
- [x] Prerequisite map v0.1 + gates G0–G6.

Non-blocking open detail:
- [ ] resolve Chapter 1 Unit 3 front-matter discrepancy when needed in detailed planning.

### P2 — Diagnostic Baseline Design
- [x] Compact 40-minute diagnostic designed.
- [x] G0–G6 mapped to observable tasks.
- [x] Teacher observation + student tasks included.
- [x] Gate evidence scale defined: `INDEPENDENT / SUPPORTED / NOT YET`.
- [x] Aggregate recording template included.
- [x] Instrument marked `READY TO ADMINISTER`.

### Not Yet Completed
- [ ] Administer diagnostic / collect classroom evidence.
- [ ] Record `student-entry-level.md`.
- [ ] Gap analysis.
- [ ] Semester 1 Scope & Sequence.
- [ ] Semester 1 cocurricular pathway.
- [ ] Weekly teaching packages.

## 10. CURRENT DIAGNOSTIC

Authoritative instrument:

`06-assessment/diagnostic/baseline-diagnostic.md`

Design:

- fits 1 JP / 40 minutes;
- samples G0–G6;
- is not a conventional 0–100 exam;
- records each gate as `INDEPENDENT`, `SUPPORTED`, or `NOT YET`;
- does not freeze a percentage threshold before first administration;
- preserves oral evidence option for G6 when writing itself blocks output.

## 11. NEXT ACTION

**P3 — Administer diagnostic and return evidence.**

Teacher administers `06-assessment/diagnostic/baseline-diagnostic.md` to the class.

After administration, record at minimum:

- number of students present;
- class/rombel;
- date;
- aggregate counts `INDEPENDENT / SUPPORTED / NOT YET` for G0–G6;
- common errors or notable patterns;
- any unusual condition that may distort evidence.

Then create:

1. `03-baseline/student-entry-level.md`;
2. `03-baseline/gap-analysis.md`;
3. initial Semester 1 Scope & Sequence.

**Hard boundary:** do not claim a class baseline and do not freeze Semester 1 Scope & Sequence before diagnostic evidence exists.

## 12. Rules for Every Future ChatGPT Session

1. Read `README.md` first.
2. Repo is project truth; do not reconstruct state from old chats.
3. Follow CURRENT STATE and NEXT ACTION unless user changes priority.
4. Distinguish `CONFIRMED`, `EVIDENCE`, `INFERENCE`, `TBD`, and `DECISION`.
5. Never fill unknown student ability with assumptions.
6. Update relevant documents and README after meaningful state changes.
7. Work that changes project state is incomplete if README becomes stale.
8. At semester transition, carry end-state evidence forward.

### Minimal prompt for a new chat

> **Cek repo `azharmz/bahasa-inggris-smp` dan lanjutkan.**

## 13. Change Discipline

Git history is the decision/history trail. When new evidence changes the plan, document the change and reason.

---

**Last project-state update:** 2026-09-15  
**Current active scope:** Grade VIII — Semester 1  
**Current phase:** P3 — Diagnostic Administration / Evidence Wait  
**Current next action:** administer `06-assessment/diagnostic/baseline-diagnostic.md` and return G0–G6 evidence.

# Bahasa Inggris SMP — Project Control

> **Repository ini adalah ONLY AUTHORITATIVE SOURCE OF TRUTH untuk proyek pembelajaran ini.**
>
> Riwayat chat bukan project state. Setiap sesi baru harus membaca README ini terlebih dahulu, lalu mengikuti tautan ke dokumen authoritative yang relevan. Jika chat/memori bertentangan dengan repo, **repo yang berlaku**.

## 1. Project Purpose

Membangun sistem pembelajaran Bahasa Inggris SMP yang terstruktur, realistis terhadap kemampuan aktual peserta didik, selaras dengan Capaian Pembelajaran (CP), dan menggunakan buku resmi sebagai sumber utama tanpa menjadikan urutan halaman buku sebagai pacing authority.

**Current active implementation:** Kelas VIII SMP.  
**Current implementation cycle:** Semester Ganjil / Semester 1.

Repo ini tidak dibatasi hanya untuk Semester 1. Semester berikutnya melanjutkan evidence dan state pembelajaran semester sebelumnya. Arsitektur juga tidak boleh menghalangi perluasan ke kelas SMP lain pada masa depan, tetapi pekerjaan saat ini tetap fokus pada Kelas VIII.

Prinsip kerja utama:

**CP-aligned · student-level-adjusted · textbook-supported · evidence-driven**

## 2. Teaching Context — CONFIRMED

- Current active grade: VIII SMP
- Current semester: Ganjil / Semester 1
- 1 JP: 40 menit
- Total alokasi: 4 JP/pekan
- Intrakurikuler: 3 JP/pekan = 120 menit
- Kokurikuler: 1 JP/pekan = 40 menit
- Buku utama: *English for Nusantara untuk SMP/MTs Kelas VIII*, 2022
- Kondisi penting: pembelajaran sebelumnya belum mengikuti buku siswa secara sistematis.
- Baseline kemampuan siswa: **NOT YET FORMALLY ASSESSED**.

### Continuity Contract

Semester adalah **timebox**, bukan pemisah kompetensi. End-of-semester evidence menjadi entry state semester berikutnya.

```text
Semester 1 baseline
    ↓
instruction + assessment
    ↓
Semester 1 end-state evidence
    ↓
Semester 2 entry state
    ↓
Semester 2 instruction + assessment
```

## 3. Authority Hierarchy

1. CP/ketentuan kurikulum resmi yang berlaku.
2. Evidence kemampuan aktual peserta didik.
3. Keputusan kurikulum/pembelajaran yang telah didokumentasikan di repo.
4. *English for Nusantara VIII* sebagai primary textbook/resource untuk current active grade.
5. Materi pendukung yang diterima dan dicatat di repo.

Buku adalah sumber utama pembelajaran, **bukan kewajiban pacing halaman demi halaman**.

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
Student Baseline / Current Evidence
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
    ↓
End-state evidence → next semester entry state
```

## 5. Instructional Status Vocabulary

- `FOUNDATION` — membangun kemampuan dasar yang menjadi prerequisite.
- `BRIDGE` — menghubungkan kemampuan dasar ke target kelas VIII/buku.
- `TEXTBOOK-ALIGNED` — langsung mengerjakan target/unit buku yang dipetakan.
- `ASSESSMENT` — pengumpulan evidence penguasaan/kemajuan.

## 6. Repository Map

```text
README.md                         ← START HERE / project control
01-governance/
  source-of-truth.md
  teaching-principles.md
02-sources/
  curriculum-sources.md           ← official Phase D curriculum source
  textbook-audit.md               ← Grade VIII textbook evidence/task audit
03-baseline/
  class-profile.md
  student-entry-level.md          ← to be created from diagnostic evidence
  gap-analysis.md                 ← after baseline evidence
04-curriculum-map/
  competency-map.md               ← CP → Grade VIII operational strands
  prerequisite-map.md             ← dependencies + diagnostic gates
  semester-1-scope-sequence.md    ← AFTER diagnostic/gap analysis
  semester-2-scope-sequence.md    ← later
05-teaching/
  semester-1/
  semester-2/
06-assessment/
  diagnostic/                     ← CURRENT WORKSTREAM
  formative/
  summative/
07-cocurricular/
  semester-1.md
  semester-2.md
08-progress/
  teaching-log.md
  student-progress.md
```

Direktori/file dibuat bertahap saat dibutuhkan; jangan membuat dokumen kosong hanya untuk memenuhi tree.

## 7. Authoritative Sources — CURRENT

### Curriculum

2025 *Panduan Mata Pelajaran Bahasa Inggris: Fase B–F dan Fase F Tingkat Lanjut*, Pusat Kurikulum dan Pembelajaran / BSKAP, Kemendikdasmen.

Phase D end target is approximately CEFR A2 and spans Listening–Speaking, Reading–Viewing, and Writing–Presenting. See `02-sources/curriculum-sources.md`.

### Textbook

*English for Nusantara untuk SMP/MTs Kelas VIII* (2022), ISBN `978-602-427-941-7`.

The book integrates listening, speaking, reading, viewing, writing, and representing through genre/text-based learning. The audit now includes actual task samples and prerequisite observations. See `02-sources/textbook-audit.md`.

## 8. Non-Negotiable Teaching Principles

1. **Jangan mengejar halaman buku demi mengejar ketertinggalan.**
2. CP menentukan arah; kemampuan aktual siswa menentukan titik mulai.
3. Jangan mengajarkan target kompleks sebelum prerequisite kritis tersedia.
4. Sederhanakan input/tugas bila perlu tanpa kehilangan arah kompetensi.
5. Grammar/vocabulary adalah alat untuk fungsi komunikasi, bukan satu-satunya tujuan kurikulum.
6. 3 JP intrakurikuler dan 1 JP kokurikuler direncanakan sebagai jalur berbeda tetapi saling mendukung.
7. Keputusan maju/remediasi harus semakin berbasis evidence kelas.
8. Jangan mengarang baseline, mastery, atau teaching history.
9. Pergantian semester tidak mereset learning state.

## 9. CURRENT STATE

**Active scope: Grade VIII — Semester 1**  
**Phase: P2 — DIAGNOSTIC BASELINE DESIGN**

### P0 — Repository Bootstrap

- [x] Repo = only authoritative source of truth.
- [x] Teaching context recorded.
- [x] Semester-continuous architecture established.

### P1 — Authoritative Source Audit

- [x] Current official Phase D English curriculum source verified and documented.
- [x] Phase D element targets documented.
- [x] Grade VIII textbook identity/approach mapped.
- [x] Textbook chapter/unit scope mapped.
- [x] Actual task demands sampled across Chapters 0–5.
- [x] Grade VIII competency map v0.1 created.
- [x] Prerequisite/dependency map v0.1 created.
- [x] Compact diagnostic gates G0–G6 defined.

Open P1 detail that does **not** block P2:

- [ ] resolve Chapter 1 Unit 3 front-matter discrepancy if/when that unit is used in detailed planning.

### Not Yet Completed

- [ ] Design feasible diagnostic baseline instrument.
- [ ] Administer diagnostic / collect classroom evidence.
- [ ] Record `student-entry-level.md`.
- [ ] Gap analysis.
- [ ] Semester 1 Scope & Sequence.
- [ ] Semester 1 cocurricular pathway.
- [ ] Weekly teaching packages.

## 10. NEXT ACTION

**P2 — Diagnostic Baseline Design**

Design a **small, classroom-feasible diagnostic**, not a large exam, to sample prerequisite gates from `04-curriculum-map/prerequisite-map.md`:

- G0 classroom access;
- G1 familiar/high-frequency vocabulary;
- G2 very simple `be` + lexical-verb sentence access;
- G3 positive/negative/question access;
- G4 explicit information extraction from a very short familiar text;
- G5 basic past-event readiness;
- G6 ability to connect 2–3 ideas/events with support.

Diagnostic should fit the real 40-minute JP structure and produce evidence usable for deciding `FOUNDATION`, `BRIDGE`, or direct `TEXTBOOK-ALIGNED` starting points.

**Do not create Semester 1 Scope & Sequence before diagnostic evidence is available.**

## 11. Rules for Every Future ChatGPT Session

1. Read `README.md` first.
2. Repo is project truth; do not reconstruct state from old chats.
3. Follow CURRENT STATE and NEXT ACTION unless user changes priority.
4. Distinguish `CONFIRMED`, `EVIDENCE`, `INFERENCE`, `TBD`, and `DECISION`.
5. Never fill unknown student ability with assumptions.
6. Update relevant documents and README after meaningful state changes.
7. Work that changes project state is incomplete if README becomes stale.
8. At semester transition, carry end-state evidence forward; do not reset learning state.

### Minimal prompt for a new chat

> **Cek repo `azharmz/bahasa-inggris-smp` dan lanjutkan.**

## 12. Change Discipline

Git history is the decision/history trail. When new evidence changes the plan, document the change and reason rather than rewriting history as if the new decision had always been known.

---

**Last project-state update:** 2026-09-15  
**Current active scope:** Grade VIII — Semester 1  
**Current phase:** P2 — Diagnostic Baseline Design  
**Current next action:** build the compact diagnostic instrument for G0–G6.

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
- Buku utama: *English for Nusantara untuk SMP/MTs Kelas VIII*, Kementerian Pendidikan, Kebudayaan, Riset, dan Teknologi, 2022
- Kondisi penting: pembelajaran sebelumnya belum mengikuti buku siswa secara sistematis.
- Baseline kemampuan siswa: **NOT YET FORMALLY ASSESSED**. Jangan menganggap percakapan atau impresi informal sebagai baseline final.

### Continuity Contract

Semester adalah **timebox**, bukan pemisah kompetensi. End-of-semester evidence menjadi entry state semester berikutnya:

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

Jangan mereset baseline hanya karena semester berganti dan jangan menganggap target yang direncanakan otomatis telah dikuasai.

## 3. Authority Hierarchy

Urutan otoritas proyek:

1. CP/ketentuan kurikulum resmi yang berlaku.
2. Evidence kemampuan aktual peserta didik.
3. Keputusan kurikulum/pembelajaran yang telah didokumentasikan di repo.
4. Buku *English for Nusantara VIII* sebagai primary textbook/resource untuk current active grade.
5. Materi pendukung lain yang secara eksplisit diterima dan dicatat di repo.

Buku adalah sumber utama pembelajaran, **bukan kewajiban pacing halaman demi halaman**. Foundation/bridge instruction boleh dan perlu diberikan bila prerequisite peserta didik belum memadai.

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

`competency-map.md` dan `prerequisite-map.md` tidak boleh dipecah secara artifisial hanya karena pergantian semester. Semester scope & sequence adalah implementasi berbatas waktu dari competency path yang lebih panjang.

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
  textbook-audit.md               ← audit authoritative buku current grade
  curriculum-sources.md           ← sumber CP/kurikulum resmi
03-baseline/
  class-profile.md                ← konteks kelas yang diketahui
  student-entry-level.md          ← baseline/evidence entry state
  gap-analysis.md                 ← gap prerequisite → target
04-curriculum-map/
  competency-map.md               ← CP → kompetensi operasional grade VIII
  prerequisite-map.md             ← dependency kemampuan lintas semester
  semester-1-scope-sequence.md    ← roadmap Semester 1 authoritative
  semester-2-scope-sequence.md    ← dibuat saat Semester 2 direncanakan
05-teaching/
  semester-1/                     ← paket pembelajaran Semester 1
  semester-2/                     ← dibuat saat Semester 2 dimulai
06-assessment/
  diagnostic/                     ← asesmen baseline/entry-state
  formative/                      ← evidence selama proses
  summative/                      ← asesmen akhir/unit bila diperlukan
07-cocurricular/
  semester-1.md                   ← jalur 1 JP kokurikuler Semester 1
  semester-2.md                   ← dibuat saat Semester 2 direncanakan
08-progress/
  teaching-log.md                 ← apa yang benar-benar diajarkan
  student-progress.md             ← evidence kemajuan/agregat kelas
```

Direktori/file dibuat bertahap saat memang dibutuhkan. Struktur di atas adalah contract organisasi, bukan alasan membuat dokumen kosong. File Semester 2 **belum perlu dibuat sekarang**; Repository Map hanya menetapkan jalur ekspansi agar arsitektur Semester 1 tidak menjadi jalan buntu.

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
9. Pergantian semester tidak mereset learning state; evidence semester sebelumnya dibawa ke semester berikutnya.

## 9. CURRENT STATE

**Active scope: Grade VIII — Semester 1**  
**Phase: P1 — AUTHORITATIVE SOURCE AUDIT**

Confirmed:

- [x] Repo ditetapkan sebagai only authoritative source of truth.
- [x] Teaching context dasar ditetapkan.
- [x] Buku utama kelas VIII teridentifikasi dan tersedia untuk audit.
- [x] Arsitektur proyek ditetapkan.
- [x] Arsitektur dibuat semester-continuous: Semester 2 akan meneruskan end-state evidence Semester 1, bukan memulai ulang.

Not yet completed:

- [ ] Ambil dan verifikasi CP Bahasa Inggris Fase D dari sumber resmi yang berlaku.
- [ ] Audit buku *English for Nusantara VIII* secara sistematis.
- [ ] Bangun competency map Grade VIII yang dapat melintasi Semester 1–2.
- [ ] Bangun prerequisite map.
- [ ] Rancang diagnostic baseline yang ringan dan feasible.
- [ ] Tetapkan baseline siswa dari evidence.
- [ ] Gap analysis.
- [ ] Susun Semester 1 Scope & Sequence.
- [ ] Susun jalur kokurikuler Semester 1.
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
9. Saat semester berganti, gunakan end-state evidence semester sebelumnya sebagai entry state; jangan melakukan reset administratif terhadap kemampuan siswa.

### Minimal prompt untuk chat baru

> **Cek repo `azharmz/bahasa-inggris-smp` dan lanjutkan.**

Prompt tersebut harus cukup untuk memulihkan state proyek tanpa handoff manual.

## 12. Change Discipline

Git history adalah decision/history trail. Jangan menghapus histori ketidakpastian dengan menulis ulang seolah keputusan sudah diketahui sejak awal. Bila evidence baru mengubah rencana, dokumentasikan perubahan dan alasannya.

---

**Last project-state update:** 2026-09-15  
**Current active scope:** Grade VIII — Semester 1  
**Current next action:** P1 — Authoritative Source Audit

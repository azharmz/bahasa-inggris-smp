# Source of Truth Governance

## Rule

Repository `azharmz/bahasa-inggris-smp` adalah **only authoritative source of truth** untuk project state pembelajaran Bahasa Inggris SMP ini.

Chat, memory, draft lokal, dan percakapan terdahulu dapat membantu proses kerja tetapi tidak memiliki otoritas jika belum tercermin di repo.

## Authority

Untuk substansi pembelajaran, gunakan hierarchy:

1. Regulasi/CP resmi yang berlaku.
2. Evidence kemampuan aktual peserta didik.
3. Keputusan yang telah didokumentasikan di repo.
4. Primary textbook yang telah ditetapkan.
5. Supporting sources yang diterima secara eksplisit.

## State Recovery

Sesi baru wajib memulai dari `README.md`. README harus menunjukkan:

- teaching context;
- authoritative documents;
- current phase/state;
- completed/not-completed work;
- next action;
- lokasi detail evidence/decision.

Tidak diperlukan handoff manual selama README dan dokumen yang ditunjuknya up to date.

## Update Contract

Setiap perubahan yang mengubah arah, status, atau posisi pembelajaran harus:

1. memperbarui dokumen detail yang relevan;
2. memperbarui `README.md` bila CURRENT STATE/NEXT ACTION berubah;
3. tidak mengklaim mastery, baseline, atau teaching history tanpa evidence.

## Evidence Labels

Gunakan label konseptual berikut saat relevan:

- `CONFIRMED` — fakta/constraint yang telah ditetapkan.
- `EVIDENCE` — didukung sumber resmi, textbook, assessment, atau classroom record.
- `INFERENCE` — interpretasi yang masuk akal tetapi bukan fakta langsung.
- `TBD` — belum diketahui/ditetapkan.
- `DECISION` — pilihan desain pembelajaran yang telah diambil.

## Anti-Staleness Rule

Pekerjaan yang mengubah project state belum selesai jika README masih menggambarkan state lama.

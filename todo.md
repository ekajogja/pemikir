# Rencana Penambahan Profil Tokoh (Batch 5 Nama)

Dokumen ini berfungsi sebagai panduan operasional dan pelacakan kemajuan untuk penambahan profil pemikir dari `tokohtambahan.md`.

## 1. Alur Kerja Standar (Standard Operating Procedure)

Setiap tokoh harus melalui fase-fase berikut sebelum file `.md` dibuat di folder `_tokoh/`:

### A. Tahap Riset & Vetting (Filter Ketat)
1.  **Verifikasi Integritas:** Pencarian rekam jejak terkait skandal korupsi (LHKPN, putusan pengadilan, pemberitaan media), pelecehan seksual, atau catatan kriminalitas lainnya.
    *   *Kriteria:* Jika ditemukan catatan valid, tokoh **diskualifikasi**.
2.  **Verifikasi Substansi Intelektual:** Memastikan tokoh memiliki "Pokok Pemikiran" yang terdokumentasi dalam karya tulis (buku/jurnal) atau teori/konsep yang diakui.
    *   *Kriteria:* Jika murni praktisi/birokrat tanpa warisan pemikiran, tokoh **ditangguhkan**.
3.  **Pengumpulan Metadata:** Tanggal lahir/wafat, afiliasi, bidang, pendidikan, dan daftar karya utama.

### B. Tahap Implementasi (Penulisan)
1.  **Format File:** `nama-depan-nama-belakang.md` (huruf kecil, kebab-case, tanpa gelar).
2.  **Kontributor:** Menggunakan nama `Anonim`.
3.  **Tanggal Diperbarui:** `2026-03-08`.
4.  **Narasi:** Minimal 150-400 kata, gaya ensiklopedis, fokus pada *apa* yang dipikirkan tokoh, bukan sekadar riwayat jabatan.

### C. Tahap Validasi & Manifest
1.  Menambahkan nama ke `daftar-tokoh.txt` secara alfabetis.
2.  Verifikasi format YAML untuk memastikan integrasi ke `assets/data/tokoh.json` berjalan lancar.

### D. Tahap Cleanup (Pembersihan Antrean)
1.  **Menghapus nama tokoh** yang sudah diterbitkan atau yang sudah dieliminasi (diskualifikasi) dari file `tokohtambahan.md` untuk menjaga akurasi antrean.

---

## 2. Status Antrean Batch (Log Kemajuan)

### Batch 1-5: Selesai ✅ (25 Tokoh)

### Batch 6: Selesai ✅ (5 Tokoh)

### Batch 7: Selesai ✅ (5 Tokoh)

### Batch 8: Selesai ✅ (5 Tokoh)

### Batch 9: Selesai ✅ (5 Tokoh)

### Batch 10: Selesai ✅
| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Asep Kadarohman | [x] | [x] | Terbit |
| Asep Saepudin Jahar | [x] | [x] | Terbit |
| Asman Boedisantoso Ranakusuma | [x] | [x] | Terbit |
| Asrinaldi | [x] | [x] | Terbit |
| Asrorun Ni'am Sholeh | [x] | [x] | Terbit |

### Batch 11: Riset Dimulai
| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Aswanto | [ ] | [ ] | Antre |
| Romli Atmasasmita | [ ] | [ ] | Antre |
| Aziz Haily | [ ] | [ ] | Antre |
| Harsja W. Bachtiar | [ ] | [ ] | Antre |
| Justika Baharsjah | [ ] | [ ] | Antre |

---

## 3. Daftar Diskualifikasi (Alasan Keamanan/Integritas)
*Daftar ini mencatat nama-nama dari `tokohtambahan.md` yang tidak lolos sensor kurasi. Catatan lengkap ada di `daftar-tokoh-tereliminasi.txt`.*

| Nama Tokoh | Alasan Penolakan | Sumber |
| :--- | :--- | :--- |
| Roeslan Abdulgani | Kasus Korupsi Percetakan Negara (1956) | Historia.id, Voi.id |
| Tri Hanggono Achmad | Dugaan penyimpangan dana abadi Unpad (Laporan KPK 2019) | Tempo, Detik |
| Ahmad Amarullah | Isu tunggakan hak dosen (Tukin) & audit internal (2024) | Berita Banten |
| Anak Agung Raka Sudewi | Keterlibatan (saksi/cekal) skandal dana SPI Udayana (2023) | Antara, Kumparan |
| Ari Kuncoro | Skandal rangkap jabatan Komisaris BUMN & revisi Statuta UI (2021) | Tempo, Tirto |
| Arief Hidayat | Pelanggaran kode etik berulang sebagai Hakim Konstitusi | MKMK, ICW |

---

## 4. Konvensi Penulisan (Checklist Akhir)
- [ ] Tidak menggunakan gelar akademik (Prof, Dr, dsb) di nama file.
- [ ] Menggunakan string untuk field `lahir` dan `wafat` di YAML.
- [ ] Minimal 2 rujukan valid di bagian `sumber`.
- [ ] Narasi menggunakan Bahasa Indonesia baku.

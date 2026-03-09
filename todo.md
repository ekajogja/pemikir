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

### Batch 6-10: Selesai ✅ (25 Tokoh)
- Semua profil telah diverifikasi integritas dan substansinya.
- Perbaikan UI (Warna link footer & body) telah diimplementasikan.
- Halaman Indeks Tokoh alfabetis (`indeks.md`) telah dibuat.
- Perubahan telah di-merge ke branch `main` (kecuali `todo.md` & `tokohtambahan.md`).

### Batch 11: Selesai ✅ (5 Tokoh)
- Tokoh: Aswanto, Romli Atmasasmita, Aziz Haily, Harsja W. Bachtiar, Justika Baharsjah.

### Batch 12: Selesai ✅ (5 Tokoh)
- Tokoh: Sjarifuddin Baharsjah, Baharuddin Syarif, Kasmat Bahoewinangoen, Bahrullah Akbar, Jamil Bakar.

### Batch 13: Selesai ✅ (5 Tokoh)
- Tokoh: Bambang Guritno, Bambang Hero Saharjo, Bambang Sudibyo, Bambang Suhendro, Binti Maunah.

### Batch 14: Selesai ✅ (5 Tokoh)
- Tokoh: Boedi Harsono, Boediono, Boedisoesetya, Boer Mauna, Brian Yuliarto.

### Batch 15: Sedang Diproses
| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Satryo Brodjonegoro | [ ] | [ ] | Antrean |
| Soemantri Brodjonegoro | [ ] | [ ] | Antrean |
| Budi Darma | [ ] | [ ] | Antrean |
| Budi Wiweko | [ ] | [ ] | Antrean |
| Burhanuddin Daya | [ ] | [ ] | Antrean |

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
| Siti Nurbaya Bakar | Kasus korupsi tata kelola sawit (Kejagung 2026) | Tempo, CNN |

## 4. Konvensi Penulisan (Checklist Akhir)
- [x] Nama file: `nama-tokoh.md` (lowercase, kebab-case, tanpa gelar).
- [x] Front Matter: Wajib ada `layout: tokoh`.
- [x] Front Matter: Field `diperbarui` menggunakan format `YYYY-MM-DD`.
- [x] Front Matter: Field `lahir` & `wafat` wajib string (contoh: `"1945"`).
- [x] Front Matter: Field `sumber` wajib list objek dengan `url` dan `label`.
- [x] Front Matter: Lengkapi field wajib (`periode`, `bidang`, `pendidikan`, `pokok_pikiran`, `karya_utama`).
- [x] Narasi: Minimal 150-400 kata, Bahasa Indonesia baku, gaya ensiklopedis.
- [x] Sinkronisasi: Tambahkan nama ke `daftar-tokoh.txt` secara alfabetis.
- [x] Referensi: Bandingkan struktur dengan `_tokoh/a-mukti-ali.md` sebagai standar utama.

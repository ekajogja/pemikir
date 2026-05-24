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

- **Batch 1-20 (Selesai):** 105 Tokoh (Log detail diarsipkan).
- **Batch 21 (Selesai):** Edi Sedyawati, Edi Slamet Irianto, Edvin Aldrian, Efa Yonnedi.

- **Batch 22 (Selesai):** Sofian Effendi, Eka Putra Wirman, Elfi Sahlan Ben, Endang Soetari Ad, Enny Nurbaningsih.
- **Batch 23 (Selesai):** Hendra Esmara, Evi Fitriani, F.X. Arif Adimoelja, Fachrudin, Abdul Malik Fadjar.
- **Batch 24 (Selesai):** Fadjry Djufry, Faisal Yunus, Faisol Nasar bin Madi, Fauzan, Freddy P. Zen.
- **Batch 25 (Selesai):** Furqon, Furtasan Ali Yusuf, Ganefri, Radi A. Gany, Garuda Wiko.
- **Batch 26 (Selesai):** Effendi Gazali, Aisjah Girindra, Syamsul Gultom, Syawal Gultom, Gunawan Suryoputro. (Catatan: Miranda Goeltom didiskualifikasi).
- **Batch 27 (Selesai):** Gunawan Tjahjono, H.B. Saanin, Sutrisno Hadi, Soejono Hadinoto, Toyib Hadiwijaya.
- **Batch 28 (Selesai):** Haedar Nashir, Didin Hafidhuddin, Hafrijal Syandri, Hamdi Muluk, Aliyah Hamka.
- **Batch 29 (Selesai):** Andi Hamzah, A. Sobana Hardjasaputra, Hardjoso Prodjopangarso, Sudarsono Hardjosoekarto. (Catatan: Andar Amin Harahap didiskualifikasi - murni praktisi).
- **Batch 30 (Selesai):** Harkristuti Harkrisnowo, Hasan Zaini, Basri Hasanuddin, Ibrahim Hasan. (Catatan: Hasbi Hasan didiskualifikasi - skandal korupsi MA, Haswandi ditangguhkan - praktisi & kontroversial).
- **Batch 31 (Selesai):** Meutia Hatta, Gusti Muhammad Hatta. (Catatan: Muhammad Hatta Ali ditangguhkan - murni praktisi).
- **Batch 32 (Selesai):** Lilik Hendrajaya, Herry Suhardiyanto, Bambang Hidayat, Aida Vitayala Sjafri Hubeis, Hussein Jayadiningrat. (Catatan: Eddy Hiariej didiskualifikasi - skandal suap KPK, Hendrawan Supratikno ditangguhkan - praktisi politik, Heri Hermansyah ditangguhkan - kontroversi akademik).
- **Batch 33 (Selesai):** Himsar Ambarita, Hoepoediono Soewondho, Jannes Humuntal Hutasoit, Huzaemah Tahido Yanggo, Ibenzani Usman. (Catatan: Sholeh Hidayat didiskualifikasi - plagiarisme, I Made Bakta didiskualifikasi - pemalsuan akta, Hendrawan Supratikno ditangguhkan - praktisi politik).
- **Batch 34 (Selesai):** I Made Damriyasa, I Nengah Kerta Besung, I Nyoman Suartha, I Wayan Bawa, Idrus Paturusi.
- **Batch 35 (Selesai):** Riswandha Imawan, Irwan Prayitno, Ismail Novel, Iwan Sugihartono, Teuku Jacob. (Catatan: Denny Indrayana didiskualifikasi - tersangka korupsi).
- **Batch 36 (Selesai):** Fasli Jalal, Jamaluddin Jompa, James Hellyward, Umar Anggara Jenie, Joenil Kahar.



---

## 3. Daftar Diskualifikasi
*Daftar lengkap tokoh yang tidak lolos sensor (Keamanan/Integritas) dapat dilihat di file `daftar-tokoh-tereliminasi.txt`.*

## 4. Konvensi Penulisan (Checklist Akhir)
- [x] Nama file: `nama-tokoh.md` (lowercase, kebab-case, tanpa gelar).
- [x] Front Matter: Wajib ada `layout: tokoh`.
- [x] Front Matter: Field `diperbarui` menggunakan format `YYYY-MM-DD`.
- [x] Front Matter: Field `lahir` & `wafat` wajib string (contoh: `"1945"`).
- [x] Front Matter: Field `sumber` wajib list objek dengan `url` dan `label`.
- [x] Front Matter: Lengkapi field wajib (`periode`, `bidang`, `pendidikan`, `pokok_pikiran`, `karya_utama`).
- [ ] Front Matter: **Wajib gunakan tanda kutip** pada nilai string yang mengandung titik dua (contoh: `judul: "Judul: Subjudul"`).
- [x] Narasi: Minimal 150-400 kata, Bahasa Indonesia baku, gaya ensiklopedis.
- [x] Sinkronisasi: Tambahkan nama ke `daftar-tokoh.txt` secara alfabetis.
- [x] Referensi: Bandingkan struktur dengan `_tokoh/a-mukti-ali.md` sebagai standar utama.

## 5. Ricek Sintaks YAML

Sebelum mengerjakan batch berikutnya, selalu lakukan ricek sintaks YAML agar sesuai dengan templat di `CONTRIBUTING.md`. Pastikan tidak ada "unquoted colons" di dalam nilai (value) YAML, karena akan menyebabkan error pada Jekyll build (Mapping values are not allowed in this context).


# Rencana Penambahan Profil Tokoh (Batch 5 Nama)

Dokumen ini berfungsi sebagai panduan operasional dan pelacakan kemajuan untuk penambahan profil pemikir dari `tokohtambahan.md`.

## 1. Alur Kerja Standar (Standard Operating Procedure)

Setiap tokoh harus melalui fase-fase berikut sebelum file `.md` dibuat di folder `_tokoh/`:

### A. Tahap Riset & Vetting (Filter Ketat)

1. **Verifikasi Integritas:** Pencarian rekam jejak terkait skandal korupsi (LHKPN, putusan pengadilan, pemberitaan media), pelecehan seksual, atau catatan kriminalitas lainnya.
    * *Kriteria:* Jika ditemukan catatan valid, tokoh **diskualifikasi**.
2. **Verifikasi Substansi Intelektual:** Memastikan tokoh memiliki "Pokok Pemikiran" yang terdokumentasi dalam karya tulis (buku/jurnal) atau teori/konsep yang diakui.
    * *Kriteria:* Jika murni praktisi/birokrat tanpa warisan pemikiran, tokoh **ditangguhkan**.
3. **Pengumpulan Metadata:** Tanggal lahir/wafat, afiliasi, bidang, pendidikan, dan daftar karya utama.

### B. Tahap Implementasi (Penulisan)

1. **Format File:** `nama-depan-nama-belakang.md` (huruf kecil, kebab-case, tanpa gelar).
2. **Kontributor:** Menggunakan nama `Anonim`.
3. **Tanggal Diperbarui:** `2026-03-08`.
4. **Narasi:** Minimal 150-400 kata, gaya ensiklopedis, fokus pada *apa* yang dipikirkan tokoh, bukan sekadar riwayat jabatan.

### C. Tahap Validasi & Manifest

1. Menambahkan nama ke `daftar-tokoh.txt` secara alfabetis.
2. Verifikasi format YAML untuk memastikan integrasi ke `assets/data/tokoh.json` berjalan lancar.

### D. Tahap Cleanup (Pembersihan Antrean)

1. **Menghapus nama tokoh** yang sudah diterbitkan atau yang sudah dieliminasi (diskualifikasi) dari file `tokohtambahan.md` untuk menjaga akurasi antrean.

---

## 2. Status Antrean Batch (Log Kemajuan)

### Batch 1: Selesai ✅

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Abdul Aziz Dahlan | [x] | [x] | Terbit |
| Abdul Djalil Pirous | [x] | [x] | Terbit |
| Abdul Haris | [x] | [x] | Terbit |
| Abdul Madjid Ibrahim | [x] | [x] | Terbit |
| Abdul Mu'ti | [x] | [x] | Terbit |

### Batch 2: Selesai ✅

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Kadir Abdussamad | [x] | [x] | Terbit |
| Achdiat K. Mihardja | [x] | [x] | Terbit |
| Achmad Baiquni | [x] | [x] | Terbit |
| Adi Maulana | [x] | [x] | Terbit |
| Mochamad Adnan | [x] | [x] | Terbit |

### Batch 3: Selesai ✅

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Saleh Afiff | [x] | [x] | Terbit |
| Agus Sartono | [x] | [x] | Terbit |
| Raudha Thaib | [x] | [x] | Terbit |
| Agustinus Purna Irawan | [x] | [x] | Terbit |
| Agustinus Suhardi | [x] | [x] | Terbit |

### Batch 4: Selesai ✅

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Ahmad Najib Burhani | [x] | [x] | Terbit |
| Ahmad Sutarmadi | [x] | [x] | Terbit |
| Ahman | [x] | [x] | Terbit |
| Akhmaloka | [x] | [x] | Terbit |
| Al Makin | [x] | [x] | Terbit |

### Batch 5: Selesai ✅

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Ali Hanafiah | [x] | [x] | Terbit |
| Ali Khomsan | [x] | [x] | Terbit |
| Armida Alisjahbana | [x] | [x] | Terbit |
| Iskandar Alisjahbana | [x] | [x] | Terbit |
| Aloei Saboe | [x] | [x] | Terbit |

### Batch 6: Menunggu Riset

| Nama Tokoh | Integritas | Substansi | Status |
| :--- | :---: | :---: | :--- |
| Bachtiar Aly | [ ] | [ ] | Antre |
| Amal Fathullah Zarkasyi | [ ] | [ ] | Antre |
| Ichlasul Amal | [ ] | [ ] | Antre |
| Amalia E. Maulana | [ ] | [ ] | Antre |
| Ahmad Amarullah | [ ] | [ ] | Antre |

---

## 3. Daftar Diskualifikasi (Alasan Keamanan/Integritas)

*Daftar ini mencatat nama-nama dari `tokohtambahan.md` yang tidak lolos sensor kurasi.*

| Nama Tokoh | Alasan Penolakan | Sumber |
| :--- | :--- | :--- |
| Roeslan Abdulgani | Kasus Korupsi Percetakan Negara (1956) | Historia.id, Voi.id |
| Tri Hanggono Achmad | Dugaan penyimpangan dana abadi Unpad (Laporan KPK 2019) | Tempo, Detik |

---

## 4. Konvensi Penulisan (Checklist Akhir)

* [ ] Tidak menggunakan gelar akademik (Prof, Dr, dsb) di nama file.
* [ ] Menggunakan string untuk field `lahir` dan `wafat` di YAML.
* [ ] Minimal 2 rujukan valid di bagian `sumber`.
* [ ] Narasi menggunakan Bahasa Indonesia baku.

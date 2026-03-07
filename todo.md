# Rencana Kerja: Penambahan Tokoh dari `tokoh-2.txt`

**Objektif:** Menambahkan seluruh tokoh yang terdaftar di `tokoh-2.txt` ke dalam folder `_tokoh/` dengan standar kualitas sesuai `CONTRIBUTING.md`.
**Kontributor:** Anonim
**Tanggal Mulai:** 2026-03-07

---

## 🛠️ Standar Kualitas (Wajib Dipatuhi)

### 1. Format File & Penamaan
- **Path:** `_tokoh/[nama-tokoh-tanpa-gelar].md`
- **Case:** Huruf kecil semua (lowercase).
- **Separator:** Spasi diganti tanda hubung (`-`).
- **Gelar:** Tanpa gelar akademik (Prof, Dr) atau keagamaan (KH, Haji).

### 2. Validasi Front Matter (YAML)
- `layout`: Harus `tokoh`.
- `kontributor`: Diisi `Anonim`.
- `diperbarui`: Format `YYYY-MM-DD` (Tanggal eksekusi).
- `lahir` & `wafat`: **Wajib string** dengan tanda kutip tunggal (misal: `'1945'`). Kosongkan `''` jika masih hidup.
- `periode`: Harus memilih dari nilai legal (`pra 1900`, `1900-1945`, `1945-1965`, `1965-1998`, `1998-2020`, `pasca 2020`).
- `bidang`: Gunakan tag yang relevan (misal: `filsafat`, `sastra`, `politik`).
- `pokok_pikiran`: Ringkasan padat (1-2 kalimat).
- `sumber`: Minimal 1 rujukan valid (URL atau Bukti Cetak).

### 3. Standar Narasi (Markdown)
- **Panjang:** Minimal 150 kata per tokoh.
- **Gaya Bahasa:** Ensiklopedis, formal (EYD), netral, dan tidak opiniatif.
- **Struktur:** 
    - Paragraf 1: Introduksi (siapa, peran utama, signifikansi).
    - Paragraf 2+: Detail pemikiran, karya, atau perjalanan intelektual.

---

## 📋 Daftar Periksa Operasional

### Fase 1: Riset & Pengumpulan Data (Per Batch)
*Rencana: 5 Tokoh per Batch*

- [x] Cari data biografi (Lahir/Wafat, Pendidikan, Afiliasi).
- [x] Identifikasi minimal 1-2 karya utama (Buku/Esai/Artikel).
- [x] Sintesis pokok pikiran utama tokoh berdasarkan literatur.
- [x] Validasi ketersediaan sumber referensi daring/cetak.

### Fase 2: Penulisan & Implementasi
- [x] Buat file `.md` di `_tokoh/`.
- [x] Isi Front Matter YAML sesuai standar di atas.
- [x] Tulis narasi minimal 150 kata.
- [x] Pastikan tidak ada typo pada nama dan istilah teknis.

### Fase 3: Verifikasi Akhir
- [x] Jalankan pengecekan jumlah kata (Word count check).
- [x] Validasi format YAML (Pastikan tidak ada error parsing).
- [x] Cek tautan sumber (Pastikan tidak broken link).

---

## 📈 Log Kemajuan (SELESAI)

| Batch | Jumlah Tokoh | Status |
| :--- | :---: | :---: |
| Batch 1 | 5 | ✅ |
| Batch 2 | 4 | ✅ |
| Batch 3 | 5 | ✅ |
| Batch 4 | 5 | ✅ |
| Batch 5 | 5 | ✅ |
| Batch 6 | 5 | ✅ |
| Batch 7 | 5 | ✅ |
| Batch 8 | 5 | ✅ |
| Batch 9 | 5 | ✅ |
| Batch 10 | 5 | ✅ |
| Batch 11 | 5 | ✅ |

**Total Tokoh Ditambahkan:** 54 Tokoh.

---

## ⚠️ Catatan Penting
- Seluruh tokoh telah dikurasi ketat untuk menjaga standar kualitas intelektual "High-End".
- Beberapa tokoh populer/selebritas telah dieliminasi atau diganti dengan tokoh yang lebih otoritatif.
- Nama-nama tokoh telah disesuaikan dengan ejaan resmi.

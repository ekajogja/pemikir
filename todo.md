# Rencana Kerja: Penambahan Tokoh Tahap Akhir (Menuju 200 Profil)

**Objektif:** Menambahkan 27 tokoh dari `tokoh-tambahan.txt` ke dalam folder `_tokoh/` guna menggenapi direktori menjadi 200 profil tokoh pemikir dengan standar kualitas sesuai `CONTRIBUTING.md`.
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
- `diperbarui`: Format `YYYY-MM-DD`.
- `lahir` & `wafat`: **Wajib string** dengan tanda kutip tunggal (misal: `'1945'`). Kosongkan `''` jika masih hidup.
- `periode`: Harus memilih dari nilai legal (`pra 1900`, `1900-1945`, `1945-1965`, `1965-1998`, `1998-2020`, `pasca 2020`).
- `bidang`: Gunakan tag yang relevan.
- `pokok_pikiran`: Ringkasan padat (1-2 kalimat).
- `sumber`: Minimal 1 rujukan valid (URL atau Bukti Cetak).

### 3. Standar Narasi (Markdown)
- **Panjang:** Minimal 150-200 kata per tokoh.
- **Gaya Bahasa:** Ensiklopedis, formal (EYD), netral, dan tidak opiniatif.
- **Struktur:** 
    - Paragraf 1: Introduksi (siapa, peran utama, signifikansi).
    - Paragraf 2+: Detail pemikiran, karya, atau perjalanan intelektual.

---

## 📈 Log Kemajuan (SELESAI)

### Seluruh Batch (12-16) telah tuntas dikerjakan.
**Total Tokoh Baru Ditambahkan:** 27 Tokoh.
**Total Kumulatif Direktori:** 200 Profil Tokoh Pemikir Indonesia.

---

## ⚠️ Catatan Penting
- Seluruh 200 tokoh kini telah memiliki profil Markdown di folder `_tokoh/`.
- Konsolidasi file daftar telah dilakukan ke dalam `daftar-tokoh.txt`.
- Standar kualitas narasi dan verifikasi sumber telah dipenuhi untuk setiap entri.

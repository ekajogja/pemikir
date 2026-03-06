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

- [ ] Cari data biografi (Lahir/Wafat, Pendidikan, Afiliasi).
- [ ] Identifikasi minimal 1-2 karya utama (Buku/Esai/Artikel).
- [ ] Sintesis pokok pikiran utama tokoh berdasarkan literatur.
- [ ] Validasi ketersediaan sumber referensi daring/cetak.

### Fase 2: Penulisan & Implementasi
- [ ] Buat file `.md` di `_tokoh/`.
- [ ] Isi Front Matter YAML sesuai standar di atas.
- [ ] Tulis narasi minimal 150 kata.
- [ ] Pastikan tidak ada typo pada nama dan istilah teknis.

### Fase 3: Verifikasi Akhir
- [ ] Jalankan pengecekan jumlah kata (Word count check).
- [ ] Validasi format YAML (Pastikan tidak ada error parsing).
- [ ] Cek tautan sumber (Pastikan tidak broken link).

---

## 📈 Log Kemajuan (Batch 1: 5 Tokoh Pertama)

| Tokoh | Status | File |
| :--- | :---: | :--- |
| Abdoel Rivai | ✅ | `abdoel-rivai.md` |
| Abdul Hadi W.M. | ✅ | `abdul-hadi-wm.md` |
| Ahmad Azhar Basyir | ✅ | `ahmad-azhar-basyir.md` |
| Adian Husaini | ✅ | `adian-husaini.md` |
| Ahmad Baso | ✅ | `ahmad-baso.md` |

## 📈 Log Kemajuan (Batch 2: 5 Tokoh Selanjutnya)

| Tokoh | Status | File |
| :--- | :---: | :--- |
| Ajip Rosidi | ✅ | `ajip-rosidi.md` |
| Ali Akbar Navis | ✅ | `ali-akbar-navis.md` |
| Arief Budiman | ✅ | `arief-budiman.md` |
| Arwani Syaerozi | ✅ | `arwani-syaerozi.md` |
| Asep Muhammad Iqbal | ❌ | *(Dieliminasi: Kurang memenuhi kriteria kedalaman pemikiran)* |

## 📈 Log Kemajuan (Batch 3: 5 Tokoh Selanjutnya)

| Tokoh | Status | File |
| :--- | :---: | :--- |
| Asrul Sani | ✅ | `asrul-sani.md` |
| Burhanuddin Mohammad Diah | ✅ | `bm-diah.md` |
| Bahtiar Effendy | ✅ | `bahtiar-effendy.md` |
| Bambang Brodjonegoro | ✅ | `bambang-brodjonegoro.md` |
| Bernard Wilhelm Lapian | ✅ | `bernard-wilhelm-lapian.md` |

## 📈 Log Kemajuan (Batch 4: 5 Tokoh Selanjutnya)

| Tokoh | Status | File |
| :--- | :---: | :--- |
| Nahrowi Dalhar | ✅ | `nahrowi-dalhar.md` |
| Cornel Simanjuntak | ✅ | `cornel-simanjuntak.md` |
| Danton Sihombing | ✅ | `danton-sihombing.md` |
| Djoeanda Kartawidjaja | ✅ | `djoeanda-kartawidjaja.md` |
| Dorodjatun Kuntjoro-Jakti | ✅ | `dorodjatun-kuntjoro-jakti.md` |

## 📈 Log Kemajuan (Batch 5: 5 Tokoh Selanjutnya)

| Tokoh | Status | File |
| :--- | :---: | :--- |
| Darmadjati Supadjar | ⏳ | `darmadjati-supadjar.md` |
| Ernest Douwes Dekker | ⏳ | `ernest-douwes-dekker.md` |
| Fahmi Idris | ⏳ | `fahmi-idris.md` |
| Fajar Riza Ul Haq | ⏳ | `fajar-riza-ul-haq.md` |
| FX Eko Armada Riyanto | ⏳ | `fx-eko-armada-riyanto.md` |

---

## ⚠️ Catatan Penting
- Jika data tahun lahir/wafat tidak ditemukan secara pasti, gunakan estimasi abad (misal: `'18xx'`) sesuai panduan atau beri keterangan di narasi.
- Prioritaskan sumber dari jurnal akademik atau situs sejarah terpercaya (Historia.id, Tirto.id, Wikipedia sebagai rujukan awal).

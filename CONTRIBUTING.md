# Panduan Kontributor — Direktori Pemikir Indonesia

Terima kasih sudah tertarik berkontribusi! Dokumen ini menjelaskan cara menambahkan tokoh baru, mengedit data yang sudah ada, dan standar yang harus dipenuhi agar kontribusi diterima.

---

## Daftar Isi

1. [Prasyarat](#prasyarat)
2. [Menambahkan Tokoh Baru](#menambahkan-tokoh-baru)
3. [Mengedit Data Tokoh yang Sudah Ada](#mengedit-data-tokoh-yang-sudah-ada)
4. [Format File Tokoh](#format-file-tokoh)
5. [Aturan Sumber Wajib](#aturan-sumber-wajib)
6. [Panduan Penulisan Narasi](#panduan-penulisan-narasi)
7. [Alur Pull Request](#alur-pull-request)
8. [Pertanyaan Umum](#pertanyaan-umum)

---

## Prasyarat

- Akun GitHub
- Git terinstal di komputer Anda
- (Opsional) Ruby + Bundler untuk menjalankan situs secara lokal

---

## Menambahkan Tokoh Baru

### 1. Fork dan clone repositori

```bash
# Fork dulu di GitHub, lalu:
git clone https://github.com/AKUN_ANDA/pemikir.git
cd pemikir
git checkout -b tambah-tokoh-nama-tokoh
```

### 2. Buat file baru di folder `_tokoh/`

Nama file mengikuti aturan:

- **Format**: `nama-depan-nama-belakang.md`
- Huruf kecil semua
- Spasi diganti tanda strip (`-`)
- Tanpa gelar akademik atau gelar kehormatan

**Contoh:**

| Nama Tokoh | Nama File |
|---|---|
| Prof. Dr. Sri Mulyani | `sri-mulyani.md` |
| Ki Hadjar Dewantara | `ki-hadjar-dewantara.md` |
| H.O.S. Tjokroaminoto | `hos-tjokroaminoto.md` |

### 3. Isi file dengan template berikut

> ⚠️ **PENTING**: Jangan lupa mencantumkan nama Anda di field `kontributor` dan tanggal saat ini di field `diperbarui` dalam template file tokoh. Ini penting untuk pelacakan perubahan dan pengakuan kontribusi Anda.

Lihat [Format File Tokoh](#format-file-tokoh) untuk panduan lengkap.

### 4. (Jika ada sumber cetak) Unggah foto bukti

```bash
# Simpan foto di:
assets/bukti/nama-tokoh-hal-xx.jpg
```

---

## Mengedit Data Tokoh yang Sudah Ada

Jika menemukan kesalahan data (tahun lahir keliru, karya utama tidak lengkap, dll.):

1. Fork dan buat branch baru: `git checkout -b perbaiki-data-nama-tokoh`
2. Edit file yang bersangkutan di `_tokoh/`
3. **Tambahkan nama Anda di field `kontributor`** dengan format: `kontributor: [Nama Sebelumnya], [Nama Anda]` dan **perbarui tanggal** pada field `diperbarui: YYYY-MM-DD`.
4. Di pesan commit, jelaskan **apa** yang diubah dan **mengapa** (sertakan sumber)
5. Buat Pull Request ke branch `main`

> ⚠️ **Penting**: Setiap perubahan data faktual **wajib disertai sumber baru** yang mendukung perubahan tersebut.

---

## Format File Tokoh

Setiap file tokoh terdiri dari dua bagian: **front matter YAML** (metadata) dan **narasi Markdown** (teks deskriptif).

### Template Lengkap

```yaml
---
layout: tokoh
nama: Nama Lengkap Tokoh
kontributor: Nama Lengkap Kontributor
diperbarui: YYYY-MM-DD          # Wajib diisi: tanggal terakhir entri ini diperbarui
lahir: YYYY-MM-DD          # format ISO 8601; isi perkiraan jika tidak pasti
wafat: YYYY-MM-DD          # kosongkan jika masih hidup
tempat_lahir: Kota, Provinsi/Wilayah
afiliasi: Institusi/Organisasi (pisahkan dengan koma jika lebih dari satu)
periode: klasik            # pilih salah satu: klasik | pergerakan | pasca-kemerdekaan | kontemporer
bidang:                    # satu atau lebih bidang
  - filsafat
  - sastra
pendidikan:
  - "Gelar, Institusi, Tahun (jika diketahui)"
  - "Gelar, Institusi, Tahun"
pokok_pikiran: "Ringkasan satu-dua kalimat tentang kontribusi/pemikiran utama tokoh."
karya_utama:
  - judul: "Judul Karya"
    tahun: YYYY
    jenis: Buku            # Buku | Esai | Artikel | Memoar | Surat Kabar | dll.
  - judul: "Judul Karya Kedua"
    tahun: YYYY
    jenis: Esai
sumber:
  - url: https://contoh.com/url-lengkap
    label: "Nama Sumber (mis. Wikipedia, Historia.id)"
  - url: /assets/bukti/nama-tokoh-hal-45.jpg
    label: "Judul Buku, hlm. 45 (foto pribadi)"
---

Narasi lengkap tentang tokoh ditulis di sini, dalam Markdown.

Paragraf pertama sebaiknya memperkenalkan tokoh secara ringkas: siapa, kapan, dan mengapa penting.

Paragraf berikutnya bisa mengulas pemikiran, karya, perjalanan hidup, atau kontribusi lebih dalam.
```

### Nilai Valid untuk Field `periode`

| Nilai | Rentang Waktu (Perkiraan) |
|-------|--------------------------|
| `klasik` | Sebelum abad ke-20 |
| `pergerakan` | 1900–1945 (era pergerakan nasional) |
| `pasca-kemerdekaan` | 1945–1998 |
| `kontemporer` | 1998–sekarang |

### Nilai Contoh untuk Field `bidang`

`filsafat`, `sastra`, `politik`, `ekonomi`, `agama`, `antropologi`, `jurnalisme`, `astronomi`, `sains`, `teknologi`, `hukum`, `pendidikan`, `seni`, `musik`, `sejarah`, `sosiologi`, `linguistik`, `feminisme`, `aktivisme`

---

## Aturan Sumber Wajib

**Setiap klaim faktual WAJIB dapat diverifikasi.** Tanpa sumber yang valid, Pull Request tidak akan diterima.

### Sumber Daring

Cantumkan URL lengkap yang bisa diakses publik:

```yaml
sumber:
  - url: https://id.wikipedia.org/wiki/Nama_Tokoh
    label: Wikipedia
  - url: https://historia.id/path/ke/artikel
    label: Historia.id
```

### Sumber Cetak

Jika menggunakan buku, jurnal fisik, atau dokumen yang tidak tersedia daring:

1. Foto halaman yang relevan (pastikan teks terbaca jelas)
2. Simpan di `assets/bukti/` dengan nama deskriptif
3. Rujuk path-nya sebagai sumber:

```yaml
sumber:
  - url: /assets/bukti/tan-malaka-madilog-hal-12.jpg
    label: "Tan Malaka, Madilog (1943), hlm. 12 — foto pribadi"
```

### Yang Tidak Diperbolehkan

- Wawancara atau komunikasi pribadi yang tidak direkam/ditranskrip
- Blog pribadi tanpa rujukan primer
- Media sosial sebagai satu-satunya sumber

---

## Panduan Penulisan Narasi

- **Bahasa**: Indonesia yang baik dan benar
- **Panjang**: Minimal 150 kata, idealnya 200–400 kata
- **Gaya**: Ensiklopedis — informatif, tidak sensasional, tidak opini subjektif
- **Sudut pandang**: Netral; hindari pujian berlebihan atau kritik tanpa dasar
- **Tokoh masih hidup**: Gunakan present tense untuk aktivitas terkini; kosongkan field `wafat`
- **Kutipan langsung**: Jika mengutip perkataan tokoh, sertakan sumber di bagian `sumber`

---

## Alur Pull Request

```
Fork repo → Buat branch → Tambah/edit file → Commit → Push → Buat PR
```

1. Pastikan satu PR hanya memuat satu tokoh (atau satu koreksi data spesifik)
2. Judul PR: `Menambahkan tokoh: [Nama Tokoh]` atau `Memperbaiki data: [Nama Tokoh]`
3. Isi deskripsi PR dengan ringkasan perubahan dan daftar sumber yang digunakan
4. **Pastikan field `kontributor` sudah diisi dengan nama Anda**
5. Pengelola akan meninjau selambatnya dalam 7 hari kerja

---

## Pertanyaan Umum

**Q: Bolehkah menambahkan tokoh yang masih hidup?**  
A: Boleh. Kosongkan field `wafat` dan gunakan present tense di narasi untuk aktivitas terkini.

**Q: Apakah ada daftar tokoh yang belum masuk tapi sangat dibutuhkan?**  
A: Cek [Issues dengan label `dibutuhkan`](https://github.com/ekajogja/pemikir/issues?q=label%3Adibutuhkan) di GitHub.

**Q: Bagaimana jika saya tidak yakin tentang periode atau bidang tokoh?**  
A: Pilih yang paling dominan/representatif. Pengelola bisa membantu menyesuaikan.

**Q: Bolehkah saya menambahkan foto tokoh?**  
A: Saat ini belum tersedia field foto. Fitur ini direncanakan di versi mendatang.

---

Pertanyaan lain? Buka [issue baru](https://github.com/ekajogja/pemikir/issues/new) atau kirim diskusi di tab Discussions.

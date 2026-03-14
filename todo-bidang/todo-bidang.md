# Rencana Kerja Standardisasi Bidang Tokoh (50 Kategori Utama)

Dokumen ini mengatur proses restrukturisasi metadata `bidang` pada setiap profil tokoh untuk meningkatkan konsistensi dan navigasi pada halaman Indeks.

## Fase 1: Audit & Proposi (Minggu 1)
- [x] **Audit Data Eksisting:** Ekstraksi seluruh nilai unik dari field `bidang` pada semua file di `_tokoh/`.
- [x] **Klasterisasi:** Mengelompokkan istilah-istilah yang mirip menjadi kategori standar.
- [x] **Penyusunan Masterlist:** Membuat file `daftar-bidang.txt` yang berisi 48 kategori standar.
- [x] **Validasi Masterlist:** Memastikan 48 kategori tersebut mencakup seluruh spektrum pemikir (Sastra, Sains, Hukum, Agama, Sosial, dll).

## Fase 2: Implementasi Metadata (Minggu 2-3)
- [x] **Mapping:** Membuat file `todo-bidang/mapping-bidang.md` sebagai jembatan nilai lama ke nilai standar.
- [/] **Refactoring Manual:** Memperbarui field `bidang` di setiap file `.md` dalam folder `_tokoh/` (58 file selesai).
- [ ] **Sinkronisasi JSON:** Memastikan perubahan tercermin dalam `assets/data/tokoh.json` (jika digunakan secara statis).

## Fase 3: Pembaruan UI & Dokumentasi (Minggu 4)
- [ ] **Update Indeks:** Modifikasi `indeks.md` (atau layout terkait) untuk menampilkan kolom "Bidang" di samping Nama dan Periode.
- [ ] **Update Dokumentasi:**
    - [ ] `README.md`: Penjelasan singkat sistem klasifikasi baru.
    - [ ] `CONTRIBUTING.md`: Penambahan aturan penulisan profil baru wajib mengikuti `daftar-bidang.txt`.
    - [ ] `tentang.md`: Penjelasan metodologi pengelompokan bidang pemikiran.

## Fase 4: Verifikasi & QC
- [ ] **Pengecekan YAML:** Validasi ulang seluruh file untuk memastikan tidak ada error sintaks pasca-edit massal.
- [ ] **Pengecekan Visual:** Memastikan tampilan tabel di halaman Indeks rapi dan responsif.

---

## Log Kemajuan
- **2026-03-10:** Inisiasi rencana kerja dan pembuatan `todo-bidang.md`.
- **2026-03-10:** Selesai melakukan audit data unik dan menyusun Masterlist 48 Bidang Standar di `daftar-bidang.txt`.
- **2026-03-10:** Selesai menyusun `mapping-bidang.md` dan memulai *refactoring* manual (30 tokoh tuntas, terakhir Ajip Rosidi).

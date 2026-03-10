# Rencana Kerja Standardisasi Bidang Tokoh (50 Kategori Utama)

Dokumen ini mengatur proses restrukturisasi metadata `bidang` pada setiap profil tokoh untuk meningkatkan konsistensi dan navigasi pada halaman Indeks.

## Fase 1: Audit & Proposi (Minggu 1)
- [ ] **Audit Data Eksisting:** Ekstraksi seluruh nilai unik dari field `bidang` pada semua file di `_tokoh/`.
- [ ] **Klasterisasi:** Mengelompokkan istilah-istilah yang mirip (misal: "Hukum Islam", "Fikih", "Syariah" menjadi satu kategori standar).
- [ ] **Penyusunan Masterlist:** Membuat file `daftar-bidang.txt` yang berisi maksimal 50 kategori standar.
- [ ] **Validasi Masterlist:** Memastikan 50 kategori tersebut mencakup seluruh spektrum pemikir (Sastra, Sains, Hukum, Agama, Sosial, dll).

## Fase 2: Implementasi Metadata (Minggu 2-3)
- [ ] **Mapping:** Membuat tabel pemetaan dari nilai lama ke nilai standar baru.
- [ ] **Refactoring Massal:** Memperbarui field `bidang` di setiap file `.md` dalam folder `_tokoh/`.
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

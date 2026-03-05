# Direktori Pemikir Indonesia

Selamat datang di repositori **Direktori Pemikir Indonesia**. Proyek ini bertujuan mendokumentasikan secara sistematis para intelektual, ilmuwan, budayawan, filsuf, aktivis, dan pemikir lainnya dari Indonesia—mulai dari tokoh tradisional seperti Ki Ageng Suryomentaram, aktivis revolusioner seperti Tan Malaka, ilmuwan seperti BJ Habibie, hingga pemikir kontemporer seperti Rocky Gerung.

Situs dapat diakses di **[https://ekajogja.github.io/pemikir](https://ekajogja.github.io/pemikir)**

## Latar Belakang

Informasi mengenai para pemikir Indonesia saat ini masih tersebar di berbagai sumber dan belum terintegrasi dalam satu direktori khusus yang mencakup lintas disiplin. Proyek ini lahir untuk mengisi kekosongan tersebut dengan menyediakan:

- Profil lengkap setiap tokoh (biografi singkat, pokok pikiran/kontribusi, karya utama)
- Pengelompokan berdasarkan periode, bidang keilmuan, atau afiliasi
- Data yang terstruktur, terbuka, dan siap digunakan untuk riset atau pengembangan lebih lanjut

Dengan semangat **open source**, kami mengundang siapa pun untuk berkontribusi—baik peneliti, mahasiswa, maupun masyarakat umum—untuk bersama-sama membangun direktori ini.

## Fitur Utama

- **Periodisasi Sejarah**  
  Tokoh dikelompokkan dalam beberapa era: Tradisional/Klasik, Pergerakan Nasional, Pasca-Kemerdekaan, dan Kontemporer.

- **Pengelompokan Bidang**  
  Misalnya: Filsafat, Ilmu Pengetahuan Alam, Ilmu Sosial, Sastra/Budaya, Politik/Hukum, Agama/Spiritualitas, dan lain-lain.

- **Profil Standar**  
  Setiap entri memuat:  
  - Nama lengkap (dengan gelar)  
  - Tahun lahir-wafat  
  - Tempat lahir  
  - Pendidikan & afiliasi  
  - Pokok pikiran/kontribusi utama  
  - Daftar karya utama  
  - Sumber referensi (wajib)
  - Kontributor
  - Tanggal terakhir diperbarui

- **Pencarian & Filter**  
  Cari berdasarkan nama, periode, bidang, atau institusi.

- **Rencana Pengembangan**  
  - Garis waktu interaktif  
  - Peta persebaran tokoh berdasarkan asal atau tempat berkarya  
  - Indeks karya dengan tautan ke katalog perpustakaan

## Struktur Data

Data tokoh disimpan dalam format **Markdown** dengan front matter YAML di folder `_tokoh/`. Setiap file mewakili satu tokoh.

### Contoh file `_tokoh/rocky-gerung.md`

```yaml
---
layout: tokoh
nama: Rocky Gerung
kontributor: Eka Y Saputra
diperbarui: 2026-03-06
lahir: 1959-01-20
wafat: 
tempat_lahir: Manado, Sulawesi Utara
afiliasi: Universitas Indonesia, Setara Institute
periode: kontemporer
bidang: [filsafat, politik, kritik sosial]
pendidikan: 
  - S1 Filsafat, Universitas Indonesia
  - S2 Filsafat, Universitas Indonesia
pokok_pikiran: "Kritik terhadap kuasa, demokrasi deliberatif, filsafat politik"
karya_utama:
  - judul: "Filsafat Politik: Telaah atas Pemikiran Hannah Arendt"
    tahun: 2006
    jenis: Buku
  - judul: "Demokrasi dan Post-Truth"
    tahun: 2019
    jenis: Esai
sumber:
  - url: https://id.wikipedia.org/wiki/Rocky_Gerung
    label: Wikipedia
  - url: https://www.liputan6.com/news/read/...
    label: Liputan6 (wawancara)
---
```

Konten deskripsi bebas ditulis dalam Markdown setelah front matter. Bagian ini bisa berisi narasi lebih panjang tentang pemikiran, perjalanan hidup, atau kontribusi tokoh.

## Aturan Sumber yang Wajib

**Setiap data yang dimasukkan WAJIB menyertakan sumber yang dapat diverifikasi.** Ini untuk menjaga kredibilitas direktori dan menghindari informasi palsu.

- **Sumber daring**: Jika informasi diambil dari situs web, jurnal online, atau arsip digital, cantumkan URL lengkap di bagian `sumber`.
- **Sumber cetak (buku, jurnal fisik)**: Jika informasi berasal dari buku atau dokumen fisik yang tidak tersedia secara daring, Anda WAJIB menyertakan **foto atau pindaian halaman terkait** sebagai bukti. Foto tersebut dapat diunggah ke folder `assets/bukti/` dengan nama file yang merujuk pada tokoh (misal: `rocky-gerung-buku1.jpg`), lalu cantumkan path lokal sebagai sumber.
  - Contoh:

    ```yaml
    sumber:
      - url: /assets/bukti/rocky-gerung-hal-45.jpg
        label: Buku "Filsafat Politik" hlm. 45 (foto pribadi)
    ```

- **Wawancara atau komunikasi pribadi**: Tidak diperkenankan, kecuali dapat diverifikasi melalui rekaman atau transkrip yang juga diunggah.

Dengan aturan ini, setiap klaim dapat ditelusuri dan dipertanggungjawabkan.

## Cara Berkontribusi

Kami sangat terbuka terhadap kontribusi dari siapa pun. Berikut langkah-langkahnya:

1. **Fork** repositori ini ke akun GitHub Anda.
2. **Buat branch baru** untuk perubahan Anda (`git checkout -b tambah-tokoh-nama`).
3. **Tambahkan data tokoh** baru di folder `_tokoh/` dengan format di atas. Pastikan:
   - Nama file menggunakan format `nama-depan-nama-belakang.md` (tanpa gelar, huruf kecil, spasi diganti strip).
   - Sertakan minimal satu sumber yang valid (lihat aturan di atas).
4. **Jika menggunakan sumber cetak**, unggah foto bukti ke folder `assets/bukti/` dan rujuk path-nya di bagian `sumber`.
5. **Commit** perubahan (`git commit -m 'Menambahkan tokoh: ...'`).
6. **Push** ke branch Anda (`git push origin tambah-tokoh-nama`).
7. Buat **Pull Request** ke repositori ini.

Setiap Pull Request akan ditinjau oleh pengelola. Jika ada kekurangan, kami akan memberikan masukan.

### Panduan Penulisan

- Gunakan bahasa Indonesia yang baik dan benar.
- Tuliskan pokok pikiran/kontribusi secara ringkas namun informatif.
- Hindari opini subjektif; tuliskan berdasarkan rujukan.
- Untuk tokoh yang masih hidup, kosongkan field `wafat`.
- Jika ada beberapa bidang, gunakan daftar (list) YAML.

## Teknologi

- **Static Site Generator:** [Jekyll](https://jekyllrb.com/) (native di GitHub Pages)
- **Tema:** Disesuaikan (menggunakan tema minima dengan modifikasi)
- **Hosting:** GitHub Pages
- **Data:** Markdown + front matter YAML

### Menjalankan secara lokal

1. Pastikan Ruby dan Bundler terinstal.
2. Clone repositori:

   ```bash
   git clone https://github.com/ekajogja/pemikir.git
   cd pemikir
   ```

3. Install dependensi:

   ```bash
   bundle install
   ```

4. Jalankan server lokal:

   ```bash
   bundle exec jekyll serve
   ```

5. Akses `http://localhost:4000` untuk melihat situs.

> **Catatan Khusus untuk Pengguna Ubuntu/Linux:**
> Sering kali `bundle install` gagal karena ekosistem dependensi Jekyll terbaru membutuhkan kompilasi native (seperti `sass-embedded` atau `json`). Jika Anda menemui masalah tersebut, Anda dapat melompati langkah Bundler sepenuhnya dengan menginstal paket bawaan Ubuntu:
>
> ```bash
> sudo apt install jekyll
> jekyll serve
> ```

## Lisensi

- **Kode sumber** (HTML, CSS, JavaScript, konfigurasi Jekyll) dilisensikan di bawah **MIT License** (lihat file [LICENSE](LICENSE)).
- **Konten teks** (profil tokoh) dilisensikan di bawah **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**. Anda bebas menggunakan, membagikan, dan menggubah konten selama mencantumkan atribusi ke proyek ini dan membagikan turunan dengan lisensi yang sama.

Dengan lisensi ini, kami berharap data dapat digunakan seluas-luasnya untuk kepentingan pendidikan dan riset.

## Kontak

Jika Anda memiliki pertanyaan, saran, atau ingin melaporkan kesalahan data, silakan buka [issue](https://github.com/ekajogja/pemikir/issues) di repositori ini.

---

**Mari kita abadikan pemikiran anak bangsa, satu profil pada satu waktu.**  
Terima kasih telah berkontribusi!

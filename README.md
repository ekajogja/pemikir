# Direktori Pemikir Indonesia

Selamat datang di repositori **Direktori Pemikir Indonesia**. Proyek ini bertujuan mendokumentasikan secara sistematis para intelektual, ilmuwan, budayawan, filsuf, aktivis, dan pemikir lainnya dari Indonesia—mulai dari tokoh tradisional, aktivis revolusioner, hingga pemikir kontemporer.

Situs dapat diakses di **[https://ekajogja.github.io/pemikir](https://ekajogja.github.io/pemikir)**

## Fitur Utama

- **Navigasi & Pencarian Canggih**  
  Filter tokoh berdasarkan Nama, Periode, atau Bidang Keilmuan secara instan dengan indikator jumlah hasil yang dinamis.
  
- **Visualisasi Grafik Bidang**  
  Diagram interaktif (Doughnut Chart) yang menunjukkan distribusi keilmuan para pemikir. Klik pada kategori grafik untuk memfilter daftar tokoh secara otomatis.

- **Linimasa Sejarah (Timeline)**  
  Halaman khusus untuk menelusuri jejak intelektual nusantara berdasarkan urutan tahun kelahiran, memberikan konteks sejarah yang lebih mendalam.

- **Data Terstruktur (Internal API)**  
  Metadata tokoh diekspor secara otomatis ke dalam format JSON (`assets/data/tokoh.json`), memudahkan pengembangan fitur visualisasi di masa depan.

- **Profil Standar & Terverifikasi**  
  Setiap entri memuat data biografi, pokok pikiran, karya utama, dan **wajib menyertakan sumber referensi yang dapat diverifikasi**.

## Struktur Data

- Data tokoh disimpan dalam format **Markdown** dengan front matter YAML di folder `_tokoh/`.
- Daftar lengkap tokoh yang terdokumentasi juga dapat dilihat pada file `daftar-tokoh.txt`.
- Untuk transparansi, daftar nama yang tidak lolos kurasi beserta alasannya dapat dilihat di `daftar-tokoh-tereliminasi.txt`.

## Kebijakan Kurasi Tokoh

Untuk menjaga standar kualitas dan kedalaman intelektual direktori ini, setiap tokoh yang didaftarkan harus memenuhi kriteria berikut:

1.  **Warisan Intelektual (Intellectual Legacy)**: Memiliki karya tulis (buku/artikel), teori, konsep orisinal, atau kontribusi pemikiran yang fundamental dan diakui di bidangnya.
2.  **Substansi di Atas Popularitas**: Fokus pada bobot pemikiran, bukan sekadar popularitas atau pengaruh media sosial. Proyek ini memprioritaskan profil "intelektual" daripada "selebritas".
3.  **Integritas & Etika**: Tokoh yang didaftarkan wajib memiliki rekam jejak moral yang bersih. Kami secara ketat mengevaluasi dan tidak menyertakan profil tokoh yang memiliki catatan terverifikasi terkait korupsi, pelecehan seksual, atau tindak kriminal berat lainnya yang mencederai martabat kemanusiaan dan intelektualitas.
4.  **Verifikasi Sumber**: Setiap klaim fakta dan pokok pikiran wajib menyertakan rujukan kredibel (jurnal akademik, buku, atau media massa otoritatif).
5.  **Inklusivitas Bidang**: Mencakup berbagai disiplin ilmu mulai dari filsafat, sains, teknologi, hukum, agama, hingga seni dan kebudayaan.

## Aturan Verifikasi Sumber

Untuk menjaga kredibilitas, setiap data **WAJIB** menyertakan rujukan:
- **Sumber daring**: URL jurnal, berita, atau ensiklopedia terpercaya.
- **Sumber cetak**: Jika tidak ada versi daring, kontributor diminta menyertakan foto/pindaian halaman terkait yang diunggah ke `assets/bukti/`.

## Teknologi

- **Static Site Generator:** [Jekyll](https://jekyllrb.com/)
- **Visualisasi:** [Chart.js](https://www.chartjs.org/)
- **Hosting:** GitHub Pages
- **Lisensi:** Creative Commons Zero v1.0 Universal (CC0 1.0) - *Public Domain*

## Cara Berkontribusi

Kami mengundang siapa pun untuk berkontribusi menambahkan profil tokoh:

1. **Fork** repositori ini.
2. **Buat file baru** di folder `_tokoh/` mengikuti format yang ada.
3. **Commit & Push** perubahan Anda.
4. Buat **Pull Request**.

Setiap perubahan pada file Markdown akan secara otomatis memperbarui grafik, linimasa, dan data JSON saat situs dibangun kembali.

---

**Mari abadikan pemikiran anak bangsa.**

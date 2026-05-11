# Belajar-Github

1. Pentingnya Penggunaan Command Line
Mengapa tidak menggunakan aplikasi klik-klik saja? Berikut alasannya:

-Efisiensi & Kecepatan: Mengetik perintah seringkali lebih cepat daripada menavigasi berbagai menu di GUI.

-Akses Fitur Lengkap: Beberapa perintah tingkat lanjut (seperti rebasing kompleks atau stashing spesifik) lebih mudah dikelola via CLI.

-Otomatisasi: Perintah CLI dapat dimasukkan ke dalam script untuk otomatisasi tugas (CI/CD).

-Standar Industri: Hampir semua server (Linux) dioperasikan melalui command line. Membiasakan diri di lokal akan memudahkan pengelolaan server nantinya.


2. Langkah-Langkah Push Repository
<img src = "/images/gitpush.png">
Fungsi: Mengirimkan perubahan kode dari komputer lokal (Local Repository) ke server pusat (Remote Repository seperti GitHub/GitLab).

Langkah-langkah:

-Inisialisasi (Jika folder baru): git init

-Menambah Remote: git remote add origin [URL_REPO]

-Memasukkan Perubahan: git add . (tanda titik berarti semua file).

-Memberi Catatan: git commit -m "Pesan commit kamu"

-Mengirim: git push origin [nama_branch] (biasanya main atau master).

3. Langkah-Langkah Clone Repository
<img src = "/images/gitclone.png/">
<img src = "/images/cd.png/">
Fungsi: Menyalin repositori yang sudah ada di server (Remote) ke komputer lokal untuk pertama kalinya.

-Langkah-langkah:

-Buka terminal di folder tujuan.

-Gunakan perintah:
git clone [URL_REPO]

-Git akan otomatis membuat folder dengan nama repo tersebut dan mengunduh seluruh sejarah versinya.


4. Langkah-Langkah Pull dan Push (Workflow Rutin)
<img src = "/images/pull.png/">
<img src = "/images/cd.png/">
Fungsi: Ini adalah alur kerja harian. Pull dilakukan untuk mengambil update terbaru dari rekan tim agar tidak terjadi konflik, sedangkan Push untuk mengirim hasil kerja kita.

Langkah-langkah Ideal:

-Pull Terlebih Dahulu: Pastikan kode lokalmu paling mutakhir.
git pull origin [nama_branch]

-Lakukan Perubahan: Edit kodingan kamu di text editor.

-Stage & Commit:
git add .
git commit -m "Penjelasan perubahan"

-Push Kembali:
git push origin [nama_branch]

-Catatan Penting: Selalu lakukan git pull sebelum bekerja atau sebelum push untuk menghindari merge conflict yang memusingkan!
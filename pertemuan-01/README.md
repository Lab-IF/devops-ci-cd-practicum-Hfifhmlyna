Laporan Praktikum DevOps - Modul 01: Implementasi Docker Dasar
Nama: Hafifa Mulyana

NIM: 105841104123

Topik: Kontainerisasi Web Server Statis

Pemahaman Konsep Kontainerisasi
Praktikum ini bertujuan untuk memahami bagaimana Docker mengubah cara kita mengelola aplikasi. Secara tradisional, kita harus menginstal web server secara manual di sistem operasi, namun dengan Docker, kita menggunakan konsep Isolation (Isolasi).

Beberapa keunggulan utama yang dipelajari dalam praktikum ini:

Standarisasi Lingkungan: Docker memastikan bahwa aplikasi berjalan dalam kondisi yang sama, baik di laptop pengembang maupun di server produksi, sehingga meminimalkan risiko "error lingkungan".

Layered File System: Setiap instruksi dalam Dockerfile membentuk lapisan (layer) yang efisien, sehingga proses build berikutnya bisa berjalan lebih cepat berkat adanya caching.

Manajemen Resource: Kontainer tidak memerlukan sistem operasi utuh untuk berjalan, melainkan hanya membutuhkan base image minimalis seperti Alpine Linux yang ukurannya sangat kecil dan ringan.

Di dunia industri, teknologi ini memungkinkan perusahaan seperti Airbnb untuk meluncurkan ratusan layanan baru secara mandiri tanpa saling mengganggu. Docker menjadi pondasi utama sebelum kita melangkah ke tahap otomatisasi yang lebih kompleks seperti CI/CD Pipeline.

Dokumentasi Aktivitas Praktikum
Berdasarkan pengujian yang telah saya lakukan, berikut adalah rincian teknisnya:

Konfigurasi Dockerfile: Saya membuat instruksi untuk menggunakan nginx:alpine sebagai basis dan menyalin file index.html ke direktori default server Nginx.

Proses Build: Menggunakan perintah docker build -t praktikum-docker:v1 . untuk menciptakan image lokal dengan nama tag tertentu.

Deployment Kontainer: Kontainer dijalankan dengan nama praktikum-hafifa menggunakan port mapping -p 8080:80.

Verifikasi Sistem: Pemeriksaan melalui perintah docker ps menunjukkan kontainer telah aktif (Up) dengan ID 98d081633b1c.

Hasil Akhir: Aplikasi web statis telah berhasil dijalankan di dalam kontainer terisolasi dan dapat diakses melalui browser pada alamat http://localhost:8080.

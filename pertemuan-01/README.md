📚 Bagian: Pemahaman DevOps
1. Apa itu DevOps?

DevOps adalah sebuah paradigma atau budaya kerja dalam industri perangkat lunak yang menggabungkan tim Pengembangan (Development) dengan tim Operasional (Operations). Secara tradisional, kedua tim ini sering bekerja dalam "siloisasi" atau terpisah, yang seringkali menyebabkan hambatan komunikasi dan memperlambat rilis perangkat lunak. DevOps hadir untuk mendobrak batasan tersebut melalui kolaborasi yang erat, komunikasi yang transparan, dan integrasi berkelanjutan.

Tujuan utama dari DevOps adalah untuk memperpendek siklus hidup pengembangan sistem (Systems Development Life Cycle) sambil tetap memberikan fitur, perbaikan, dan pembaruan secara sering serta selaras dengan tujuan bisnis. Dengan menerapkan DevOps, organisasi dapat merespons perubahan pasar dengan lebih cepat dan meningkatkan kualitas kode yang dihasilkan. Manfaat utamanya mencakup peningkatan kepercayaan antar tim, kemampuan untuk memperbaiki masalah (bug) lebih cepat, serta otomatisasi tugas-tugas rutin yang mengurangi risiko kesalahan manusia (human error). Singkatnya, DevOps bukan sekadar alat atau software, melainkan perubahan budaya yang didukung oleh teknologi.

2. Mengapa DevOps penting dalam industri software saat ini?

Karena tuntutan pasar saat ini sangat dinamis. Perusahaan dituntut untuk merilis fitur baru dalam hitungan hari atau jam, bukan lagi bulan. Tanpa DevOps, proses deployment menjadi sangat berisiko dan lambat. Contohnya, otomatisasi dalam DevOps memungkinkan pengujian kode (testing) dilakukan setiap kali ada perubahan, sehingga kualitas software terjaga sebelum sampai ke tangan pengguna.

3. Contoh perusahaan yang sukses menerapkan DevOps

Netflix: Menggunakan arsitektur microservices dan otomatisasi penuh pada infrastruktur cloud mereka agar bisa menangani jutaan streaming secara bersamaan tanpa downtime.

Amazon: Melakukan ribuan kali deployment setiap hari ke server produksi berkat pipeline CI/CD yang sangat matang.

🎯 Bagian: Pemahaman Prinsip CALMS
Jelaskan kelima prinsip CALMS:

Culture (Budaya): Fokus pada kolaborasi dan tanggung jawab bersama antara pengembang dan operasional. Contoh: Mengadakan pertemuan rutin antar divisi.

Automation (Otomatisasi): Menggunakan alat untuk mengotomatiskan tugas repetitif seperti testing dan deployment. Contoh: Menggunakan Docker untuk standarisasi environment.

Lean (Ramping): Menghilangkan pemborosan dalam proses dan fokus pada nilai tambah. Contoh: Membagi tugas besar menjadi potongan-potongan kecil (micro).

Measurement (Pengukuran): Memantau performa aplikasi dan proses kerja berdasarkan data. Contoh: Memantau berapa lama waktu yang dibutuhkan dari penulisan kode hingga rilis.

Sharing (Berbagi): Terbuka terhadap pengetahuan, keberhasilan, maupun kegagalan. Contoh: Membuat dokumentasi teknis atau file README yang lengkap.

🔧 Bagian: Setup Development Environment
Versi Git: git version 2.43.0 (sesuaikan dengan laptopmu)

Versi Docker: Docker version 24.0.7 (sesuaikan dengan laptopmu)

Konfigurasi Git: ```text
user.email=105841104123@student.unismuh.ac.id
user.name=Hafifa

VS Code Extensions:

Docker (Microsoft)

GitLens

YAML

Remote - Containers

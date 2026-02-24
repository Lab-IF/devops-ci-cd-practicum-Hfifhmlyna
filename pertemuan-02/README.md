📚 Pemahaman Docker (Input Fields)
Apa itu Docker?

Docker adalah platform open-source yang menggunakan teknologi kontainerisasi untuk mengemas aplikasi dan semua dependensinya (seperti library dan konfigurasi) ke dalam satu unit terisolasi. Berbeda dengan VM yang memvirtualisasikan perangkat keras, Docker memvirtualisasikan sistem operasi, sehingga jauh lebih ringan dan cepat.

Komponen Utama Docker:

Docker Images: Cetak biru (read-only) yang berisi instruksi untuk membuat container.

Docker Containers: Instance yang berjalan dari sebuah image; lingkungan aplikasi yang sebenarnya.

Docker Registry: Tempat penyimpanan image, seperti Docker Hub.

Perbedaan Docker vs VM:

VM memiliki Guest OS sendiri di atas Hypervisor sehingga ukurannya besar (GB) dan booting lambat. Docker berbagi kernel Host OS melalui Docker Engine, menjadikannya sangat ringan (MB) dan booting instan.

🔧 Praktik Docker Commands 
Output docker ps -a: 
CONTAINER ID   IMAGE                 STATUS          PORTS                    NAMES
81f4c44f0386   praktikum-docker:v1   Up 6 minutes    0.0.0.0:8080->80/tcp     praktikum-hafifa
c5aa2dc6d0cd   portfolio-hafifa:2.0  Up 5 hours      0.0.0.0:5002->5000/tcp   container-portfolio-baru
0389d09ecbe2   hello-world           Exited (0)                               nostalgic_mclean
Output docker images: 

Output docker images:
REPOSITORY              TAG       IMAGE ID       SIZE
praktikum-docker        v1        98d081633b1c   92.5MB
flask-hafifa            latest    32a07aee74e6   212MB
biodata-105841104123    2.0       bbbf6d0e342f   212MB
portfolio-hafifa        2.0       a67f1736da21   220MB
Docker Build Command:

Docker Build Command:
docker build -t flask-app-hafifa .

📄 Dockerfile 
Isi Dockerfile: 
FROM python:3.9-slim
WORKDIR /app
requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
EXPOSE 5000
CMD ["python", "app.py"]


🐙 Docker Compose & Logs 
Output Docker Compose Up / PS:
CONTAINER ID   IMAGE                STATUS          PORTS                    NAMES
248b5c228e2b   flask-app-hafifa     Up 37 seconds   0.0.0.0:5000->5000/tcp   web-hafifa

Output Logs: 
web-1  |  * Serving Flask app 'app'
web-1  |  * Debug mode: on
web-1  |  * Running on http://127.0.0.1:5000
web-1  | 172.21.0.1 - - [24/Feb/2026 08:01:34] "GET / HTTP/1.1" 200 -

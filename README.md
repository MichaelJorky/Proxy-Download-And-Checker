# Proxy Download And Checker

> **Peringatan:** :red_circle: Alat ini dibuat khusus untuk keperluan pendidikan dan penelitian. Penulis tidak bertanggung jawab atas segala bentuk penyalahgunaan atau kerusakan yang mungkin timbul dari penggunaan program ini. Harap gunakan dengan bijak dan hanya di lingkungan di mana Anda memiliki izin eksplisit.

Proxy Download dan Checker dengan Judge Proxy adalah tools atau program yang digunakan untuk mengunduh daftar proxy dari berbagai sumber (proxy download) dan memeriksa validitas proxy tersebut (proxy checker) dengan bantuan Judge Proxy. Berikut penjelasan masing-masing istilah:

1. Proxy Download

- Proxy Download adalah proses mendapatkan daftar proxy dari sumber online, seperti website yang menyediakan daftar proxy secara gratis atau berbayar.
- Proxies biasanya berupa alamat IP dan port, misalnya: 192.168.1.1:8080.
- Proxy digunakan untuk routing koneksi internet, menyembunyikan IP asli, atau mengakses konten yang dibatasi berdasarkan lokasi.

2. Proxy Checker

- Proxy Checker adalah program untuk memeriksa apakah proxy dalam daftar masih aktif dan dapat digunakan.
- Proses ini mencakup:
  - Memeriksa apakah proxy bisa dihubungi (connectivity check).
  - Menguji kecepatan proxy (response time).
  - Mengecek tingkat anonimitas (transparent, anonymous, atau elite).
  - Validasi proxy untuk protokol tertentu (HTTP, HTTPS, SOCKS4, SOCKS5).

3. Judge Proxy

- Judge Proxy adalah server atau endpoint yang digunakan untuk menguji bagaimana proxy berfungsi.
- Saat proxy digunakan untuk mengakses Judge Proxy, server ini memberikan laporan yang berisi:
  - IP yang terlihat (visible IP): apakah proxy benar-benar menyembunyikan IP asli Anda.
  - Headers yang diterima: untuk mengetahui apakah proxy mengungkapkan informasi tambahan (misalnya, IP asli di header X-Forwarded-For).
  - Status koneksi: apakah proxy dapat meneruskan request ke server.

Judge Proxy sangat penting untuk menentukan tingkat anonimitas proxy:

- Transparent Proxy: Mengungkapkan IP asli pengguna.
- Anonymous Proxy: Menyembunyikan IP asli tetapi mengungkapkan bahwa Anda menggunakan proxy.
- Elite Proxy: Tidak mengungkapkan IP asli maupun keberadaan proxy.

Contoh Alur Kerja Proxy Download dan Checker:

1. Download Daftar Proxy:
- Program mengambil daftar proxy dari sumber online atau file lokal.
- Contoh format proxy: IP:Port, seperti 123.45.67.89:8080.

2. Mengirim Request melalui Proxy:
- Setiap proxy diuji dengan mengakses Judge Proxy.
- Contoh Judge Proxy: example-judge.com.

3. Menganalisis Respon:
- Judge Proxy menganalisis request untuk memeriksa apakah proxy aktif, tingkat anonimitasnya, dan kecepatan koneksi.

4. Menyimpan Hasil:
- Proxy yang valid disimpan ke dalam daftar, biasanya berdasarkan kategori (anonymous, elite, atau lainnya).

Kegunaan:

- Web Scraping: Untuk menyembunyikan IP dan menghindari pembatasan dari server target.
- Bypass Geo-blocking: Mengakses konten yang dibatasi berdasarkan lokasi geografis.
- Anonimitas: Menyembunyikan alamat IP asli saat berselancar di internet.

~ (v1.0.0.1) Senin 16 Desember 2024 - First Release Proxy Download & Checker

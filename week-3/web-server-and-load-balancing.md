# Task Week 3

## Web Server & Load Balancing

1. Jelaskan apa itu web server dan gambarkan bagaimana cara webserver bekerja.

   Web server itu seperti rumah di internet tempat menyimpan dan menyajikan halaman web. Bayangkan web server seperti pelayan di restoran yang menyajikan makanan kepada pelanggan. Ketika Anda mengetik alamat situs web di peramban web Anda, seperti Google.com, permintaan Anda dikirim ke web server. Web server kemudian menyiapkan halaman web yang diminta dan mengirimkannya kembali ke peramban Anda agar Anda bisa melihatnya.

Proses kerjanya seperti ini: Ketika seseorang meminta halaman web, peramban web mereka mengirim permintaan ke web server. Web server kemudian menemukan halaman yang diminta, seperti halaman depan situs web, mengumpulkannya, dan mengirimkannya kembali ke peramban pengguna. Kemudian peramban web menampilkan halaman web tersebut kepada pengguna.

Jadi intinya, web server adalah tempat di internet tempat halaman web disimpan dan disajikan kepada pengguna saat mereka memintanya.

2. Buatlah reverse proxy untuk aplilkasi wayshub-frontend yang telah di deploy dan untuk domain sesuaikan dengan nama anda ex: alvin.xyz
   
   Cek status nginx kemudian buat direktori baru pada /etc/nginx lalu buat sebuah file konfigurasi reverse proxy
   
   ![RP 1](screenshots/6.png)

   ![RP 2](screenshots/7.png)
   
   Kembali ke direktori /etc/nginx lalu edit file nginx.conf dengan menambahkan direktori yang berisi file konfigurasi reverse proxy yang telah dibuat
   
   ![RP 3](screenshots/8.png)
   
   ![RP 4](screenshots/9.png)
   
   Cek apakah file konfigurasi terdapat masalah atau tidak kemudian restart nginx jika tidak ada masalah
   
   ![RP 5](screenshots/10.png)
   
   Selanjutnya membuat virtual host dengan kembali ke server lokal untuk mejalankan sudo nano /etc/hosts
   
   ![RP 6](screenshots/11.png)
   
   Tambahkan alamat IP serta domain dari reverse proxy yang telah dibuat sebelumnya
   
   ![RP 7](screenshots/12.png)
   
   Kemudian kembali masuk ke server reverse proxy untuk menjalankan command npm start pada direktori aplikasi
   
   ![RP 8](screenshots/13.png)
   
   Dan akhirnya frontend dari aplikasi wayshub dapat diakses dengan domain afifsuryaaa.xyz pada web
   
   ![RP 9](screenshots/14.png)

3. Jelaskan apa itu load balance.

   Suatu proses untuk membantu memastikan situs web tetap stabil dan cepat meskipun ada banyak pengguna yang mengaksesnya dengan cara membagi lalu lintas web ke beberapa server sehingga setiap server tidak terlalu sibuk dan situs web tetap dapat diakses dengan cepat sekalipun banyak yang mengaksesnya.

4. implementasikan load balancing kepada aplikasi wayshub-frontend yang telah anda gunakan.

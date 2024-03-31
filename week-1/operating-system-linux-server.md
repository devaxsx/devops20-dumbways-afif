# Operating System & Linux Server

1. Cari perbedaan antara distro Ubuntu dan CentOS!
Ubuntu: berbasis debian, sering update, lebih mudah dipahami pemula.
CentOS: berbasis RHEL, jarang update, lebih susah dipahami pemula.

2. Apa perbedaan dari CLI & GUI?
CLI: Interface berupa teks; tidak user friendly; memerlukan sedikit resource.
GUI: Interface berupa gambar, ikon, dsb; user friendly; memerlukan banyak resource.


3. Di VM masing-masing :
    - Install nginx, lalu akses melalui browser/`curl <ip kalian>`
    ![Install Nginx](screenshots/nginx_1.jpg)

    ![Nginx via URL](screenshots/nginx_2.jpg)

    - Ganti IP address kalian (bebas) lalu akses kembali nginx (`/etc/netplan`)
    ![Change IP & Re-access Nginx 1](screenshots/nginx_3.jpg)

    ![Change IP & Re-access Nginx 2](screenshots/nginx_4.jpg)

    ![Change IP & Re-access Nginx 3](screenshots/nginx_5.jpg)

    ![Change IP & Re-access Nginx 4](screenshots/nginx_6.jpg)

4. Terangkan fungsi systemctl dan contoh commandnya (gunakan nginx)
![Systemctl](screenshots/nginx_7.jpg)

Systemctl berfungsi untuk meng on/off kan ataupun mengecek status suatu layanan
semisal pada contoh diatas adalah untuk cek status nginx aktif atau tidak.

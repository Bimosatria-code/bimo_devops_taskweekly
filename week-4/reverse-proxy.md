# Dokumentasi Cara Membuat Reverse Proxy
Berikut adalah dokumentasi proses pembuatan dari setiap aplikasi:

## Langkah-langkah reverse proxy dan pembuatan domain Aplikasi Nodejs
### Pertama masuk kedalam folder /etc/nginx, kemudian buat sebuah direktori untuk menjadi tempat untuk file domain. lalu buat file nodejs.bimo.xyz, berikut perintah-perintahnya:
- cd /etc/nginx
- mkdir domain
- cd domain
- sudo nano nodejs.bimo.xyz
- ![gambar domain 1](assets/nodejsdomain-1.png)

- sudo nginx -t
- ![gambar domain 2](assets/nodejsdomain-2.png)

### Dan setelah itu kita edit file nginx.conf didalamnya kita masukkan include /etc/nginx/domain/*;
- sudo nano nginx.conf
- ![gambar domain 3](assets/nodejsdomain-6.png)

### Kemudian kita buat virtual host di local kita dan masukkan ip dan nama domainnya, berikut perintah-perintahnya;
- sudo nano /etc/hosts
- ![gambar domain 4](assets/nodejsdomain-3.png)
- sudo systemctl reload nginx
- ![gambar domain 5](assets/nodejsdomain-5.png)

### Terakhir masuk kedalam folder app-nodejs dan jalankan node index.js. Setelah aplikasi berjalan kita buka domain pada browser, berikut perintah-perintahnya;
- cd ~/Dumbways/app-nodejs
- node index.js
- ![gambar domain 4](assets/nodejsdomain-4.png)



## Langkah-langkah reverse proxy dan pembuatan domain Aplikasi Python
### Pertama masuk kedalam folder /etc/nginx, kemudian masuk kedalam direktori domain lalu buat file python.bimo.xyz, berikut perintah-perintahnya:
- cd /etc/nginx
- cd domain
- sudo nano python.bimo.xyz
- ![gambar py domain 1](assets/pythondomain-1.png)
- ![gambar py domain 2](assets/pythondomain-2.png)

### Setelah selesai save dan buat virtual host dilocal kita. Didalamnya kita isikan ip dan nama domain kita, berikut perintahnya:
- sudo nano /etc/hosts
- ![gambar py domain 3](assets/pythondomain-4.png)
- sudo systemctl reload nginx

### Langkah berikutnya kita pindah direktori ke cd ~/Dumbways/app-nodejs dan jalankan index.py, berikut perintahnya:
- cd ~/Dumbways/app-python
- python3 index.py
- ![gambar py domain 4](assets/pythondomain-5.png)

### Terakhir buka pada browser domainnya python.bimo.xyz
- ![gambar py domain 5](assets/pythondomain-6.png)


## Langkah-langkah reverse proxy dan pembuatan domain Aplikasi Golang
### Pertama masuk kedalam folder /etc/nginx, kemudian masuk kedalam direktori domain lalu buat file golang.bimo.xyz, berikut perintah-perintahnya:
- cd /etc/nginx
- cd domain
- sudo nano golang.bimo.xyz
- ![gambar go domain 1](assets/golangdomain-1.png)
- ![gambar go domain 2](assets/golangdomain-2.png)

### Setelah selesai save dan buat virtual host dilocal kita. Didalamnya kita isikan ip dan nama domain kita, berikut perintahnya:
- sudo nano /etc/hosts
- ![gambar go domain 3](assets/golangdomain-4.png)
- sudo systemctl reload nginx

### Langkah berikutnya kita pindah direktori ke cd ~/Dumbways/app-golang dan jalankan go run index.go kemudian build dengan go build index.go, berikut perintahnya:
- cd ~/Dumbways/app-golang
- go run index.go
- go build index.go
- ./index
- ![gambar go domain 4](assets/golangdomain-5.png)

### Terakhir buka pada browser domainnya golang.bimo.xyz
- ![gambar go domain 5](assets/golangdomain-6.png)

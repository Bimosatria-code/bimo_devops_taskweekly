# Dokumentasi Membuat aplikasi nodejs, python3 dan golang
Berikut adalah dokumentasi proses pembuatan dari setiap aplikasi:

## Langkah-langkah installasi Nodejs
### Pertama langkah installasi dengan memasukkan perintah-perintah berikut satu per satu:
- curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
- ![gambar install nodejs 1](assets/nodejs-9.png)

- nvm install 16.13.0
- nvm use 16
- ![gambar install nodejs 2](assets/nodejs-10.png)

### Berikutnya setelah langkah installasi selesai, untuk melakukan pengecekan masukkan perintah-perintah berikut satu per satu:
- node -v
- npm -v
- ![gambar cek versi nodejs dan npm](assets/nodejs-11.png)

### Jika nvm belum terdeteksi, masukkan perintah-perintah berikut:
- exec bash
- exec zsh

### Kemudian langkah-langkah pembuatan aplikasi, masukkan perintah-perintah berikut:
- mkdir app-nodejs
- cd app-nodejs
- npm init -y
- ![gambar membuat aplikasi nodejs](assets/nodejs-12.png)

### Kemudian buka file package.json dengan nano kemudian tambahkan perintah start pada script, berikut contohnya:
- nano package.json
- ![gambar membuat aplikasi nodejs](assets/nodejs-15.png)

### lalu setelah itu install express, masukkan perintah berikut:
- npm install express -y
- ![gambar install package express nodejs](assets/nodejs-13.png)

### lalu setelah install express selanjutnya adalah membuat file index.js dimana didalamnya adalah berisi code aplikasi yg akan dijalankan, masukkan perintah berikut untuk membuat index.js:
- nano index.js
- ![gambar buat file index.js nodejs](assets/nodejs-14.png)

### lalu setelah itu simpan file dan jalankan perintah berikut untuk menjalankan aplikasinya:
- node index.js
- ![gambar menjalankan aplikasi nodejs](assets/nodejs-16.png)

### Kemudian terakhir jalankan pada web browser: http://localhost:3000
- ![gambar membuka aplikasi dibrowser nodejs](assets/nodejs-17.png)


## Langkah-langkah installasi Python3
### Pertama langkah installasi dengan memasukkan perintah-perintah berikut satu per satu:
- sudo apt update
- sudo apt upgrade -y
- python3 -V
- sudo apt install python3-pip
- pip install flask

### Kemudian langkah selanjutnya setelah installasi selesai kita masuk ketahap pembuatan aplikasi, dengan memasukkan perintah-perintah berikut satu per satu:
- mkdir app-python
- cd app-python
- nano index.py
- ![gambar membuat aplikasi python3](assets/python-2.png)
- ![gambar membuat aplikasi python3 2](assets/python-1.png)

### Lalu untuk menjalankannya masukkan perintah berikut:
- python3 index.py
- ![gambar menjalankan aplikasi python3](assets/python-4.png)

### Kemudian terakhir jalankan pada web browser: http://localhost:5000
- ![gambar membuka aplikasi dibrowser python3](assets/python-3.png)


## Langkah-langkah installasi Golang
### Pertama langkah installasi dengan memasukkan perintah-perintah berikut satu per satu:
- wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
- ![gambar download golang](assets/go-1.png)

- rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit
- export PATH=$PATH:/usr/local/go/bin
- go version
- ![gambar installasi golang](assets/go-2.png)

### Berikutnya setelah installasi selesai kita masuk ketahap pembuatan aplikasinya, dengan memasukkan perintah-perintah berikut:
- mkdir app-golang
- cd app-golang
- nano index.go
- ![gambar membuat aplikasi golang](assets/go-3.png)
- ![gambar membuat aplikasi golang](assets/go-4.png)

### Kemudian tahap terakhir kita jalankan aplikasi golang, dengan perintah berikut:
- go run index.go
- go build index.go
- ./index.go
- ![gambar membuat aplikasi golang](assets/go-5.png)


# Addition
## langkah2 install pm2
### Pertama kita install pm2 secara global. berikut perintahnya:
- npm install pm2 -g
- ![gambar pm2 install](assets/pm2.png)

### Kemudian setelah itu ketik perintah $pm2 ecosystem simple untuk mendapatkan config ecosystem dan setelah itu edit file ecosystem.config.js, kemudian save lalu jalankan pm2 start, berikut perintahnya:
- pm2 ecosystem simple
- sudo nano ecosystem.config.js
- pm2 start
- ![gambar pm2 ecosystem](assets/pm2-start.png)

### Terakhir untuk melihat list aplikasi yg sudah kita jalankan dengan pm2 kita bisa menggunakan perintah berikut:
- pm2 list
- ![gambar pm2 list](assets/pm2-list.png)

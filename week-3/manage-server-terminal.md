# Dokumentasi Manage Server With Terminal
Berikut adalah dokumentasi cara memanage server dengan terminal:

## Manipulasi Text dengan Text Editor Nano
### Nano adalah sebuah text editor yang biasa digunakan diterminal untuk mengedit text, berikut short key dalam text editor nano:
- ctrl + X = digunakan untuk exit dan juga untuk mensave file
![gambar CTRL+X](assets/nano-ctrlx.png)
- alt + A = digunakan untuk memasuki mode select
![gambar ALT+A](assets/nano-altA.png)
- ctrl + U = digunakan untuk paste
- ctrl + K = digunakan untuk memotong / cut
- ctrl + A = digunakan untuk pindah kursor ke awal baris
![gambar CTRL+A](assets/nano-ctrlA.png)
- ctrl + E = digunakan untuk pindah kursor ke belakang baris
![gambar CTRL+E](assets/nano-ctrlE.png)
- ctrl + W = digunakan untuk search
![gambar CTRL+W](assets/nano-ctrlW.png)

## Manipulasi Text CAT
### Cat adalah salah satu perintah yang berfungsi untuk membuat daftar konten atau isi file,berikut contoh penggunaan:
- cat nama-file : untuk melihat isi file
![gambar CTRL+W](assets/cat-lihat.png)
- cat > nama-file : untuk membuat file baru
![gambar CTRL+W](assets/cat-membuat.png)
- cat file1 file2 > file3 : untuk menggabungkan isi file
![gambar CTRL+W](assets/cat-gabung.png)

## Manipulasi Text SED
### Sed adalah singkatan dari stream editor. Gunanya untuk memanipulasi teks dasar pada file. dengan sed kita dapat mengganti string pada sebuah file, berikut contoh penggunaannya:
- sed -i 's/aku/saya/g' file.txt
![gambar sed](assets/sed.png)

## Manipulasi Text GREP
### Grep adalah perintah untuk pencarian sebuah string pada suatu file, berikut contoh penggunaannya:
- grep belajar file.txt
![gambar grep](assets/grep.png)

## Manipulasi Text SORT
### Sort adalah perintah untuk mengurutkan data baik secara ascending maupun descending, berikut contoh penggunaannya:
- sort nama-file
![gambar grep](assets/sort.png)

## Manipulasi Text ECHO
### Echo adalah perintah untuk mencetak string / pesan dari hasil perintah lain, berikut contoh penggunaannya:
- echo "aku sudah mempelajari CI/CD" >> file3.txt
![gambar echo](assets/echo.png)

## Manipulasi Text DIFF
### Diff adalah perintah untuk membandingkan konten dalam file, berikut contoh penggunaannya:
- diff file1.txt file2.txt
![gambar diff](assets/diff.png)


## Monitoring
### Monitoring merupakan aktivitas untuk melihat kinerja sistem:

### Htop merupakan perintah untuk memonitoring sistem, kita dapat melihat penggunaan memory, cpu, swap. Berikut contoh penggunaan:
- $ htop
![gambar htop](assets/htop.png)

### Lsof merupakan perintah untuk melihat seluruh file yg terbuka berdasarkan proses aktif yang berjalan disistem. Berikut contoh penggunaan:
- $ lsof
![gambar lsof](assets/lsof.png)

### Ps perintah untuk melaporkan snapshot dari proses saat ini. Berikut contoh penggunaan:
- $ ps
![gambar ps](assets/ps.png)
- $ ps-aux
![gambar ps-aux](assets/ps-aux.png)
- $ ps -f -u bimo
![gambar ps-u](assets/ps-u.png)

### Nmon adalah alat monitoring untuk menampilkan informasi tentang berbagai sumber daya sistem seperti cpu, memori, disk, djaringan dan lain2. Berikut contoh penggunaan:
- $ nmon
![gambar nmon](assets/nmon-home.png)
- klik C
![gambar nmon CPU](assets/nmon-cpu.png)
- klik d
![gambar nmon disk](assets/nmon-cpu-disk.png)

### Network Firewall adalah merupakan perintah untuk mengamankan sebuah server.
#### UFW adalah Uncomplicated Firewall atau bentuk penyederhaan dari fitur frontend iptables untuk menkonfigurasi firewall, berikut cara setting menggunakan ufw:

- $ sudo ufw default deny incoming
- $ sudo ufw default allow outgoing
![gambar default](assets/default-allow-deny.png)

- $ sudo ufw allow "OpenSSH"
- $ sudo ufw deny "OpenSSH"
![gambar allow-deny](assets/firewaLL-rules-allow-deny.png)

- $ sudo ufw enable
- $ sudo ufw disable
![gambar enable-disable](assets/firewaLL-enable.png)

- $ sudo ufw delete allow "Nginx Full"
- $ sudo ufw delete deny "Nginx Full"
![gambar delete](assets/firewaLL-delete.png)

- $ sudo ufw  allow 80/tcp
- $ sudo ufw  deny 80/tcp
![gambar port](assets/firewaLL-port.png)
# Installasi Linux Ubuntu Server di Virtual Box
Berikut adalah proses installasi Linux di Virtual Machine:

## Pertama 
![gambar 1](assets/install-1.png)
### Siapkan aplikasi Virtual Box dan iso file ubuntu yg sudah didownload. Kemudian buka aplikasi Virtual box dan Klik NEW 

## Kedua 
![gambar 2](assets/install-2.png)
### Kemudian akan muncul module dan isikan dengan nama,type dan versi OS yg akan diinstall. sesuaikan dengan spesifikasi laptop anda,lalu klik next.

## Ketiga 
![gambar 3](assets/install-3.png)
### Pada bagian Memori Size, anda bisa mengatur seberapa besar memori yg akan digunakan. Namun jika terlalu besar akan membuat perangkat laptop anda menjadi sedikit lambat, maka disarankan menggunakan memori setengah dr memory keseluruhan anda. Jika sudah klik next.

## Keempat 
![gambar 4](assets/install-4.png)
### Kemudian pada bagian HardDisk, Anda dapat membuat hard disk virtual, lalu klik next.

## Kelima 
![gambar 5](assets/install-5.png)
### Ada banyak tipe hard disk virtual, disini kita menggunakan VDI (VirtualBox Disk Image) yaitu tipe standard yang digunakan VirtualBox, lalu klik next.

## Keenam 
![gambar 6](assets/install-6.png)
### Selanjutnya, kita memilih penyimpanan fisik pada hard disk. Disini kita menggunakan Dynamic Allocated, lalu klik next.

## Ketujuh 
![gambar 7](assets/install-7.png)
### Tentukan lokasi penempatan virtual hard disk Anda sekarang beserta ukurannya. Jangan lupa klik Create.

## Kedelapan 
![gambar 8](assets/install-8.png)
### Setelah selesai, kemudian langkah selanjutnya klik setting lalu pilih storage dan klik pada gambar disk bertuliskan empty dan search iso yg sudah didownload dengan mengklik gambar disk biru dikanan. setelah file iso sudah dipilih klik ok.

## Kesembilan 
![gambar 9](assets/install-9.png)
### kemudian klik start dan ketika tampil pilih bahasa sesuai dengan yg kamu inginkan, disarankan memilih bahasa English. lalu tekan enter.

## Kesepuluh 
![gambar 10](assets/install-10.png)
### Kemudian pada Keyboard Configuration pilih sesuai yg kamu inginkan, tapi disarankan memilih English(US) pada bagian Layout dan variant. lalu pilih done dan enter.

## Kesebelas 
![gambar 11](assets/install-18.png)
### Kemudian pada bagian Network Connection kita bisa setup ip kita sendiri, pilih enp0se3 lalu pilih manual dan isikan ip wifi atau modem kita, lalu isi ip yg ingin kita custom, lalu isi gateway sesuai default gateway milik wifi kita lalu save. dan jika sudah klik done

## Keduabelas 
![gambar 12](assets/install-12.png)
### Kemudian pada Configuration proxy klik done

## Ketigabelas 
![gambar 13](assets/install-13.png)
### Pada bagian storage configuration pilih costum storage layout. lalu klik done.

## Keempatbelas 
![gambar 14](assets/install-14.png)
### lalu buat partisi untuk swap sebesar 2 gb lalu create dan buat lagi partisi untuk ext4 sebesar sisa dr storagenya, lalu create. setelah selesai membuat partisi klik done.

## Kelimabelas 
![gambar 15](assets/install-16.png)
### lalu pada profile setup kita isikan nama, nama server, username, password. ini berguna ketika kita akan memasuki mode root nanti. setelah selesai klik done

## Keenambelas 
![gambar 16](assets/install-17.png)
### lalu pada SSH setup kita pilih done saja. kemudian ubuntu server kita akan diinstall dan kita hanya perlu menunggu sampai proses selesai. ketika proses selesai masukkan username yg sudah dimasukkan tadi beserta passwornya.







# Get Laravel in Docker

Pada repository ini teman-teman yang ingin mengistall aplikasi laravel di dalam  docker container bisa jadikan repository ini menjadi referensi ya!, berikut cara penginstallannya:

### Clone Repository
Pastiin teman-teman harus punya git/github dulu,untuk yang belum punya bisa download klik [link](https://git-scm.com/downloads) ini. Lanjut kalau sudah install bisa langsung clone repo ini.

```bash
  https://github.com/DRY-7717/get-laravel-in-docker-container.git
```
### Build Dockerfilfe / Docker Image
Oke, kalau sudah bisa clone teman-teman bisa buka repositorynya dan jalankan perintah ini:
```bash
  docker compose build
```
Tunggu proses build selesai.

### Menjalankan container
Wokkeh, kalau sudah selesai proses build teman-teman bisa menjalankan perintah ini untuk menjalankan container docker:

```bash
  docker compose up -d
```
Tunggu prosesnya sampai selesai, untuk melihat containernya berjalan atau tidak, teman teman bisa jalankan perintah berikut:

```bash
  docker-compose ls
```
atau,
```bash
  docker container ls
```
### Install Laravel Di Dalam Container
Wokkeh, lanjut teman-teman bisa jalankan perintah ini untuk masuk kedalam containernya:

```bash
  docker-compose exec app bash
```
Lanjut untuk menginstall laravelnya, jalankan perintah ini,disini saya menggunakan laravel versi 10:

```bash
  composer create-project laravel/laravel:^10.0 example-app
```
"example-app" bisa teman-teman ganti namanya sesuai keinginan kalian mau namai apa projectnya.

Wokkeh, kalau sudah teman teman tinggal jalankan perintah ini untuk keluar dari containernya:

```bash
  exit
```
### Memindahkan Seluruh Folder atau File Keluar
Wokkeh kalau sudah keluar dari docker container teman-teman bisa menjalankan perintah ini untuk mengeluarkan folder atau file keluar:

```bash
  docker cp get_laravel_container:/var/www/example-app/. .
```

Wokkeeh proses semua sudah selesai dan aplikasi laravel kalian sudah terinstall.

## Pemberitahuan

Cara ini digunakan buat teman-teman yang tidak ingin menginstall php atau composer di laptop atau pc kalian ya!, tapi kalau sudah ada xampp atau laragon atau sudah install composer di laptop kalian,cukup gunakan itu saja, Mohon maaf kalau ada kesalah pada repository ini. Kalau teman-teman ingin memberi masukan repository ini bisa ajukan issue aja ya! Terima kasih. WOKKKEEEEHHHHHHH!!!!!!!!!


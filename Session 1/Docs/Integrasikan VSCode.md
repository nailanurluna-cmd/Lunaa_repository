# Cara Integrasi VSCode dengan GitHub

### 1. **Buat Akun GitHub**
Buka https://github.com lalu daftar dengan email aktif

### 2. **Buka **Terminal** kemudian Buat Folder**
Jalankan perintah ini di Terminal
```bash
mkdir .ssh
```

### 3. **Generate SSH Key**
Jalankan perintah:
```bash
ssh-keygen -t ed25519 -c "youremail@example.com"
```
Bagian "youremail@example.com" ganti dengan email yang terdaftar **GitHub**.


### 4. **Tentukan Nama File**
Saat diminta nama file, masukkan nama bebas. lalu tekan enter.

### 5. **Generate SSH Key**
Jalankan perintah:
```bash
ssh-keygen -t rsa -b 4096 -C "youremail@example.com"
```
Bagian "youremail@example.com" masukkan nama bebas, lalu tekan enter.

### 6. **Keluar dengan Perintah exit**
Masukkan perintah ini untuk keluar dari proses sebelumnya.
```bash
exit
```

### 7. **Lewati Passphrase**
Saat muncul tulisan *Enter passphrase*, cukup tekan enter dua kali tanpa mengetik apa-apa.

### 8. **Cek Isi Folder**
Jalankan perintah ini untuk memastikan file sudah berhasil dibuat
```bash
ls
```

### 9. **Tampilkan Isi File**
Jalankan perintah ini lalu akan memunculkan kode panjang:
```bash
cat exit.pub
```

### 10. **Salin Kode**
Salin kode panjang tersebut (dimulai dari *ssh-rsa...* sampai alamat email di belakang).

### 11. **Buka Github**
Buka **GitHub**, klik icon profil kanan atas lalu pilih settings

### 12. **Masuk ke Menu SSH and GPG Keys**
Setelah masuk ke menu **SSH and GPG Keys**, klik tombol **New SSH Key** lalu masukkan kode panjang yang sebelumnya sudah disalin. Kemudian klik **Add SSH Key**

### 13. **Verifikasi Via Email**
Jika Github meminta verifikasi, pencet link verifikasi yang muncul.

### 14. **Terakhir, Masukkan Kode Verifikasi**
Cek inbox email, salin kode yang dikirim, lalu masukkan ke Github

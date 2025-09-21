# Cara Instalasi MongoDB di Debian/Ubuntu

Berikut adalah langkah-langkah untuk menginstal MongoDB di Terminal:

1.  **Impor Kunci Publik GPG**
    Jalankan perintah ini untuk menginstal kunci publik MongoDB.
    
    ```bash
    wget -qO - [https://www.mongodb.org/static/pgp/server-6.0.asc](https://www.mongodb.org/static/pgp/server-6.0.asc) | sudo apt-key add -
    ```

2.  **Buat File Daftar Repositori**
    Perintah ini akan membuat file yang memungkinkan sistemmu menemukan paket MongoDB.
    
    ```bash
    echo "deb [ arch=amd64,arm64 ] [https://repo.mongodb.org/apt/ubuntu](https://repo.mongodb.org/apt/ubuntu) focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list
    ```

3.  **Perbarui Daftar Paket**
    Perbarui daftar paket sebelum instalasi.
    
    ```bash
    sudo apt update
    ```

4.  **Instal MongoDB**
    Sekarang, jalankan perintah ini untuk menginstal paket server MongoDB.
    
    ```bash
    sudo apt install mongodb-org
    ```
    Jika diminta konfirmasi, ketik `y` lalu tekan Enter.
    
5.  **Mulai Layanan MongoDB**
    Mulai layanan MongoDB dengan perintah ini.
    
    ```bash
    sudo systemctl start mongod
    ```

6.  **Cek Status MongoDB**
    Untuk memastikan instalasi berhasil, cek statusnya:
    
    ```bash
    sudo systemctl status mongod
    ```
    Jika muncul tulisan `active (running)`, berarti server sudah berjalan. Tekan `q` untuk keluar dari tampilan status.
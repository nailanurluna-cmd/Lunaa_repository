 # Cara Instalasi MariaDB di Debian/Ubuntu

Berikut adalah langkah-langkah untuk menginstal MariaDB di Terminal:

1.  **Perbarui Paket Sistem**
    Jalankan perintah ini untuk memperbarui daftar paket sistemmu:
    
    ```bash
    sudo apt update
    ```
    
2.  **Instal MariaDB**
    Gunakan perintah ini untuk menginstal server dan client MariaDB:
    
    ```bash
    sudo apt install mariadb-server mariadb-client
    ```
    Jika diminta konfirmasi, ketik `y` lalu tekan Enter.
    
3.  **Amankan Instalasi**
    Jalankan perintah ini untuk mengamankan server:
    
    ```bash
    sudo mysql_secure_installation
    ```
    Ikuti instruksi yang muncul di Terminal. Jika ini instalasi baru, biasanya kamu bisa langsung menekan Enter untuk password root, lalu ketik `y` untuk semua pertanyaan berikutnya.

4.  **Cek Status MariaDB**
    Untuk memastikan instalasi berhasil, cek status server dengan perintah ini:
    
    ```bash
    sudo systemctl status mariadb
    ```
    Jika muncul tulisan `active (running)`, berarti sudah berhasil. Tekan `q` untuk keluar dari tampilan status.

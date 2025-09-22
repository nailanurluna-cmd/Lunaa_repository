1. Saat memasukkan kode **mkdir .ssh** tertulis **cannot create directory.**
**Solve** lanjut step selanjutnya aja, masukkan **ssh-keygen -t ed25519 -c "youremail@example.com"**
Email-nya diganti email kita yang terdaftar di github ya.

2. Saat memasukkan kode **ssh-keygen -t ed25519 -c "youremail@example.com"** tertulis **Too many arguments.**

**Solve** langsung step selanjutnya aja, masukkan **ssh-keygen -t rsa -b 4096 -C "youremail@example.com"** lalu enter. nanti kita disuruh isi nama filenya
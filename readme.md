How To Install this Project
1. Persiapan
- Memiliki CLI/Command Line Interface berupa Command Prompt (CMD) atau Power Shell atau Git Bash (selanjutnya kita sebut terminal).
- Memiliki Web Server (misal XAMPP) dengan PHP minimal versi 7.1.3.
- Composer telah ter-install, cek dengan perintah composer -V melalui terminal.
- Memiliki koneksi internet (untuk proses installasi).

2. Langkah-Langkah
- git clone Melalui terminal,
- cd ke direktori food-order-system.
- (Sesuai petunjuk installasi) Pada terminal, berikan perintah composer install. Ini yang perlu koneksi internet.
- Composer akan menginstall dependency paket dari source code tersebut hingga selesai.
- Jalankan perintah php artisan, untuk menguji apakah perintah artisan Laravel bekerja.
- Buat database baru (kosong) pada mysql (via phpmyadmin) dengan nama food-order-system.
- Duplikat file .env.example, lalu rename menjadi .env.
- Kembali ke terminal, php artisan key:generate.
- Setting koneksi database di file .env (DB_DATABASE, DB_USERNAME, DB_PASSWORD).
	DB_CONNECTION=mysql
	DB_HOST=localhost
	DB_PORT=3306
	DB_DATABASE=food-order-system
	DB_USERNAME=root
	DB_PASSWORD=
- Run migrations (tables and Seeders) php artisan migrate --seed. Cek di phpmyadmin, seharusnya tabel dan isi nya sudah muncul.
- Setelah selesai, Jalankan perintah php artisan serve maka dapat diakses dengan http://localhost:8000/


Untuk Database
Atau bisa juga import file food.sql di phpmyadmin pada database yang sudah dibuat 


Link masuk ke admin = http://localhost:8000/admin
email : admin@email.com
password : 123456

Link masuk menjadi user = http://localhost:8000/login-check
email : rahmetuloh@gmail.com
password : 123456


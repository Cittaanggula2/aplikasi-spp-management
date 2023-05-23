# aplikasi-spp-management
Aplikasi SPP Management menggunakan Laravel

Berikut Cara menjalankan project nya :

buka command prompt > ketik git clone https://github.com/hilman-firdd/Aplikasi-Manajemen-SPP-Sekolah.git lalu tekan enter.
install composer terlebih dahulu, https://getcomposer.org/Composer-Setup.exe
apabila sudah ada xampp control panel di device kalian, pastikan php version punya kalian 7.x. cara cek, nyalakan xampp control panel untuk service apache dan mysql, lalu buka https://localhost/dashboard/phpinfo.php
apabila php version kalian versi 8, lakukan uninstall xampp di device kalian
lalu install xampp versi 7, https://sourceforge.net/projects/xampp/files/XAMPP%20Windows/7.4.30/xampp-windows-x64-7.4.30-1-VC15-installer.exe/download
ulangi step nyalakan kembali xampp dan cek php info kalian apakah sudah versi 7.x
kemudian, buka folder project yang sudah kita clone, search di windows cmd (command prompt), open cmd (command prompt), ketik cd aplikasi, lalu tekan tab pada keyboard, kalian akan melihat di layar prompt menjadi 
cd Aplikasi-Manajemen-SPP-Sekolah, kemudian tekan enter.
open folder Aplikasi-Manajemen-SPP-Sekolah, pastikan file .env sudah ada, apabila belum ada, copy dari file .env.example dan paste di dalam folder itu kemudian rename menjadi .env
buka file .env menggunakan IDE yang kalian punya seperti notepad++, visual studio code, dll
apabila ingin mengikuti database name yang sudah dibuat di file .env, maka cukup membuat database baru di https://localhost/phpmyadmin/
kemudian di sebelah kiri pilih New
kemudian input database name sesuai dengan database name di file .env (spp_app jika tidak ingin dirubah dan mengikuti apa yang sudah diset) lalu tekan tombol Create
kembali ke command prompt yang sudah dibuka sebelum nya, jalankan composer update tunggu hingga selesai
lalu jalankan composer install tunggu hingga selesai
kemudian jalankan php artisan migrate
lalu php artisan db:seed
lalu php artisan key:generate
lalu php artisan storage:link
kemudian open folder Aplikasi-Manajemen-SPP-Sekolah, open folder storage, open folder framework, lalu buat folder baru sessions
kembali ke command prompt, dan jalankan project dengan php artisan serve
buka browser dan ketik localhost:8000 pada url bar
login dengan akun username: superadmin dan password: password
untuk beberapa role dan username yang ada bisa dicoba juga menggunakan password yang sama. seperti role : admin, kepsek, bendahara, siswa
role tersebut memiliki hak akses menu navigasi pada website yang berbeda. paling lengkap adalah superadmin.
selamat mencoba

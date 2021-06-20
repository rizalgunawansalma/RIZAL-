Nama	:	rizal gunawan
Nim	:	311910798
Kelas	:	TI19B1

1.	Konfigurasi ekstensi PHP yang perlu diaktifkan seperti di gambar ini. Untuk mengaktifkan ekstensinya, hapus tanda ;
![image](https://user-images.githubusercontent.com/85833641/122664494-a3c63280-d156-11eb-82ef-60ae57979864.png)
2.Ada beberapa ekstensi lainnya juga untuk pengembangan Codeinteger, seperti berikut.
•	php-json ekstension untuk bekerja dengan JSON;
•	php-mysqlnd native driver untuk MySQL;
•	php-xml ekstension untuk bekerja dengan XML;
•	php-intl ekstensi untuk membuat aplikasi multibahasa;
•	libcurl (opsional), jika ingin pakai Curl.
•	Buat folder baru pada htdocs bernama lab11_ci.
•	Unduh Codeinteger di web https://codeigniter.com/download
•	Ubah nama direktory framework-4.x.xx menjadi ci4. Dan taruh kedalam folder lab11_ci
•	Buka browser dengan alamat http://localhost/lab11_ci/ci4/public/
![image](https://user-images.githubusercontent.com/85833641/122664510-c22c2e00-d156-11eb-89e5-6a36e6b1386c.png)
3.Menjalankan CLI (Command Line Interface) Buka XAMPP Control Panel, pilih Shell untuk membuka terminal/command prompt, arahkan sesuai dengan direktori folder lab11_ci seperti pada gambar ini. Perintah yang dapat dijalankan untuk memanggil CLI Codeinteegr adalah php spark
![image](https://user-images.githubusercontent.com/85833641/122664528-e425b080-d156-11eb-86da-08243351ad8c.png)
4.Mengaktifkan Mode Debugging Codeinteger menyediakan firut Debugging untuk memudahkan developer untuk mengetahui pesan error. Semua jenis error akan ditampilkan. Untuk mengaktifkannya, ubah nilai konfigurasi pada environtmen variable CI_ENVIRONMENT menjadi development seperti pada gambar ini. Dan ubah nama file env menjadi .env
![image](https://user-images.githubusercontent.com/85833641/122664538-f4d62680-d156-11eb-9871-9690eeda035b.png)
![image](https://user-images.githubusercontent.com/85833641/122664542-fa337100-d156-11eb-9252-c3407334e230.png)
Gambar dibawah ini adalah setelah mengaktifkan fitur Debugging. Setelah menghapus tanda ; pada file app/Controller/Home.php
![image](https://user-images.githubusercontent.com/85833641/122664557-0fa89b00-d157-11eb-9c21-670d258a8959.png)
5. Membuat Route Baru
![image](https://user-images.githubusercontent.com/85833641/122664565-1fc07a80-d157-11eb-89d0-c9c019f783a6.png)
6. Selanjutnya, akses alamat url http://localhost:8080/about untuk mencoba route yang telah dibuat. Ketika diakses akan muncul tampilan error, artinya file/page tersebut tudak ada. Untuk dapat mengakses halaman tersebut, buat Controller yang sesuai dengan rooting yang dibuat di Controller Page
7. ![image](https://user-images.githubusercontent.com/85833641/122664589-3797fe80-d157-11eb-9c94-d2433d37499a.png)
Membuat Controller Page Buat file baru dengan nama page.php pada direktori Controller, masukkan kode seperti gambar atau bisa mengakses file diatas. Setelah itu, save dan refresh halaman web yang tadi error. 
![image](https://user-images.githubusercontent.com/85833641/122664633-6a41f700-d157-11eb-8392-7fbe8380481d.png)
Tambahan
Ketika halaman tidak muncul dan masih error, coba untuk mengaktifkan perintah php spark serve pada command prompt seperti gambar ini. Pastikan untuk tetap berjalan pada latar belakang. 
![image](https://user-images.githubusercontent.com/85833641/122664643-79c14000-d157-11eb-8fd8-8f8dd339ff14.png)
Auto Routing Auto Routing secara default sudah aktif, untuk mengubah nilai variablenya dapat mengubah true menjadi false.
Sebelum diubah
![image](https://user-images.githubusercontent.com/85833641/122664654-9198c400-d157-11eb-95bd-f5339426de62.png)
Setelah diubah
![image](https://user-images.githubusercontent.com/85833641/122664661-a07f7680-d157-11eb-8b48-f7908d1bc32e.png)
•	Membuat View Buat file baru dengan nama about.php pada direktori app/views. Lihat gambar untuk lebih 
![image](https://user-images.githubusercontent.com/85833641/122664675-b4c37380-d157-11eb-8801-a3246c16b037.png)
Membuat Layout Web dengan CSS
•	Buat file css pada direktori Public dengan nama style.css.
copy file layout dari Praktikum 4 
![image](https://user-images.githubusercontent.com/85833641/122664690-cad13400-d157-11eb-9b4f-9fd4546f1e4d.png)
•	Buat folder template pada direktori view. Kemudian buat file header.php dan footer.php 
![image](https://user-images.githubusercontent.com/85833641/122664697-d91f5000-d157-11eb-8aae-96f9e62333f2.png)
•	Isikan kode seperti dibawah ini, bisa diakses pada file diatas. Save dan buka url http://localhost:8080/about
![image](https://user-images.githubusercontent.com/85833641/122664703-e89e9900-d157-11eb-8062-c8f7b1ba97d4.png)
Tugas
Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.
![image](https://user-images.githubusercontent.com/85833641/122664717-f9e7a580-d157-11eb-9600-b289c6367bad.png)

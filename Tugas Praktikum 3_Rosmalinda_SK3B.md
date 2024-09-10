Nama : Rosmalinda <br/>
Nim : 09011282328086 <br/>
Kelas : SK3B 

# Laporan Praktikum 2 Sistem Operasi
## BAB I. Pendahuluan
### 1.1 Latar Belakang
Sistem operasi linux adalah salah satu sistem operasi open-source yang menyediakan platform yang aman dan stabil untuk berbagai layanan aplikasi. Salah satu komponen dalam pengelolaan sistem linux adalah sistem file. Sistem file berfungsi sebagai struktur organisasi data di media penyimpanan. Sistem file di linux mengatur bagaimana data disimpan, diakses, dikelola, dan struktur organisasi file serta direktori. Dengan sistem file yang terorganisir penggunabdapat dengan mudah dalam mengelola file, mengakses data, dan memastikan integritas serta keamanan data. <p/>
Sistem file di linux memainkan peran kunci dalam pengelolaan data dan memfasilitasi interaksi yang efisien antara pengguna dan perangkat penyimpanan. Struktur sistem file Linux diatur dalam bentuk hierarki pohon yang dimulai dari root directory (/), yang merupakan titik awal dari semua path di sistem. Di bawah root directory, terdapat berbagai direktori penting yang menyimpan berbagai jenis data dan konfigurasi, seperti /bin untuk binary executables, /etc untuk file konfigurasi sistem, /home untuk direktori home pengguna, dan /var untuk file yang sering berubah seperti log dan cache. Dari praktikum ini di harapkan kita dapat menngetahui cara mengelola file, mengakses data dan lain sebagainya. <p/>

### 1.2 Tujuan
1.  Mengenal organisasi File di Linux. <br/>
2.  Menciptakan dan manipulasi direktori. <br/>
3.  Mempelajari ijin akses (permission) dari file dan direktori. <br/>
4.  Mengenal konsep Owner dan Group. <br/>
5.  Mengerti konsep Link dan symbolic link. <br/>
   
### 1.3 Alat dan Bahan
1.  Laptop
2.  Sistem Operasi Linux
3.  Command Line Linux

### 1.4 Dasar Teori
1. Organisasi file : <br/>
   Sistem file linux disusun secara hierarkis dalam bentuk struktur pohon yang berawal dari root directory (/). Semua file dan direktori di Linux termasuk perangkat keras disusun dalam struktur ini. Beberapa direktori penting dalam sistem file Linux terdiri dari /bin (yang berisi file executable yang dapat digunakan oleh semua pengguna), /etc (berfungsi untuk menyimpan file konfigurasi siste)m, /home (berfungsi sebagai direktori home untuk masing-masing pengguna) dan /var (berfungsi menyimpan file variatif seperti log, cache, serta file sementara). <p/>
2. Menciptakan dan Manipulasi direktrori: <br/>
   Dalam pengelolaan direktori, sistem Linux memungkinkan pengguna untuk menciptakan, menghapus, atau memodifikasi direktori menggunakan command line. Beberapa perintah dasar untuk manipulasi direktori yaitu mkdir untuk membuat direktori baru, rmdir atau rm -r untuk menghapus direktori, mv untuk memindahkan atau mengganti nama direktori, dan cp -r untuk menyalin direktori beserta isinya. <p/>
3. Izin Akses (Permission): <br/>
   Setiap file dan direktori di Linux memiliki aturan izin akses yang menentukan siapa yang dapat membaca, menulis, atau mengeksekusi file tersebut. Izin akses terbagi menjadi tiga kategori yaitu Read (r) yang memungkinkan seseorang membaca konten file atau melihat daftar direktori, Write (w) yang mengizinkan perubahan pada file atau modifikasi direktori; serta Execute (x) yang memungkinkan pengguna menjalankan file sebagai program atau mengakses direktori. Format izin akses ini dapat dilihat dengan menggunakan perintah ls -l yang menampilkan izin file dalam bentuk simbolik seperti drwxr-xr-x. Setiap file atau direktori memiliki tiga set izin: untuk owner, group, dan others. <p/>
4. Konsep Owner dan Group: <br/>
   Di Linux, setiap file dan direktori dimiliki oleh seorang owner dan sebuah group. Owner memiliki kendali penuh atas file atau direktori, sementara grup terdiri dari beberapa pengguna yang memiliki izin akses sesuai dengan yang diberikan oleh owner. Untuk mengelola kepemilikan file atau direktori, perintah chown (change ownership) dan chgrp (change group) dapat digunakan. <p/>
5. Link dan Symbolic link: <br/>
  Linux juga mendukung dua jenis link yang dapat digunakan untuk menunjuk ke file atau direktori lain yaitu hard link dan symbolic link(symlinks). Hard link adalah referensi langsung ke data pada disk yang memungkinkan beberapa nama file  merujuk ke data yang sama. Sebaliknya, Symbolic link adalah pintasan ke file atau direktori lain yang  menjadi "rusak" jika file aslinya dihapus. Perintah ln digunakan untuk membuat hard link, dan ln -s digunakan untuk membuat symbolic link. <p/>


## BAB II. Pembahasan
### 2.1 Lihat peralatan I/O, character device, yang ada pada system komputer. <p/>
   **Melihat peralatan I/O keseluruhan :** <br/>
   <img src="https://github.com/user-attachments/assets/6c7ff978-860c-4213-abf8-523f278bd71d" width=500/>
   <br/>
   **Melihat Peralatan I/O dengan karakter tertentu contohnya d :** <br/>
   <img src="https://github.com/user-attachments/assets/bb67f3e6-ebd9-4f48-a67b-7d455e71cbc5" width=500/>
   <br/>

### 2.2 Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5. <p/>
   <img src="https://github.com/user-attachments/assets/60277572-94bf-446a-a81f-e431cd7cfa63" width=500/>
   <br/>

### 2.3 Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret. <p/>
   <img src="https://github.com/user-attachments/assets/611a67e6-3bb0-4d4c-a0af-2c5b4e294265" width=500/>
   <br/>
   
   **Hasil :** <p/>
   **1. Isi file di Januari** <p/>
   <img src="https://github.com/user-attachments/assets/17e1abeb-3440-4198-8b95-702dd14ca3f2" width=500/>
   <br/>
   **2. copy ke februari dan maret** <p/>
   <img src="https://github.com/user-attachments/assets/7e4ab840-1f0c-495e-8b8d-713b799b3dbe" width=500/>
   <br/>
   <img src="https://github.com/user-attachments/assets/d37aa0f6-5c98-4c0e-98f7-3ea448bf7aa6" width=500/>
   <br/>

### 2.4 Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write. <p/>
   <img src="https://github.com/user-attachments/assets/e079c6d8-486d-4c5c-89f1-e628e010f852" width=500/>
   <br/>

### 2.5 Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute. <p/>
   <img src="https://github.com/user-attachments/assets/2d8bccac-f5a5-4970-b989-e5b171f64e61" width=500/>
   <br/>

### 2.6 Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute. <p/>
   <img src="https://github.com/user-attachments/assets/02fbb26a-4c8b-487d-88c0-dfb6ae3150f1" width=500/>
   <br/>

### 2.7 Hapuslah direktori maret. <p/>
   <img src="https://github.com/user-attachments/assets/05f80576-2b9b-4df9-9eb5-6e05a7489a89" width=500/>
   <br/>

### 2.8 Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari. <p/>
   <img src="https://github.com/user-attachments/assets/054c526c-90da-4128-9c2d-3ad1565dcae0" width=500/>
   <br/>

### 2.9 Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakah nilai default-nya.  <p/>
   <img src="https://github.com/user-attachments/assets/c559b1d6-8cc7-46ef-a2c9-46a724a7a48b" width=500/>
   <br/>

### 2.10 Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ? <p/>
   <img src="https://github.com/user-attachments/assets/eaf11167-9289-44fa-99da-8eb47537c1de" width=500/>
   <br/>

## BAB III. Penutup
### 3.1 Kesimpulan
Sistem file pada Linux adalah struktur data yang digunakan oleh sistem operasi untuk mengatur dan mengelola data di penyimpanan sekunder. Sistem file ini berperan dalam menyimpan, mengelola akses, dan menjamin integritas data melalui berbagai fitur yang tersedia. Sistem file di Linux berbentuk seperti pohon, dimulai dari root dan berkembang menjadi direktori serta subdirektori. Struktur direktori ini merupakan konsep fundamental yang memungkinkan pengguna mengelola file dan direktori secara hierarkis. Dalam praktikum ini, saya mempelajari cara membuat, menghapus, serta mengelola direktori, cara mengatur izin akses file dan direktori bekerja termasuk peran owner, group, dan others dalam pengaturan izin akses. Pemahaman tentang perintah seperti chmod, chown, serta ls -l sangat membantu dalam mengelola hak akses dan kepemilikan file dengan lebih baik sehingga memastikan data tetap aman dan terstruktur dengan benar. <p/>

   

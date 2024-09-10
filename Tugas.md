# Tugas-Praktikum-3-Sistem-Operasi

<h1>I. PENDAHULUAN</h1>
<h2>1.1 Latar Belakang</h2>
<p>Sistem file bertanggung jawab untuk mengatur penyimpanan dan pengambilan data dari media penyimpanan, seperti hard disk atau SSD. Sistem file menentukan cara data disimpan, diorganisasi, dan diakses oleh sistem operasi dan pengguna.Pemahaman yang baik tentang sistem file sangat penting karena berkaitan langsung dengan efisiensi, kecepatan akses, dan keandalan dalam mengelola data. Dalam konteks administrasi sistem, kemampuan untuk bekerja dengan berbagai jenis sistem file serta melakukan operasi dasar seperti membuat, menghapus, dan mengelola partisi atau volume adalah keterampilan esensial. Oleh karena itu, praktikum ini bertujuan untuk memberikan pengalaman langsung dalam mengelola sistem file pada Linux, termasuk cara mengakses, memodifikasi, dan mengoptimalkan performa sistem file.</p><br/>

<p>Melalui praktikum ini, mahasiswa diharapkan dapat memahami struktur sistem file Linux, melakukan manajemen file dan direktori, serta menggunakan perintah-perintah dasar Linux seperti ls, cp, mv, rm, dan lainnya. Selain itu, mahasiswa juga akan belajar tentang pentingnya hak akses file (file permissions) dan bagaimana sistem operasi Linux mengatur izin untuk membaca, menulis, dan mengeksekusi file. Dengan demikian, praktikum ini akan menjadi dasar yang kuat dalam memahami peran sistem file dalam menjaga integritas dan efisiensi operasional sistem komputer.</p><br/>
<h2>1.2 Tujuan Praktikum</h2>
1. Mengenal organisasi File di Linux<br/>
2. Menciptakan dan manipulasi direktori<br/>
3. Mempelajari ijin akses (permission) dari file dan direktori<br/>
4. Mengenal konsep Owner dan Group<nbr/>
5. Mengerti konsep Link dan symbolic link<br/>
<h2>1.3 Alat dan bahan</h2>
1. Laptop<br/>
2. Aplikasi Virtualbox<br/>
3. Ubuntu 24.04<br/>
<h2>1.4 Dasar Teori</h2>
<p>1. Sistem file pada Linux adalah mekanisme untuk mengatur penyimpanan data di media seperti hard disk atau SSD. Setiap file dan direktori diatur dalam struktur hierarki yang dimulai dari root directory /. Linux mendukung berbagai jenis sistem file, seperti Ext4, XFS, dan Btrfs, yang masing-masing digunakan sesuai kebutuhan spesifik. Sistem file ini bertanggung jawab dalam menentukan cara data disimpan, diakses, dan dikelola di dalam sistem operasi.</p><br/>
<p>2. Linux adalah sistem operasi multi-user yang membutuhkan pengaturan izin akses file untuk menjaga keamanan data. Setiap file atau direktori memiliki tiga jenis izin: read (r), write (w), dan execute (x), yang berlaku untuk tiga kategori pengguna: user, group, dan others. Izin ini ditampilkan secara simbolik atau numerik (misalnya 755). Pengaturan izin dilakukan dengan perintah chmod, yang memungkinkan perubahan hak akses guna menjaga kontrol dan keamanan sistem.</p><br/>
<p>3. Linux adalah sistem operasi multi-user yang membutuhkan pengaturan izin akses file untuk menjaga keamanan data. Setiap file atau direktori memiliki tiga jenis izin: read (r), write (w), dan execute (x), yang berlaku untuk tiga kategori pengguna: user, group, dan others. Izin ini ditampilkan secara simbolik atau numerik (misalnya 755). Pengaturan izin dilakukan dengan perintah chmod, yang memungkinkan perubahan hak akses guna menjaga kontrol dan keamanan sistem.</p><br/>
<h1>II. PEMBAHASAN</h1>
<h2>Langkah-Langkah Praktikum </h2>
<h2>1. Lihat peralatan I/O, character device, yang ada pada system komputer. </h2><br/>
<img src = https://github.com/user-attachments/assets/d7810652-f369-40ca-a9aa-1daeb733786c width=500/>
<img src = https://github.com/user-attachments/assets/c86ff731-70d7-4fb4-8087-6d648a9ba345 wodth=500/>

<h2>2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.  </h2><br/>
<img src = https://github.com/user-attachments/assets/9d4f078a-1d99-435a-b8f0-3fdb82dfe604 width=500/>

<h2>3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari 
dan copy-kan file tersebut ke sub direktori februari dan maret.</h2><br/>
<img src = https://github.com/user-attachments/assets/3702f7ff-b9ea-4df7-a28d-f6f8823fba02 width=500/>

<h2>4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others 
dapat melakukan write. </h2><br/>
<img src = https://github.com/user-attachments/assets/2a0793ad-e9a2-4c21-8326-eb0db45bffa6 width=500/>

<h2>5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat 
melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read 
dan execute. </h2><br/>
<img src = https://github.com/user-attachments/assets/b035c7e9-8176-41e4-aaf9-2608afbf7d81 width=500/>

<h2>6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat 
melakukan write, read dan execute. </h2><br/>
<img src = https://github.com/user-attachments/assets/9c828cc1-17cd-4e31-9a19-9d5bf685c095 width=500/>

<h2>7. Hapuslah direktori maret.  </h2><br/>
<img src = https://github.com/user-attachments/assets/fff17339-2565-45fe-a75e-4e3471bec66c width=500/>

<h2>8. Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat 
melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori 
februari. </h2><br/>
<img src = https://github.com/user-attachments/assets/b518862d-2128-48cd-9817-b001c5304539 width=500/>
<img src = https://github.com/user-attachments/assets/92759b99-d795-48c2-83d2-d3704395c96e width=500/>

<h2>9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan 
nilai default-nya ?  </h2><br/>
<img src = https://github.com/user-attachments/assets/5aa1d17f-7f55-43b0-8dc7-673784e95dab width=500/>

<h2>10. Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah 
list perhatikan berapa link yang terjadi ? </h2><br/>
<img src = https://github.com/user-attachments/assets/8ca69ebe-b168-4194-b165-71e93932e063 width=500/>
<h1>III. PENUTUP</h1>
<h2>3.1 Kesimpulan</h2>
<p>Praktikum ini memberikan pemahaman mendalam tentang pengelolaan sistem file di Unix/Linux, termasuk manajemen file, struktur direktori, dan pengaturan izin akses. Sistem file berperan penting dalam menyimpan dan mengatur data, sementara izin akses memastikan keamanan dan kolaborasi yang aman. Struktur direktori yang terorganisir memudahkan pengelolaan dan pencarian file. Penguasaan operasi dasar seperti membuat, menyalin, dan menghapus file adalah keterampilan penting. Secara keseluruhan, praktikum ini membekali peserta dengan keterampilan praktis untuk mengelola sistem file secara efisien dan aman.</p><br/>

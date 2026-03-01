# Assingment_machine_learning_session2
Belajar pengantar dari machine learning lalu installasi anaconda, membuat conda environment, menginstall library, dan mengepush ke github

## Python
Python adalah bahasa pemrograman multifungsi yang banyak disukai untuk analisis data.
Karakteristik Python:
 - Python mengeksekusi kode baris demi baris, jadi tidak perlu kompilasi
 - Python tidak perlu mendeklarasikan tipe variabel
 - Mudah dipelajari dan terbaca
 - Python juga sering terupdate librarynya.

## Environment Manager
Environment manager adalah alat yang membuat, mengatur dan mengupdate lingkungan project python yang membutuhkan versi python dan versi library.
Envi ini bertujuan untuk merapikan dan menyesuaikan library dengan versi python.

## Anaconda



## Installasi Anaconda
Anaconda sendiri digunakan untuk 
1. Membuka website resmi Anaconda https://www.anaconda.com/download
2. Download Anaconda
3. Setelah selesai, install Anaconda hingga muncul Anaconda enviroment
4. Untuk mengecek apakah sudah terinstall Anaconda dengan cara mengecek di CMD
5. Lalu ketik conda --version, jika muncul versi maka conda berhasil terinstall

## Conda Environment
1. Buka file tugas assigmnet lalu ketik cmd di path file untuk membuka CMD
2. Ketik di CMD, conda create -n ml-1 python=3.15 pandas numpy scikit-learn, ini digunakan untuk membuat environment conda baru bernama ml-1 dengan versi python dan langsung menginstall library, lalu enter
3. untuk mengaktifkan conda environment ketik conda activate ml-1

## Menginstall Library
Menginstall seaborn dengan mengetik pip install seaborn

## Mengepush ke github
1. Membuat repository baru di github, lalu salin link repository untuk di push ke git
2. Untuk menampilkan seluruh konfigurasi Git yang aktif dengan mengetik di cmd
   git config --list, enter
3. Untuk menambahkan semua file ke github
   git add . , enter
4. Untuk mengcommit perubahan
   git commit -m "commit semua file submition" , enter
5. Untuk mengganti nama branch yang aktif untuk menjadi main
   git branch -M main, enter
6. Lalu hubungkan ke reopsitory github
   git remote add origin https://github.com/RevaNia12/Machine_Learning_Assinggment_Session2.git, enter
7. Dan terakhir tinggal mengepush ke github
   git push -u origin main, enter

   

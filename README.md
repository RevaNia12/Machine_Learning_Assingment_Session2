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
Anaconda sendiri adalah platform yang sering digunakan AI dan data science yang menggunakan bahasa python.
Alasan penggunaan Anaconda:
- Mudah dipelajari buat pemula
- Package manager untuk membuat project python

## Hands On YEAH
### Installasi Anaconda
Anaconda sendiri digunakan untuk 
1. Membuka website resmi Anaconda https://www.anaconda.com/download
2. Download Anaconda
3. Setelah selesai, install Anaconda hingga muncul Anaconda enviroment
4. Untuk mengecek apakah sudah terinstall Anaconda dengan cara mengecek di CMD
5. Lalu ketik conda --version, jika muncul versi maka conda berhasil terinstall

### Conda Environment
1. Buka file tugas assigmnet lalu ketik cmd di path file untuk membuka CMD
2. Ketik di CMD, conda create -n ml-1 python=3.15 pandas numpy scikit-learn, ini digunakan untuk membuat environment conda baru bernama ml-1 dengan versi python dan langsung menginstall library, lalu enter
3. untuk mengaktifkan conda environment ketik conda activate ml-1

### Menginstall Library
Menginstall seaborn dengan mengetik pip install seaborn

## Library untuk manipulasi data dan machine learning
1. Pandas untuk manupasi dataframe
2. Scikit-learn untuk preprocessing
3. Tensorflow untuk deep learning
4. Numpy untuk manipulasi array, matriks
5. Matplotlib dan seaborn untuk visualisasi data berupa grafik
   
## Hands On Data Manipulation
1. Membuka notebook di vs code
2. Menginstall extension jupyter dan python, lalu tunggu sampai selesai
3. import pandas as pd
   url = 'https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv'
   df = pd.read_csv(url) , untuk membaca dataset dari url
4. from sklearn.datasets import load_iris
   iris = load_iris()
   memuat dataset Iris yang sudah disediakan oleh scikit-learn ke dalam program Python.
5. display (df)
   untuk menampilkan dataset
6. df.isnull().sum()
   Untuk mengetahui jumlah data yang kosong
7. df.head()
   Untuk menampilkan beberapa baris pertama dari DataFrame
8. kolom_sampah = ['PassengerId', 'Name', 'Ticket', 'Cabin', 'Embarked']
   df_bersih = df.drop(columns=kolom_sampah)
   Untuk membuang data yang tidak mempengaruhi penelitian lalu membuat variabel baru df_bersih tanpa kolom_sampah.
9. df_bersih.head()
    Untuk mengecek DataFrame bersih apakah variabel yang terbuang sudah tidak ada
10. median_umur = df_bersih['Age'].median()
    df_bersih['Age'] = df_bersih['Age'].fillna(median_umur)
    Untuk mengisi nilai yang kosong di umur dengan median umur
11. df_bersih = df_bersih.dropna()
    menghapus baris data yang mengandung nilai kosong
12. df_final_gdum = pd.get_dummies(df_bersih, columns=['Sex'], drop_first=True, dtype=int)
    Untuk mengubah tipe data pada sex menjadi int
13. from sklearn.preprocessing import MinMaxScaler
    scaler = MinMaxScaler()
    df_scalemimax = scaler.fit_transform(df_final_gdum)
    menormalisasi (scaling) data numerik ke rentang 0 sampai 1

## Git
Git adalah sistem kontrol versi yang berjalan secara lokal di komputer untuk melacak perubahan pada kode dan file.

## Github
Github adalah platform web yang menggunakan Git untuk menyediakan lokasi untuk menyimpan, berbagi dan berkolaborasi dalam proyek.

## Hands On Git and Github
### Mengepush ke github
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
   
<img width="1183" height="346" alt="image" src="https://github.com/user-attachments/assets/c6707803-e1ef-47d4-84a2-ca26217c0810" />
Jika sudah seperti inii, selamatt sudah berhasill mengepushh github :V

   

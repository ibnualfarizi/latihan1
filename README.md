# latihan1
# Apa itu Git?
* Git adalah salah satu sistem pengontrol versi (Version Control
System) pada proyek perangkat lunak yang diciptakan oleh Linus
Torvalds.
* Pengontrol versi bertugas mencatat setiap perubahan pada file
proyek yang dikerjakan oleh banyak orang maupun sendiri. 
* Git dikenal juga dengan distributed revision control (VCS terdistribusi),
artinya penyimpanan database Git tidak hanya berada dalam satu
tempat saja.
# Instalasi Git
* Download Git, buka website resminya Git [git-scm.com](https://git-scm.com "aa'nhue")
* Kemudian unduh Git sesuai dengan arsitektur komputer kita. Kalau
menggunakan 64bit, unduh yang 64bit. Begitu juga kalau
menggunakan 32bit. 
* Selamat, Git sudah terinstal di Windows. Untuk mencobanya,
silahkan buka CMD atau PowerShell, kemudian ketik perintah
``git --version``

![Tanpa judul](https://user-images.githubusercontent.com/57051625/68082686-3024c400-fe52-11e9-9009-307b62dc6443.png)

# Menambahkan Global Config
* Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email.
* konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.
* apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit
* Config Global Repository
$ git config --global user.name “nama_user”
$ git config --global user.email “nama_user"

![Tanpa judul nama](https://user-images.githubusercontent.com/57051625/68082801-a4ac3280-fe53-11e9-895d-3c6a702539f1.png)

# Perintah Dasar Git
* git init, perintah untuk membuat repository local 
* git add, perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
* git commit, perintah untuk menyimpan perubahan kedalam database git. 
* git push -u origin master, perintah untuk mengirim perubahan pada repository local menuju server repository.
* git clone [url], perintah untuk membuat working directory yang diambil dari repositry sever. 
* git remote add origin [url], perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)
* git pull, perintah untuk mengambil/mendownload perubahan terbaru dari server repository ke local repository

# Membuat Reposiory Local
* Jalankan perintah git init, untuk membuat repository local.
* Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
* Pada direktori tersebut, semua perubahan pada working directory akan disimpan. 

![Tanpa judul git in](https://user-images.githubusercontent.com/57051625/68082886-a3c7d080-fe54-11e9-87e0-cca1b28228bf.png)

# Menambahkan File baru pada repository
* Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository) 
* disini kita akan coba buat satu file bernama README.md (text file)
$ echo “#Latihan 1” >> README.md
* File README.md berhasil dibuat.

![Tanpa judul3](https://user-images.githubusercontent.com/57051625/68082453-90663680-fe4f-11e9-9ad5-4bacabeee8fa.png)

# Commit (Menyimpan perubahan ke database)
* Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”
* Perubahan berhasil disimpan. 

![Tanpa judul 4png](https://user-images.githubusercontent.com/57051625/68082949-8b0bea80-fe55-11e9-8bdb-67bf166ec47c.png)

# Membuat repository server
* Server reopsitory yang akan kita gunakan adalah http://github.com 
* Anda harus membuat akun terlebih dahulu. 
* Pada laman github, klik tombol start a project, atau 
* Dari menu (icon +) klik New Repository
# Membuat repository server
* Isi nama repositorynya, misal: labpy1. 
* lalu klik tombol Create repository
# Menambahkan Remote Repository
* Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user. 
* Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]
# Push (Mengirim perubahan ke server)
* Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
* Perintah ini akan meminta memasukkan username dan password pada akun github.com 

![Tanpa judul5](https://user-images.githubusercontent.com/57051625/68082977-e4741980-fe55-11e9-9b25-0f72683e883c.png)

# Melihat hasilnya pada server repository
* Buka laman github.com, arahkan pada repositorinya. 
* Maka perubahan akan terlihat pada laman tersebut
# Clone Repository
* Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory). 
* Untuk melakukan cloning, gunakan perintah git clone [url]

![Tanpa judu4l](https://user-images.githubusercontent.com/57051625/68083002-3157f000-fe56-11e9-8003-e812416b1d77.png)

# Tes
Untuk membuat Gradle dan menambahkan pustaka


Buat Proyek Gradle Baru:

Jalankan perintah berikut di terminal untuk membuat proyek Gradle baru dengan jenis proyek Java:

bash
Copy code
gradle init --type java-library
Ini akan membuat struktur dasar proyek Gradle dengan file build.gradle awal.

Tambahkan Tugas Khusus Gradle:

Buka file build.gradle di direktori root proyek dan tambahkan kode berikut untuk menentukan tugas khusus:

groovy
Copy code
task greetingTask() {
    doLast {
        String name = project.hasProperty('name') ? project.property('name') : 'Gradle User'
        println "Hello, $name! Welcome to Gradle World!"
    }
}
Ini akan membuat tugas Gradle sederhana yang akan mencetak pesan salam dengan nama yang diberikan.

Menambahkan Pustaka:

Untuk menambahkan pustaka, tambahkan kode berikut ke file build.gradle Anda di bagian dependencies:

groovy
Copy code
dependencies {
    implementation 'com.google.guava:guava:29.0-jre'
    testImplementation 'junit:junit:4.13'
}
Ini akan menambahkan pustaka Google Guava dan JUnit ke proyek Anda.

Dorong Proyek ke GitHub:

Inisialisasi repositori git di direktori proyek:

csharp
Copy code
git init
Tambahkan semua perubahan ke area staging:

csharp
Copy code
git add .
Lakukan commit perubahan:

sql
Copy code
git commit -m "Initial commit"
Buat repositori baru di GitHub.

Tambahkan URL repositori GitHub sebagai remote:

csharp
Copy code
git remote add origin https://github.com/<nama_pengguna_anda>/<nama_repositori>.git
Dorong proyek ke repositori GitHub:

perl
Copy code
git push -u origin master
Dengan langkah-langkah ini, Anda telah membuat proyek Gradle dengan tugas khusus dan menambahkan pustaka, serta mendorongnya ke repositori GitHub. Semoga berhasil!

![image](https://github.com/RajabAlFajri/Tes/assets/86873137/8a9c7a0a-4939-4f40-8806-eb08ba4e4151)

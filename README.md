# Mengerjakan Skenario yang ada di KataCoda

## Orchestration using Docker Compose

A. Step 1 ( Mendefinisikan kontainer pertama )

Pada step ini docker compose itu didasarkan  pada file _docker-compose.yml_. File ini nantinya
akan mendefinisikan semua kontainer yang ada dan penyettingan yang diperlukkan.
Adapun format file nya adalah seperti gambar dibawah ini :

![gambar 1](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss1.jpg)

B. Step 2 ( Menentukkan pengaturan )

Pada step ini menjelaskan bahwasanya docker compose itu didukung dengan smeua properti yang bisa djelaskan 
dengan menggunakan _docker run_.
Adapaun contoh propertinya adl sebagai berikut :

+ Properti untuk me link kan container dengan nama redis, yang querynya seperti berikut :

![gambar 2](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss2.jpg)

+ Properti untuk ports, yang querynya seperti dibawah ini :

![gambar 3](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss3.jpg)

C. Step 3 ( Mendefinisikan kontainer kedua )

Pada step ini dijelaskan bahwa kita menggunakan DockerFile itu sebagai dasar dari kontainer kita,
oleh karena itu kali ini kita akan menggunakan image yang ada di Docker Hub sebagai kontainer kedua.
Untuk mendefinisikan kontainer kedua caranya hampir sama ketika membuat kontainer yang pertama tadi 
adapun querynya adalah sebagai berikut :

![gambar 4](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss4a.jpg)

D. Step 4 ( docker Up )

Pada step ini dijelaskan bahwa setelah kita membuat file _docker-compose.yml_ maka kita dapat memunculkan aplikasi dengan menggunakan peirintah _up_
dan jika kita ingin bersamaan memunculkanya di kontainer kita dapat menggunakan perintah _up <name>_
Untuk lebih jelas menegnai query untuk memunculkan alikasi dan hasilnya dari yang sudah kita buat adl sbg berikut :

![gambar 5](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss4b.jpg)

E. Step 5 ( Memanajemen docker )

Pada step ini dijelaskan bahwa fungsi dari docker compose tidak hanya untuk mengatur pembuatan kontainer saja
akan tetapi docker compose juga mampu mengatur semua kontainer dengan menggunakan perintah-perintah berikut ini :

+ _docker-compose ps_ ( berfungsi untuk melihat detail dari kontainer yang sudah dimunculkan )


+ _docker-compose logs_ ( berfungsi untuk melihat semua logs yang ada )


+ _docker-compose_



Adapun hasil dari uji coba ketiga perintah tersebut adalah sebagai berikut :

![gambar 6](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss5a.jpg)

![gambar 7](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss5b1.jpg)

![gambar 8](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss5b2.jpg)


F. Step 6 ( Skala docker / Docker Scale )

Pada step ini dijelaskan bahwa fungsi dari docker compose selain untuk memunculkan aplikasi yang kita buat , docker compose juga berfungsi untuk memberikan skala
pada kontainer yang sedang berjalan dengan menggunakan perintah _docker-compose scale web=3_, dan untuk mengentikanya adalah dengan menggunakan 
query _docker-compose scale web=1_

Adapun hasil dari query-query tersebut adalah sebagai berikut :

![gambar 9](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss6.jpg)



G. Step 7 ( Menghentikan docker )

Pada step ini dijelaskan bahwa setelah kita memunculkan aplikasi kita, dan ketika ingin
menghentikan pengaturan dari kontainer maka bisa menggunakan perintah _docker-compose stop_, dan ketika ingin
menghapus semua kontainer yang sudah dibuat maka menggunakan perintah _docker-compose rm_

Adapun hasil dari query-query tersebut adalah sebagai berikut :

![gambar 10](https://github.com/AnnisaFahma/docker_AnnisaFahma2/blob/master/gambar/ss7.jpg)


## Sekian praktik hari ini :)
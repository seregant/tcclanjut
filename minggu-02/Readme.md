## MINGGU 02 - Menggunakan fitur pull request

1. Setelah login ke GitHub pilih repositori lalu masuk ke menu tab **Pull requests**
	
	![1](images/step1.PNG)
	
2. Klik button **New pull request**
	
	![2](images/step2.png)
	
3. Jika belum ada fork atau branch lain yang berbeda dengan master, maka kita tidak bisa melakukan pull request dan akan diinstruksikan untuk membuat branch baru agar dapat dibandingkan dengan master. Kita bisa membuat branch dari repo tersebut menjadi repo di akun kita dengan menggunakan fitur fork
	
	Disini saya menggunakan repo dari [Reno Faizal](https://github.com/renfaizal/tcclanjut) 

	![3](images/fork.png)

	Klik icon fork tersebut maka akan dibuat sebuah repo baru di akun kita dengan menduplikasi dari repo yang kita fork.

	![5](images/fork2.png)

	Pada gambar di atas dapat kita lihat setelah menlakukan klik ke icon fork kita akan dialihkan ke akun kita sendiri ke repo hasil duplikasi dari repo yang kita fork, sehingga kita memiliki repo yang sama persis dengan repo dimana kita ingin berkontribusi di repo tersebut. Di repo baru ini kita bebas melakukan perubahan karena repo ini milik kita sendiri.

	Berikut adalah hasil dari proses duplikasi dengan fork yang sudah selesai

	![6](images/fork3.png)
	
4. Setelah melakukan perubahan di repo fork kita, untuk melakukan merge ke repo asli kita perlu melakukan pull request.

	Berikut adalah perubahan yang saya lakukan di repo saya sendiri

	![7](images/step5.png)

	Kita buat pull request di repo asli

	![4](images/step4.PNG)

	Kita klik link "Compare accross fork" lalu pilih repo kita dari hasil forking sebelumnya dan pilih branch dimana kita melakukan perubahan. Maka hasilnya akan seperti pada gambar di atas.

5. Isi form keterangan perubahan pada repo

	![8](images/step8.png)

	Gambar di atas adalah form untuk mengisi keterangan dari pull request kita buat. Check "Allow edit from maintenance" apa bila kita ingin mengijinkan pemilik repo mengedit branch yang akan kita ajukan menjadi pull request untuk digabungkan ke repo asli.

	Setelah itu klik "Create pull request"

6. Berikut adalah hasil dari pull request yang telah dibuat.

	![8](images/success.png)

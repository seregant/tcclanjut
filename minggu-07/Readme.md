### Go HTTP Server

1. Membuat HTTP Server dengan menggunakan library __net/http__

    Package __net/http__ adalah package bawaan dari go yang digunakan untuk menjalankan web server sehingga program dapat menjalankan web server dan menerima serta merspon request http.

    ![01](img/01-Helloword.png)

    Contoh script di atas adalah contoh penggunaan library __net/http__. Request untuk setiap route yang diterima pada library __net/http__ menggunakan funsi ```HandleFunc()``` dengan dua parameter. Prameter pertama adalah route dari request dan parameter kedua adalah fungsi yang digunakan untuk melakukan response ke requet route tersebut.

    Pada contoh tersebut web server dijalankan pada port 8080 sesuai dengan konfigurasi yang dilakukan melalui fungsi ```ListenAndServe()```

    Untuk menjalankan program masuk ke direktori script main.go lalu jalankan perintah ```go run main.go```. Lalu untuk testing akses menggunakan browser pada localhost:8080.

    ![02](img/1-03-Helloword.png)

    Dapat kita liat pada output browser, respon yang didapatkan untuk route " / " pada aplikasi adalah tampilan yang sesuai dengan kode yang dijalankan pada fungsi yang dimasukan ke parameter ke dua ```HandleFunc()```.

2. Menggunakan framework __mux__

    Banyak framework pada bahasa pemrograman go untuk membuat backend service. Salah satunya adalah __mux__. Untuk menggunakan mux terlebih dahulu download packagenya dengan perintah ```go get -u github.com/gorilla/mux```.

    Jika tidak ada error terjadi maka package library mux akan didownload dan tersimpan dalam folder ${GOPATH}/src seperti berikut.

    ![03](img/2-02.png)

    Berikut adalah contoh penggunaan __mux__ :

    ![04](img/2-03.png)

    Dapat dilihat pada kode di atas, untuk mengimport library di luar dari library bawaan golang, kita harus menuliskan path folder library secara lengkap pada direktori ${GOPATH}/src dimana library disimpan.

    Pada framework __mux__ dalam request rout dapat dibuat variabel dengan menambahkan tanda ```{}``` . Dalam contoh di atas pada parameter request route terdapat dua variabel yaitu ```title``` dan ```page``` dimana nilai yang ada pada variabel ini dapat diambil dengan menggunakan fungsi `Vars()` yang disediakan dalam libarary __mux__.

    Berikut adalah hasil output dari program tersebut :

    ![05](img/2-04.png)

    Dalam output tersebut dapat kita lihat nilai dari variabel title adalah `Nama Buku` dan nilai dari variabel page adalah `100`.
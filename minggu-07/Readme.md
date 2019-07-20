### Go HTTP Server

1. Membuat HTTP Server dengan menggunakan library ___net/http/__

    Package ___net/http__ adalah package bawaan dari go yang digunakan untuk menjalankan web server sehingga program dapat menjalankan web server dan menerima serta merspon request http.

    ![01](img/01-Helloword.png)

    Contoh script di atas adalah contoh penggunaan library ___net/http__. Request untuk setiap route yang diterima pada library ___net/http__ menggunakan funsi ```HandleFunc()``` dengan dua parameter. Prameter pertama adalah route dari request dan parameter kedua adalah fungsi yang digunakan untuk melakukan response ke requet route tersebut.

    Pada contoh tersebut web server dijalankan pada port 8080 sesuai dengan konfigurasi yang dilakukan melalui fungsi ```ListenAndServe()```
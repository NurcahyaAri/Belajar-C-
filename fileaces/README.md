<h1>File Access?</h1>

<h2>Reina : Mas Apa sih File Akses?? </h2>

<h2>Takahiro : </h2>

<p>
Nah jadi gini, ketika kalian membuat dan menjalankannya maka data yang kalian simpan didalam variabel itu sifatnya itu sementara. jadi ketika program yang sudah kalian jalankan tersebut kalian keluarkan maka isi dari variabel tersebut juga akan hilang. contohnya gini, ketika kalian membuat program untuk menghitung luas persegi panjang, dimana rumus persegi panjang adalah sisi * sisi. nah ketika kalian inputkan sisinya bernilai 5 maka selama program itu berjalan sisinya ya nilainya 5, tetapi ketika program tersebut kalian keluarkan maka sisi tersebut nilainya bisa berubah lagi tergantung kalian.

nah jika kalian ingin menyimpan nilai dari variabel yang sudah kalian isikan untuk kalian pakai kembali maka cara satu satunya adalah menggunakan akses file.. apa itu sih akses file? nah akses file adalah suatu cara agar kita dapat memanipulasi file dengan program yang kita buat, jadi tanpa harus membuat file secara manual tetapi program sudah membuatkannya secara automatis, kemudian kita bisa menyimpan data dari variabel yang sudah kita deklarasikan sebelumnya... jadi saat kita membuat program luas persegi dan kita ingin data persegi sebelumnya yang sudah kita hitung itu masih ada dan bisa ditampilkan kembali suatu saat nanti kalian bisa melakukannya dengan file akses ini... ya namanya file akses
</p>


<h2>Reina : Aku masih bingung mas hehehe<h2>

<h2>Takahiro : </h2>

<p>
Jadi Gampangnya gini Rei.. kalau kamu pengen nyimpen data biar bisa kamu baca lagi besok besok kan harus dibukukan datanya biar ga hilang,nah di program juga gitu. intinya kalau kamu mau biar data yang udah kamu buat besok bisa terbaca lagi harus pake file akses

oh iya rei untuk contoh programnya lagi sudah ada di directori ini. kamu tinggal cari yang input.cpp (ini untuk input data dari file ke program), output.cpp (ini untuk output data dari program ke file), io.cpp (ini untuk melakukan keduanya ya)
</p>



Untuk mendeklarasikan file akses kita perlu memasukan library standarnya
yaitu

    #include<fstream>


kemudian untuk menggunakan melakukan output ke dalam file yaitu dengan

    ofstream namaobjek;

dimana nama objek sesuai kebutuhakn kita. kita bisa saja menamakan objeknya hendra, budi, tas, dan lain lain

lalu untuk mencetak text ke dalam file yaitu menggunakan sintak

    namaobjek << "Hello World" ;

dimana "Hello World" adalah text yang akan tercetak didalam file tersebut

nah selain untuk mencetak text kedalam file, kita juga bisa mengambil data dari file agar bisa ditampung/ dicetak didalam program yang ada

caranya dengan menggunakan

    ifstream namaobjek;

untuk penamaan objek sesuai kebutuhan kita.

dan untuk mengambil isi filenya yaitu dengna

    namaobjek >> variabel_penampung;


oh iya setelah kita meninstansiasikan objek ofstream ataupun ifstream kita harus melakukan pembukaan terhadap file yang ada. caranya seperti ini

    namaobjek.open("namafile");

nah contohnya seperti ini

    //mencetak ke dalam file

    int main(){
        ofstream cetak;
        cetak.open("file.txt");
        cetak << "Hello World" << endl;
    }

    // mengambil data dari file

    int main(){
        ifstream input;
        string tampung;
        input.open("file.txt");
        input >> tampung;
        cout << tampung << endl;
    }


nah untuk dasarnya seperti itu. kalian bisa mengunduh program contohnya didalam folder ini



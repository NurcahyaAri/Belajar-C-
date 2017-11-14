# Apa itu C++
C++ adalah sebuah bahasa pemrograman yang dikembangkan dari bahasa C oleh Bjarne Stroustrup pada tahun 1980 an di Bell Labs. Salah satu kelebihan bahasa C++ dibandingkan bahasa C adalah dukungan terhadap konsep PBO (Pemrograman Berorientasi Objek)



# Table Konten : 
* [Sintak Dasar](#sintak-dasar)
* [Komentarin Sourcenya yuk biar tidak bingung](#komentar)
    * [Komentar sebaris](#komentar-sebaris)
    * [komentar lebih dari 1 baris](#komentar-lebih-dari-sebaris)
* [Kenalan dengan Tipe data dan Variabel yuk](#kenalan-dengan-tipe-data-dan-variabel-yuk)
    * [Tipe Data](#tipe-data)
    * [Variabel](#variabel)
    * [Operator Assignment](#operator-assignment)
* [Berhitung Matematika di C++ yuk](#berhitung-matematika-di-c-yuk)
* [Mari kita kontrol program kita](#mari-kita-kontrol-program-kita)


## Sintak Dasar
Untuk menulis kode program dengan C++ ada sintak dasarnya, dimana sintak tersebut sangatlah penting agar program dapat berjalan, karena jika tidak ada maka program tidak dapat berjalan sama sekali, atau bahkan error. Sintak dasarnya seperti ini :

    #include<iostream>
    using namespace std;

    int main(){

    }

Penjelasan kode :

    #include<iostream> 
    
 C++ melampirkan beberapa header dengan cara #include<file_header_yang_ingin_ditampilkan>,
oh iya #include itu termasuk preprocessor dan #include ini berguna untuk memanggil atau menambahkan file header.
setiap File header memiliki fungsi dan kegunaan tertentu salah satunya adalah iostream. 
iostream adalah library standar untuk melakukan operasi input maupun output dalam program 
yang kita tulis, salah satu sintak untuk melakukan input dan output adalah cin 
dan cout dimana cin adalah sintak untuk melakukan input dari keyboard dan
cout adalah sintak untuk mencetak kode program agar dapat tampil dilayar.
berikut ini adalah contoh sederhana dari input dan output program paling sederhana : 

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/basic%20input%20output%20.gif" alt="alt text" width="510px" height="267px" alt="input output sederhana" title="input output sederhana">

    using namespace std;

 untuk menggunakan standar library dari C++ maka kita harus menuliskan kode tersebut, karena jika tidak 
 dituliskan maka program yang kita buat akan error.

    int main(){

    }
 
terakhir adalah int main(), int main() sendiri adalah fungsi utama dalam program c++. setiap kode program yang ditulis akan dipanggil disini, jadi ketika program kalian jalankan maka semua baris yang ada di fungsi main inilah yang nantinya akan diproses, tetapi jika kalian menulis kode diluar main() dan tidak dipanggil didalam fungsi ini maka kode tersebut tidak akan diproses sama sekali


## Komentar
Ketika kita sudah menulis sebuah kode program terkadang kita juga bingung apa yang sudah kita tulis, atau kita malah lupa bagaimana proses program tersebut berjalan, dan juga kita sering kali lupa dan bertanya tanya "mengapa kita buat programnya seperti ini ya? gunanya sebenernya apa ini?" nah dengan adanya komentar ini kita dapat mengomentari kegunaan dari baris program yang sudah kita buat agar kita tidak bingung, selain itu komentar juga biasa digunakan untuk menulis lisensi program atau pengarang program tersebut. berikut ini adalah contoh komentar
<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/komentar.png" alt="alt text" alt="input output sederhana" title="input output sederhana">

disitu terlihat jelas bahwa komentar tidak akan ikut tampil ketika program dijalankan. oh iya komentar ada dua jenis, yaitu : 

### komentar sebaris
ketika kita hanya ingin mengomentari hanya satu baris program maka kita dapat menggunakan komentar jenis ini cara penggunaannya seperti ini
    // text yang ingin dijadikan komentar

### komentar lebih dari sebaris
sedangkan ketika kita ingin mengomentari 2 baris atau 3 atau mungkin 10 baris kita juga bisa, untuk mengomentari lebih dari 10 baris caranya seperti ini

    /* Nama saya Ari Nurcahya,
       Saya bingung mau nulis apa lagi
       Saya suka kucing, dan juga suka Dia*/

untuk komentar lebih dari 1 baris kita mulai dengna '/*' kemudian ditutup dengan '*/'

## Kenalan dengan Tipe data dan Variabel yuk
melakukan pemrograman bagaikan melakukan operasi matematika, dimana kita perlu memerlukan variabel.
2x + 3 = 10 adalah salah satu contoh dimana kita memerlukan variabel yang bernama x, dan x sendiri bernilai 4. 2x + 3 = 10; 2 adalah koefisien, x adalah variabel + adalah operator penjumlahan dan 3 adalah konstantan. dalam pemrograman kita bisa menulisnya 2 * x + 3; karena pada hakikatnya bahasa pemrograman tidak mengenal yang namanya koefisien

### Tipe Data
Tipe data apasih? dalam melakukan programming kita mungkin harus menulis sebuah Variabel, Konstanta, ataupun Fungsi. nah ketiga hal tersebut adalah contoh dimana kita membutuhkah tipe data. maksudnya adalah karena Variabel, Konstanta dan fungsi adalah sebuah data, jadi kita harus tau tipenya adalah apa.
Tipe data sendiri juga merepresentasikan bilangan yang akan kita gunakan. mungkin kita harus menggunakan bilangan bulat, atau mungkin pecahan. nah tapi perlu diketahui juga kita tidak mungkin bisa menggunakan data berupa pecahan pada tipe data bilangan bulat. beberapa tipe data yang mungkin memang harus dihafal dan diketahui adalah int (untuk bilangan bulat), float (bilangan pecahan), dan bool (untuk data berupa pernyataan benar dan salah)

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/tipe%20data.png" alt="alt text" alt="input output sederhana" width="492px" height="483px" title="Tabel tipe data">


### Variabel
Variabel adalah suatu hal yang bisa berubah ubah dan belum pasti, jika dalam programming variabel bisa juga diartikan sebagai sebuah penampung data yang nilainya dapat berubah ubah sesuai kebutuhakn kita. 
contoh nyata variabel adalah : 
- 2x + 2; dimana x adalah variabel, dan dia mempengaruhi hasilnya
- x = 2 + 2; x tersebut juga adalah variabel, dan x tersebut dicari nilainya

untuk mendeklarasikan variabel diperlukan beberapa syarat dimana
- nama variabel tidak boleh diawali angka
- nama variabel tidak boleh menggunakan angka
- nama variabel tidak boleh menggunakan spasi
- nama variabel tidak boleh sama dengan kata yang sudah ada dalam bahasa C++
- nama variabel tidak boleh menggunakan simbol (contoh *, =, :, dll)
- nama variabel di C++ bersifat Case-Sensitive, maksudnya adalah antara variabel nama dan variabel Nama adalah sesuatu yang berbeda, karena nama bukan kapital, sedangkan Nama adalah kapital

cara pendeklarasian variabel adalah : 

    tipe_data nama_variabel;

contoh : 

    int a;
    int variabel;
    float bilGanjil;
    float bilGanjil1;
    bool apakah_benar;
    char nama;

    kita juga bisa mendeklarasikan variabel sebaris, contoh

    int harga_sepeda, harga_motor, harga_mobil;

screenshoot pendeklarasian variabel : 
scrennshot ini adalah contoh salah dari pendeklarasian variabel

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/variabel%20error%201.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Error menamakan variabel">

penjelasan : pada gambar tersebut terjadi error karena kita tidak bisa mendeklarasikan dengan model seperti itu. karena dengan memberi tipe data lagi pada variabel berarti kita telah menyelesaikan baris tersebut, jadi seharusnya kita bukan menggunakan ',' (koma) tetapi seharusnya ';' (titik koma)

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/variabel%20error%202.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Error menamakan variabel">

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/variabel%20error%203.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Error menamakan variabel">

penjelasan : pada dua gambar diatas terjadi error karena salah dalam melakukan pemberian nama pada variabel, coba kalian lihat lagi syarat syarat dalam pemberian nama variabel kembali. disitu terlihat jelas kita tidak bisa melakukan penamaan menggunakan angka didepan ataupun spasi

lalu bagaimana cara mendeklarasikan variabel dengan benar?

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/variabel%20sukses.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Penamaan variabel yang benar">

terlihat ketika program dikompilasi tidak terjadi error sama sekali, karena penamaan variabel tersebut sudah sesuai aturannya

### Konstanta
Konstanta adalah nilai yang tidak dapat berubah dan sudah pasti. contoh konstanta yang jelas adalah nilai pi untuk menghitung linkaran, dimana pi selalu bernilai 3.14, tidak mungkin kan pi bernilai sesuka kita.

cara pendeklarasian pi sangat mirip dengan variabel, perbedannya hanyalah konstanta diawali kata kunci const. untuk mendeklarasian konstanta seperti ini : 

    const tipe_data nama_variabel;

perbedaan antara konstanta dengan variabel adalah dimana variabel bisa kita gunakan tanpa perlu memberi nilai sedangkan konstanta tidak bisa

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/konstanta%20error.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Pendeklarasian konstanta yang salah">

lalu bagaimana cara mendeklarasikan konstanta yang benar? yaitu dengan memberinya nilai atau [assignment](#assignment).

berikut ini adalah cara mendeklarasikan konstanta dengan benar

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/deklarasi%20konstanta.png" alt="alt text" alt="input output sederhana" width="632px" height="483px" title="Pendeklarasian konstanta yang benar">


### Operator Assignment
Assignment atau penugasan, adalah operator untuk memberikan nilai kepada variabel ataupun konstanta. cara untuk melakukan assignment atau penugasan adalah dengan menggunakan operator '=' (sama dengan)

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/assignment.gif" alt="alt text" alt="input output sederhana" width="668px" height="546px" title="Cara melakukan Pemberian nilai kepada variabel">


## Berhitung Matematika di C++ yuk

    2 + 2 = 4;
    x + y;
    1/2 * x * y;

berikut diatas adalah salah contoh perhitungan matematika. perhitungan di dalam matematika sendiri sudah pasti ada nilai (operand), operasinya (operator) dan hasilnya. di dalam pemrograman pun kurang lebih seperti itu. 

contoh 1 
kita mendapatkan persoalan menghitung jumlah uang kita sekarang (Rp. 50,000) dikurang harga makanan yang kita beli (Rp. 10,000), jajannya yang kita beli adalah inputan dari user. bagaimanakan penyelesaiannya?

untuk penyelesaiannya seperti gambar dibawah ini
<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/hitung_sederhana-min.gif" alt="alt text" alt="input output sederhana" title="Penyelesaian">


contoh 2
Menghitung luas lingkaran dengan jari jari sepanjan 7cm. bagaimana penyelesaiannya?

analisa untuk penyelesaian :
kita deklarasikan variabel untuk jari jari, nilai hasil, dan konstanta untuk nilai pi
setelah itu kita hitung dengan rumus 
luas = pi * r * r;

source code

    #include<iostream>
    using namespace std;

    int main(){
        float r, hasil;
        const float pi = 3.14;
        r = 7;
        hasil = pi * r * r;

        cout << "Luas lingkarannya adalah : " << luas << endl;
    }

penjelasan source code 

mengapa kita gunakan r, dan hasil bertipe float? ya betul sekali, karena hasil kemungkinan akan menampung nilai bertipe pecahan, dan r sebenarnya bisa menggunakan int tetapi agar lebih ringkas saja kita jadikan float

dan pi kita jadikan const karena nilai pi sudah pasti dan tidak mungkin berubah

### Operator Aritmatika

Operator Aritmatika adalah operator yang biasa digunakan untuk melakukan perhitungan matematika seperti penjumlahan, pengurangan, perkalian, pembagian

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/tabel aritmatika.png" alt="alt text" alt="Tabel Operasi Aritmatika" title="Penyelesaian">

### Operator Gabungan

Operator gabungan atau yang mungkin lebih dikenal dengan operasi unary adalah operasi aritmatika yang hanya menggunakan 2 variabel saja. jika biasanya kita menggunakan binary (hasil = a + b), maka jika dijadikan unary berarti hasil = a; hasil += b;

jenis oeprator Gabungan

    += (untuk menjumlahkan)
    -= (untuk mengurangkan)
    *= (untuk mengkalikan)
    /= (untuk membagikan)
    %= (untuk modulus)

Contoh merubah operasi binary menjadi operasi gabungan (unary)

    a = a + b; (binary)
    a += a; (unary)

    x = x * y;
    x *= y;

    luas = 1/2 * a * t (binary)
    unarynya maka : 
    luas = a;
    luas *= t;
    luas /= 2;

### Operator Kenaikan (increment) dan Penurunan (Decrement)
Operator ini dibagi menjadi dua jenis yaitu Increment (++) dan Decrement (--). oh iya untuk increment dan decrement masing masing ada 2 jenis. yaitu post increment, dan pre increment. kemudian post decrement, dan pre decrement

<b>Post Increment</b>
Operator Post Increment adalah operator penambahan nilai kepada variabel, dan dia akan menambahkannya terlebih dahulu

<b>Pre Increment</b>
Operator Pre Increment adalah operator penambahan nilai kepada variabel dan dia akan menambahkan sesudahnya

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/increment-decrement.png" alt="alt text" alt="Increment" title="Penyelesaian">

penjelasan perbedaan Post dan pre
d = ++c dan ketika d di outputkan ke layar monitor hasilnya adalah 1, karena nilai c dijumlahkan terlebih dahulu sebelum dbierikan nilainya kepada d

sedangkan ada e = d++ hasilnya bisa 1 juga karena nilai d yang diberikan kepada e belum dijumlahkan, tetapi setelah nilai diberikan ke variabel e nilai d baru dijumlahkan

<b>Post Decrement</b>
sama halnya dengan increment tetapi decrement akan melakukan penurunan nilai
<b>Pre Decrement</b>
sama halnya dengan increment tetapi decrement akan melakukan penurunan nilai

<img src="https://github.com/NurcahyaAri/Belajar-Cplusplus/blob/master/images/idecrement.png" alt="alt text" alt="Increment" title="Penyelesaian">


## Mari kita kontrol program kita

terkadang kita membutuhkan pemilihan keputusan di dalam program kita. jadi kita hanya butuh baris program ini saja yang diproses ketika kondisnya seperti ini, dan ketika kondisinya seperti itu maka kita akan memproses baris yang itu.

nah dengan kemamumpuan untuk mengkontrol program kita dapat membuat program berjalan semestinya, lalu maksudnya mengontrol itu apa saya masih bingung?

nah semisal kita akan mencetak 'saya suka dia' ketika nilai yang kita inputkan adalah bilangan ganjil saja, maka otomatis ketika nilai yang kita inputkan genap berarti tidak akan tampil apa apa di layar monitor kita.

untuk melakukan pengontrolan dalam program kita dapat menggunakan if, if..else, maupun switch case

### Kendalikan dengan If

syntax if

    if(kondisi){
        // pernyataan
    }











    



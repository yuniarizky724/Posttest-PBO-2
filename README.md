# Posttest-PBO-2
# Manajemen Penyewaan Busana di Butik
### Program ini dibuat dengan aplikasi Java untuk mengelola data penyewa busana di butik. fitur yang tersedia meliputi menambah pesanan, melihat daftar pesanan, mengubah dan menghapus data. Sedangkan semua data disimpan dalam ArrayList. program ini berjalan berulang dan akan berakhir hingga pengguna memilih menu keluar.

# Class Busana
<img width="466" height="231" alt="image" src="https://github.com/user-attachments/assets/98c818c9-11d3-4de7-ac52-46019a974fef" />
### Program ini dibuat dengan menggunakan struktur MVC (Model View Controller), yang mana setiap  3 package memiliki peran tanggung jawab spesifik.
### - Package Model
### - Package Service
### - Package Main

<img width="477" height="127" alt="image" src="https://github.com/user-attachments/assets/1bd006f3-f6b8-4280-955a-ceea669c8ef3" />
### Class Busana dideklarasikan sebagai public agar dappat diakses dari package lain dengan 3 atribut.

<img width="765" height="162" alt="image" src="https://github.com/user-attachments/assets/81fdf4b8-511e-4ccd-bd49-132aaeef9b68" />
### COnstructor dipakai untuk membuat objek baru. Kata kunci this digunakan untuk membedakan antara atribut class dan parameter constructor yang memiliki nama sama.

<img width="780" height="572" alt="image" src="https://github.com/user-attachments/assets/a1f56aa5-a670-4061-8c9a-2290cbd65cfb" />
### Getter digunakan untuk membaca nilai dan atribut, sedangkan setter digunakan untuk mengubah nilai pada atribut yang tersedia.

# Class Service

<img width="657" height="90" alt="image" src="https://github.com/user-attachments/assets/66421edc-11cb-4abb-9db3-20870936610a" />
### Kode diatas yaitu BusanaService yaitu untuk mengimpor Busana dari package model sehingga dapat membuat dan memanipulasi objek Busana. ArrayList digunakan untuk menyimpan semua Busana sementara di memory dan Scanner digunakan untuk membaca input.

<img width="922" height="86" alt="image" src="https://github.com/user-attachments/assets/48ece48a-b28c-4146-b3a7-43443a2f4251" />
### method Create yaitu meminta pelanggan untuk mengisi semua atribut yang tersedia. jika input data dari pelanggan valid, dibuat objek Busana baru dengan ID Busana dan dimasukkan ke list.

<img width="924" height="622" alt="image" src="https://github.com/user-attachments/assets/53983fc9-7f09-4239-9546-82932d7a6ea9" />
## method Create yaitu meminta pelanggan untuk mengisi semua atribut yang tersedia. jika input data dari pelanggan valid, dibuat objek Busana baru dengan ID Busana dan dimasukkan ke list.

<img width="850" height="279" alt="image" src="https://github.com/user-attachments/assets/c95a62a5-7cfb-4590-a129-786d5819dad4" />
### Method ini yaitu untuk menampilkan Busana. Jika list kosong, method berhenti. Alurnya membaca data dari model dan menampilkannya ke terminal atau output.

<img width="1049" height="569" alt="image" src="https://github.com/user-attachments/assets/6d0d0218-1be0-4eeb-a344-2d0490e1356b" />
### Method update meminta ID Busana yang harus diperbarui. 

<img width="1055" height="329" alt="image" src="https://github.com/user-attachments/assets/72f7c7d3-02ab-40f7-8113-6a32e54e0026" />
### Method Delete meminta ID, mencari objek list, dan menghapusnya jika ditemukan.

<img width="1051" height="495" alt="image" src="https://github.com/user-attachments/assets/bbdc829d-c787-4839-b470-f61d5d46d4b5" />
### Method ini dideklatrasikan public agar bisa dipanggil dari package lain, misalnya dari class Min. Method ini tidak mengembalikan nilai karena tujuannya adalah menampilkan hasil pencarian langsung. Jika tidak ada satu pun yang cocok (false), program menampilkan pesan bahwa tidak ada data yang sesuai.

# Class Main

<img width="477" height="89" alt="image" src="https://github.com/user-attachments/assets/91c49628-517b-4c01-a047-d427ef74754c" />
### kode di atas menandakan lass MainApp berada dalam package Main. Dengan ini, package lain harus melakukan import untuk bisa mengakses MainApp. Package Main berfungsi sebagai View dalam arsitektur MVC, tempat menampilkan menu dan menerima input user..

<img width="731" height="168" alt="image" src="https://github.com/user-attachments/assets/ece7ad68-0613-4738-a1be-dd34abc91215" />
### Class Main dideklarasikan public agar bisa diakses dari luar package, dan method main adalah titik awal program dijalankan oleh Java. Semua alur program dimulai dari sini. kemudian dibuat objek scanner untuk membaca input dari user, ini menjadi kontrol alur program, apakah user ingin menambah, menampilkan, mengubah, menghapus, mencari data, atau keluar.

<img width="865" height="300" alt="image" src="https://github.com/user-attachments/assets/7a943fed-efe4-4a2c-95d3-30e24c36f9bd" />
### kode di atas adalah bagian menu utama ditampilkan ke user. setiap opsi menu diarahkan untuk menjalankan method tertentu di service. User bisa melihat pilihan dan menentukan operasi yang ingin dilakukan.

<img width="1046" height="326" alt="image" src="https://github.com/user-attachments/assets/165e046b-bfc4-458a-a03b-83872b824065" />
### bagian kode ini adalah pengendali menu utama. Switch case mengecek pilihan user dan memanggil method yang sesuai di Busana untuk menambah, menampilkan, mengubah, menghapus, atau mencari Busana. pilihan 6 menghentikan program, sedangkan input yang tidak valid akan menampilkan pesan error.

<img width="401" height="204" alt="image" src="https://github.com/user-attachments/assets/d7ce4f94-eb9d-4f1f-9746-884310813637" />
### Output dari Main

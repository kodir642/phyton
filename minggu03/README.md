Nama  : heru dwi pangestu
nim   : 185410038

List 
Memiliki beberapa method dalam tipe data list. sebagai berikut:
list.append(x) = ( Menambahkan item pada akhir list. Sama dengan a[len(a):] = [x]. )
list.extend(itterable) = ( Memperluas list dengan menambahkan semua item dari iterable. Sama dengan a[len(a):] = iterable. )
list.insert(i,x) = ( Menyisipkan item pada posisi tertentu didalam list. Argument pertama adalah indeks elemen yang akan disisipkan, jadi menyisipkan di depan list tersebut. a.insert(len(a), x) sama dengan a.append(x). )
list.remove(x) = ( Menghapus item yang ditunjuk x. jika item yang dimaksud tidak ada, maka akan menghasilkan valueError. )
list.pop([i]) = ( Digunakan untuk menghapus elemen dalam list (oleh bawaan elemen terakhir), dan mengembalikan nilai dari elemen. )
list.clear() = ( Menghapus semua item dari list. Sama dengan del a[:]. )
list.index(x[,start[,end]]) = ( Mencari posisi suatu nilai )
list.count(x) = ( Menghitung kemunculan nilai tertentu. )
list.sort(*, key=None, reverse=False) = ( Mengurutkan list. )
list.reverse() = ( Membalik urutan list. )
list.copy() = ( Untuk menduplikat/menyalin list )
contoh penggunaan method di atas ini, sebagai berikut :
 

List sebagai stack
Stack  sangat cocok digunakan dengan Metode list, elemen terakhir yang di tambahkan merpakan elemen pertama yang diambil (terakhir-keluar, masuk-pertama). Untuk menambahkan item ke atas stack, gunakan append(). Untuk mengambil item dari atas stack, gunakan pop() tanpa menulis indeks. Contoh :
 
List sebagai antrian
elemen pertama yang ditambahkan adalah elemen pertama yang diambil (pertama-masuk, pertama-keluar). Akan tetapi, list kurang efisien untuk tujuan ini, sebab melakukan penyisipan atau pop dari awal list akan lambat hal itu di karenakan semua elemen lainnya akan digeser satu per satu). Dan Untuk mengimplementasikan antrian, gunakan collections.dequeyang dirancang untuk memiliki penambahan cepat dan muncul dari kedua ujungnya. 
Contoh:
 
Pemahaman list memberikan cara yang ringkas untuk membuat list. Aplikasi umum adalah membuat list baru di mana setiap elemen adalah hasil dari beberapa operasi yang diterapkan ke setiap anggota urutan lain atau dapat diulang, atau untuk membuat rangkaian elemen yang memenuhi kondisi tertentu. Misalnya, anggap kita ingin membuat list kotak, seperti:
 
 
 

List comprehensions
Ekspresi awal dalam pemahaman list dapat berupa ekspresi sembarang apa pun, termasuk pemahaman list lainnya
 
list comprehension berikut akan mengubah baris dan kolom:
 
listcomp bersarang dievaluasi dalam konteks for yang mengikutinya 
 

Del statemnet
menghapus item dari daftar yang diberikan indeksnya
 
Del juga dapat digunakan untuk menghapus seluruh variable del a

Tuples and Sequences 
Tupel adalah urutan, seperti daftar. Perbedaan utama antara tupel dan daftarnya adalah bahwa tupel tidak dapat diubah tidak seperti List Python. Tupel menggunakan tanda kurung, sedangkan List Python menggunakan tanda kurung siku.
  
Sets
Satu set adalah koleksi tidak berurutan tanpa elemen duplikat. Set objek juga mendukung operasi matematika seperti penyatuan, persimpangan, perbedaan, dan perbedaan simetris. Tanda kurung kurawal atau set() fungsinya dapat digunakan untuk membuat set.
 
 

Dictionaries
dictionary diindeks oleh keys, yang dapat berupa jenis apa pun yang tidak dapat diubah immutable type; string dan angka selalu bisa menjadi kunci key
 
dict()konstruktor membangun kamus langsung dari urutan pasangan kunci-nilai:
 
Selain itu, pemahaman dict dapat digunakan untuk membuat kamus dari ekspresi kunci dan nilai yang berubah-ubah:
 
Jika kuncinya adalah string sederhana, terkadang lebih mudah untuk menentukan pasangan menggunakan argumen kata kunci:
 

Looping Techniques

Saat mengulang kamus dictionaries, kunci key dan nilai value terkait dapat diambil pada saat yang sama menggunakan metode items() Saat mengulang melalui urutan, indeks posisi dan nilai terkait dapat diambil pada saat yang sama menggunakan fungsi enumerate() Untuk mengulang dua urutan atau lebih secara bersamaan, entri dapat dipasangkan dengan fungsi zip() Untuk mengulang urutan secara terbalik, pertama tentukan urutan dalam arah maju dan kemudian panggil fungsi reversed()
 


Saat melakukan perulangan melalui suatu urutan, indeks posisi dan nilai terkait dapat diambil pada saat yang sama menggunakan enumerate()fungsi tersebut
 
Untuk mengulang lebih dari dua atau lebih urutan pada saat yang sama, entri dapat dipasangkan dengan zip()fungsi tersebut.
 
Untuk mengulang urutan secara terbalik, pertama-tama tentukan urutan dalam arah maju dan kemudian panggil reversed()fungsinya.
 
Untuk mengulang urutan dalam urutan terurut, gunakan sorted()fungsi yang mengembalikan daftar terurut baru sambil membiarkan sumber tidak berubah.
 
Menggunakan set()secara berurutan menghilangkan elemen duplikat. Penggunaan sorted()kombinasi dengan set()lebih dari satu urutan adalah cara idiomatik untuk mengulang elemen unik dari urutan dalam urutan yang diurutkan.
 
Terkadang Anda tergoda untuk mengubah daftar saat Anda mengulanginya; naTerkadang Anda tergoda untuk mengubah daftar saat Anda mengulanginya; namun, seringkali lebih sederhana dan lebih aman untuk membuat daftar baru.mun, seringkali lebih sederhana dan lebih aman untuk membuat daftar baru.
 

More on Conditions
Perhatikan bahwa dalam Python, tidak seperti C, penugasan di dalam ekspresi harus dilakukan secara eksplisit dengan operator walrus :=. Ini menghindari masalah kelas umum yang dihadapi dalam program C: mengetikkan = dalam ekspresi ketika == dimaksudkan.
 

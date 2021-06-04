# Metode-Numerik-2021
Dibuat oleh Tim Kelompok 10 Oseanografi Tahun Ajaran 2020/2021

Nama Anggota Kelompok : (Nama_NIM_Kelas)
1. Istikhanah_26050119120029_A
2. Rhieni Rahma Aulia_26050119120028_B
3. Talitha Sari Ismaniar_26050119120027_B
4. Achmad Usamah_26050119120026_A
5. Nur Hasanah_26050119120024_B
6. Muhammad Irsad Khairi_26050119120023_B
7. Muhammad Faqih Fajri_26050119120022_B
8. Yoas Heryanto_26050119120020_B
9. Rohmatun Dwi Astuti_26050119120019_B
10. Siti Hamidah_26050119120018_B
11. Muhammad Fakhri_26050119130043_B

  Repository ini dibuat untuk memenuhi tugas akhir praktikum Metode Numerik tahun ajaran 2020/2021, didalamnya terdapat aplikasi yang dapat digunakan untuk menyelesaikan permasalahan secara metode numerikal. Cara untuk menjalankan aplikasi penyelesaian secara metode numerikal ini hanya tinggal run dan memasukkan (input) angka-angka yang diperlukan, agar dapat menampilkan hasil. Perlu diketahui bahwa Library pada Python merupakan sebutan untuk kode program tambahan yang digunakan untuk kebutuhan tertentu. Modul adalah objek Python dengan atribut yang diberi nama yang bisa dibind dan dijadikan referensi, dimana di dalamnya mendefinisikan fungsi, kelas, dan variabel. Aplikasi penyelesaian numeris pada repository ini dibuat dengan menggunakan bahasa Python dengan library Matplotlib, Numpy, Scipy, modul Sys dan masih banyak lagi komponen di dalamnya. Pada aplikasi ini dibuat suatu penyelesaian numeris dalam bentuk code bahasa Python mulai dari modul 2 hingga modul 5 praktikum dengan setiap metodenya menggunakan fungsi (def). Fungsi (def) pada Python adalah kumpulan perintah atau baris kode yang dikelompokkan menjadi satu kesatuan untuk kemudian bisa dipanggil atau digunakan berkali-kali, jadi fungsi (def) ini akan membuat kode program menjadi lebih terstruktur dan re-usable.

Berikut adalah rincian metode (modul 2 sampai modul 5) yang telah kami susun dalam repository Tugas Akhir ini:
	
	MODUL 2: Akar-Akar Persamaan
	1. Metode Setengah Interval
	2. Metode Interpolasi Linier
	3. Metode Newton-Rapson
	4. Metode Secant
	5. Metode Iterasi

	MODUL 3: Sistem Persamaan Linier dan Matriks
	1. Metode Gauss
	2. Metode Gauss-Jordan
	3. Metode Gauss-Seidel
	4. Metode Jacobi

	MODUL 4: Integrasi Numerik
	1. Metode Trapesium Banyak Pias
	2. Metode Simpson 1/3

	MODUL 5: Persamaan Diferensial Biasa
	1. Metode Euler
	2. Metode Heun
  
# Cara Penggunaan Executable File (.exe)💻
  Secara bahasa exe adalah bahasa singkatan dari executable, format file ini sebagian besar digunakan untuk program pada DOS, Windows, dan platform lainnya. File exe dapat berisi resource (sumber daya), grafik bitmap, ikon, dan komponen lainnya untuk menjalankan program yang dapat dieksekusi yang juga berada di file exe. Format file executable ini dapat dikompres dengan kompresor yang dapat dieksekusi seperti paket runtime dan dapat diekstraksi kembali.
  Berdasarkan pengertian tersebut, perlu diperhatikan bahwa file (.exe) yang kami lampirkan dalam repository ini berkaitan dengan directory file dalam penggunaannya, maka terdapat beberapa bagian script yang harus disesuaikan. Berikut adalah langkah dalam menggunakan file (.exe):

1. Pengguna dapat mengunduh folder Kelompok 10 pada repositori ini. 
2. Buka file codemetnum10.py pada folder code. 
3. Pada bagian Modul 4: Metode Trapesium 1 Pias, ubah directory file sesuai dengan lokasi directory file folder image anda. Hal yang sama juga dilakukan pada Modul 4: Metode Trapesium Banyak Pias dan Modul 5: Metode Euler dan Heun. Sesuaikan akhiran directory file dengan metode yang digunakan. plt.savefig('C:\Kelompok 10\Images*NamaMetode*.png')
4. Simpan file codemetnum10.py. 
5. Buka file setup.exe. Lalu ikuti perintah yang terdapat pada program.

# Tentang MODUL 2: Akar-Akar Persamaan
1. Metode Setengah Interval

    Metode setengah interval merupakan metode analisis numerik paling sederhana diantara metode-metode analisis lainnya. Metode ini termasuk metode yang tangguh, meskipun metode ini sangat sederhana namun selalu dapat menemukan akar persamaan yang dicari. Kelebihan dari metode ini adalah selalu berhasil dalam menentukan akar-akar yang dicari atau dengan kata lain selalu konvergen. Selain kelebihan, dalam metode ini juga terdapat kekurangan, yaitu hanya dapat dilakukan apabila ada akar persamaan pada interval yang diberikan. Jika terdapat beberapa akar pada interval yang diberikan maka hanya satu akar saja yang dapat ditemukan.
  
    Metode Setengah Interval merupakan metode penyelesaian persamaan non linear yang sederhana, dimana apabila diberikan suatu persoalan mengenai perhitungan salah satu akar dari persamaan, yang pertama kita lakukan adalah menghitung nilai f(x) pada interval dua titik yakni Xn dan Xn+1, lalu dengan mengingat fungsi adalah kontinyu, maka perubahan tanda dari fungsi antara kedua buah x tersebut akan memotong sumbu x paling tidak satu kali. Titik perpotongan antara sumbu x dan fungsi merupakan akar-akar persamaan. Selanjutnya yaitu membuat interval berikutnya untuk membuat interval yang semakin kecil, dimana akar persamaan berada. Hal yang sama dilakukan secara berulang menggunakan sistem iterasi untuk perhitungan interval-interval berikutnya hingga semakin kecil dimana akar persamaan berada yang bisa disesuaikan dengan suatu nilai ketelitian yang diminta. 

2. Metode Interpolasi Linier

    Metode interpolasi linier hampir mirip dengan metode setengah interval. Prinsip pencarian akar persamaan dari metode ini didasarkan pada penggunaan interpolasi linier. Interpolasi linier dilakukan melalui dua titik pertama dengan garis interpolasi memotong sumbu x dan dititik perpotongan tersebut didapatkan pendekatan akar yang pertama. Kemudian pendekatan tersebut dievaluasi pada fungsi nonlinier sehingga diperoleh titik pada fungsi nonlinier tersebut. Kemudian dilakukan lagi interpolasi melalui ujung sebelumnya dan diperoleh pendekatan akar berikutnya.
    
    Interpolasi jenis linier merupakan program atau metode yang digunakan untuk menentukan nilai antara dua persamaan linier (disebut juga persamaan garis lurus). Disebut sebagai persamaan garis lurus karena merupakan hasil persamaan linier dengan bentuk kurva pada grafik membentuk garis lurus. Yang dapat dilakukan dalam melakukan suatu metode interpolasi linier yaitu menghubungkan 2 titik dengan sebuah garis lurus, dimana pendekatan formulasi interpolasi linier sama dengan persamaan garis lurus. Selanjutnya diketahui bahwa suatu pendekatan formulasi interpolasi linier sama dengan persamaan garis lurus. Untuk memperbaiki kondisi tersebut dilakukan sebuah interpolasi dengan membuat garis yang menghubungkan titik yaitu melalui orde 2, orde 3, orde 4, dst, yang sering juga disebut interpolasi kuadratik, kubik, dst. Sehingga dapat diambil kesimpulan bahwa Interpolasi linier merupakan salah satu metode yang digunakan untuk mengetahui nilai dari suatu interval dua buah titik yang terletak dalam satu garis lurus, dimana metode ini dibuat dari kumpulan titik-titik dan titik yang membentuk garis lurus maupun lengkung dapat berubah bentuk menjadi wujud gambar yang lebih komplek.

3. Metode Newton-Raphson 
  
    Metode Newton-Raphson merupakan metode yang sederhana,namun cukup handal dalam mendapatkan akar persamaan nonlinier, dengan catatan terkaan awal yang diberikan cukup dekat. Metode Newton-Raphson tidak memerlukan dua buah terkaan awal, melainkan cukup satu saja tetapi diusahakan terkaan tersebut cukup dekat dengan akar persamaan yang dicari. Metode Newton-Raphson memiliki laju konvergensi lebih cepat, akan tetapi, syarat yang harus dipenuhi adalah bahwa taksiran awal yang diberikan harus sedekat mungkin dengan harga eksaknya. Metode Newton-Raphson memiliki kelebihan dan kekurangan. Kelebihan dari metode Newthon-Raphson adalah nilai yang konvergensi yang dihasilkan lebih cepat. Sedangkan kelemahan dari metode ini adalah tidak selalu menemukan akar (divergen) , kemungkinan sulit dalam mencari f’(xn) dan penetapan harga awal (xn) yang sulit.
  
    Metode Newton-Raphson merupakan metode penyelesaian persamaan non-linier dengan menggunakan pendekatan satu titik awal dan mendekatinya dengan memperhatikan slope atau gradien. Metode ini banyak digunakan dalam mencari akar-akar dari suatu persamaan. Langkah yang dilakukan dalam metode ini yaitu dimulai dari memilih nilai awal Xi secara sembarang, lalu menghitung nilai Xi+1 dan f(Xi+1) secara iterasi sehingga didapatkan nilai f(Xi+1) yang kecil dan bisa disesuaikan dengan nilai ketelitian yang diminta. Perlu diketahui bahwa dalam hal ini, slope atau gradien pada titik awal dan titik yang mendekatinya diperhatikan dan titik pendekatan ke n+1 ditulis sebagai Xn+1=Xn-(f(Xn)/f'(Xn)). Kelebihan Metode Newton-Raphson adalah bila taksiran awal kebetulan memang mendekati akar yang sesungguhnya maka waktu yang dibutuhkan untuk menghitung akar lebih cepat. Kekurangan Metode Newton-Raphson adalah bila taksiran awal tidak tepat, hasilnya justru akan divergen (semakin menjauhi nilai akar yang sebenarnya).

4. Metode Secant
    
    Metode Secant pada dasarnya metode Secant sama dengan metode Newton-Raphson, perbedaannya hanya terletak pada pendekatan untuk turunan pertama dari f saja. Pendekatan f' pada metode Secant didekati dengan ungkapan beda hingga yang didasarkan pada taksiran akar sebelumnya (beda mundur), yaitu disebut juga Metode Interpolasi Linear, dalam prosesnya tidak dilakukan penjepitan akar [x0, x1] dan tidak harus mengandung akar yang akan dicari, sehingga f(x0) dan f(x1) bisa bertanda sama serta iterasi berlangsung sampai batas maksimum atau sampai dipenuhinya batas Toleransi (T).
  
    Metode Secant merupakan perbaikan dari metode regula-falsi dan Newton Raphson, dimana kemiringan dua titik dinyatakan secara diskrit dengan mengambil bentuk garis lurus yang melalui satu titik. Kelebihan Metode Secant adalah dapat digunakan untuk mencari akar- akar persamaan dari persamaan polinomial kompleks, atau persamaan yang turunan pertamanya sangat sulit didapatkan. Metode Secant ini dibuat sebagai perbaikan dari metode Newton, yaitu nilai turunan f'(x) didekati dengan beda hingga. Langkah dalam metode Secant ini yaitu dimulai dengan menentukan X0, X1, toleransi, dan jumlah iterasi maksimum. Lalu, menghitung Xbaru = X1 - f(X1)( X1- X0)/f(X1) –f(X0). Jika nilai mutlak (Xbaru - X1) < toleransi, maka diperoleh tulisan xbaru sebagai hasil perhitungan, namun jika tidak, lanjutkan ke langkah berikutnya. Jika jumlah iterasi > iterasi maksimum, program diakhiri namun jika X = Xbaru, program dilakukan berulang kembali ke langkah kedua yakni perhitungan Xbaru sampai dengan didapatkan nilai akar persamaan sesuai dengan nilai ketelitian yang diminta.

5. Metode iterasi (tidak langsung) 
    
    Di dalam matematika, iterasi dapat diartikan sebagai suatu proses atau metode yang digunakan secara berulang-ulang (pengulangan) dalam menyelesaikan suatu permasalahan matematik. Metode iterasi merupakan metode yang berbasiskan terhadap aplikasi dari langkah algoritma sederhana yang diulang-ulang pada sistem persamaan tersebut hingga sistem persamaan mencapai keadaan konvergen yang merepresentasikan solusi dari suatu sistem persamaan. Pada metode iterasi, banyaknya langkah-langkah perhitungan yang dilakukan tidak dapat diprediksi, dimana tipikalnya adalah sebanyak N perhitungan per satu kali iterasi. Kekurangan lainnya adalah, jika sistem persamaan tidak berada pada kondisi yang kondusif, maka konvergensi dari suatu sistem persamaan tidak dapat terjamin. Kelebihan dari penggunaan metode iterasi adalah sedikitnya memori komputer yang digunakan sebagai akibat dari algoritma yang mendesain agar komputer hanya menyimpan koefisien-koefisien yang tidak nol. Metode iterasi adalah metode yang memisahkan x dengan sebagian x yang lain sehingga diperoleh : x=g(x).
  
# Tentang MODUL 3: Sistem Persamaan Linier dan Matriks
1. Metode Gauss 
  
    Metode Gauss adalah suatu cara mengoperasikan nilai-nilai di dalam matriks menjadi matriks yang lebih sederhana dan banyak digunakan dalam penyelesaian sistem persamaan linier. Prosedur penyelesaian dari metode ini adalah dengan melakukan operasi baris menjadi matriks eselon-baris. Metode ini mengubah persamaan linear tersebut ke dalam matriks augmentasi dan mengoperasikannya. Metode eliminasi gauss termasuk dalam metode penyelesaian persamaan linear dengan cara langsung. Metode Gauss ini adalah membawa persamaan kedalam bentuk matriks dan menyederhanakan matriks menjadi bentuk segitiga atas. Setelah mendapat bentuk matriks tersebut dilakukan subtitusi balik untuk mendapat nilai dari akar persamaan.

2. Metode Gauss-Jordan 
  
    Metode Gauss-Jordan adalah pengembangan dari eliminasi Gauss yang hasilnya lebih sederhana lagi. Metode ini meneruskan operasi baris dari eliminasi Gauss sehingga menghasilkan matriks yang Eselon-baris dan juga dapat digunakan sebagai salah satu metode penyelesaian persamaan linear dengan menggunakan matriks. Metode Gauss-Jordan juga dapat digunakan untuk mencari invers dari sebuah matriks.

3. Metode iterasi Gauss-Seidel 
  
    Metode iterasi Gauss-Seidel adalah metode yang menggunakan proses iterasi hingga diperoleh nilai-nilai yang berubah-ubah dan akhirnya relatif konstan. Metode iterasi Gauss- Seidel dikembangkan dari gagasan metode iterasi pada solusi persamaan tak linier. Metode eliminasi gauss-seidel digunakan untuk menyelesaikan SPL yang berukuran kecil karena metode ini lebih efisien. Dengan metode iterasi Gauss-Seidel toleransi pembulatan dapat diperkecil karena iterasi dapat diteruskan sampai seteliti mungkin sesuai dengan batas toleransi yang diinginkan. Kelemahan dari metode ini adalah masalah pivot (titik tengah) yang harus benar–benar diperhatikan, karena penyusunan yang salah akan menyebabkan iterasi menjadi divergen dan tidak diperoleh hasil yang benar.

4. Metode iterasi Jacobi 
  
    Metode iterasi Jacobi digunakan untuk menyelesaikan persamaan linier yang proporsi koefisien nol nya besar. Iterasi dapat diartikan sebagai suatu proses atau metode yang digunakan secara berulang-ulang (pengulangan) dalam menyelesaikan suatu permasalahan matematika. Kelebihan dari metode ini adalah langkah penyelesaiannya yang sederhana, sedangkan kelemahannya adalah proses iterasinya lambat. Terutama untuk persamaan linear serentak dengan ordo tinggi dan hanya dapat digunakan menyelesaikan persamaan linear serentak.
  
# Tentang MODUL 4: Integrasi Numerik
    
   Integrasi numerik merupakan cara alternatif untuk mengintegrasikan suatu persamaan, disamping integrasi analitis. Integrasi analitis terkadang merupakan cara integrasi yang sulit, khususnya pada persamaan-persamaan yang kompleks dan rumit. Dalam integrasi numerikal untuk penyelesaian berbagai permasalah numeris di sini dapat menggunakan empat buah metode yaitu antara lain:

1. Metode Trapesium Banyak Pias
  
    Metode trapesium merupakan metode pendekatan integral numerik dengan persamaan polinomial order satu. Dalam metode ini kurve lengkung dari fungsi f (x) digantikan oleh garis lurus. Pada metode trapesium satu pias memberikan kesalahan sangat besar. Untuk mengurangi kesalahan yang terjadi maka kurve lengkung didekati oleh sejumlah garis lurus, sehingga terbentuk banyak pias. Luas bidang adalah jumlah dari luas beberapa pias tersebut. Semakin kecil pias yang digunakan, hasil yang didapat menjadi semakin teliti. Metode trapesium dapat digunakan untuk integral suatu fungsi yang diberikan dalam bentuk numerik pada interval diskret.

2. Metode Simpson 1/3
    
    Kaidah simpson 1/3 adalah kaidah yang mencocokkan polinomial derajat pada tiga titik data diskrit yang mempunyai jarak yang sama. Hampiran nilai integrasi yang lebih baik dapat ditingkatkan dengan menggunakan polinom interpolasi berderajat yang lebih tinggi. Rumus Simpson dapat diturunkan berdasarkan deret Taylor. Metode simpson 1/3 dapat menghasilkan ketelitian orde 3 dan hanya memerlukan 3 titik. Pada simpson 1/3 hanya berlaku untuk jumlah pias genap.
  
3. Metode Trapesium 1 Pias
  
    Metode trapesium merupakan metode pendekatan integral numerik dengan persamaan polinomial order satu. Dalam metode ini kurve lengkung dari fungsi f (x) digantikan oleh garis lurus. Seperti pada Gambar 1, luasan bidang di bawah fungsi f (x) antara nilai x = a dan nilai x = bdidekati oleh luas satu trapesium yang terbentuk oleh garis lurus yang menghubungkan f (a) dan f (b) dan sumbu-x serta antara x = a dan x = b. Pendekatan dilakukan dengan satu pias (trapesium).
  
4. Metode Simpson 3/8
  
    Metode Simpson 3/8 diturunkan dengan menggunakan persamaan polinomial order tiga yang melalui empat titik Metode Simpson 1/3 biasanya lebih disukai karena mencapai ketelitian order tiga dan hanya memerlukan tiga titik, dibandingkan metode Simpson 3/8 yang membutuhkan empat titik. Dalam pemakaian banyak pias, metode Simpson 1/3 hanya berlaku untuk jumlah pias genap. Apabila dikehendaki jumlah pias ganjil, maka dapat digunakan metode trapesium. Tetapi metode ini tidak begitu baik karena adanya kesalahan yang cukup besar. Untuk itu kedua metode dapat digabung, yaitu sejumlah genap pias digunakan metode Simpson 1/3 sedangkan 3 pias sisanya digunakan metodeSimpson 3/8.
  
# Tentang MODUL 5: Persamaan Diferensial Biasa
   
   Persamaan diferensial adalah persamaan yang memuat turunan satu atau beberapa fungsi yang tak diketahui. Persamaan diferensial biasa hanya mengandung satu variabel atau satu peubah bebas. Metode satu langkah persamaan diferensial biasa ilaha metode euler maupun metode heun.

1. Metode Euler 
    
    Metode Euler merupakan metode yang dapat diturunkan dari Deret Taylor. Metode Euler menggunakan garis tangen ke fungsi di awal interval sebagai perkiraan kemiringan fungsi selama interval, dengan asumsi bahwa jika ukuran langkah kecil, kesalahan akan menjadi kecil. Metode Euler digunakan sebagai dasar untuk metode Heun. Metode ini pada dasarnya adalah merepresentasikan solusinya dengan beberapa suku deret Taylor. Metode Euler adalah salah satu dari metode satu langkah yang paling sederhana. Di banding dengan beberapa metode lainnya, metode ini paling kurang teliti. Namun demikian metode ini perlu dipelajari mengingat kesederhanaannya dan mudah pemahamannya.
    
    Metode Euler menggunakan garis tangen ke fungsi di awal interval sebagai perkiraan kemiringan fungsi selama interval, dengan asumsi bahwa jika ukuran langkah kecil, kesalahan akan menjadi kecil. Namun, bahkan ketika ukuran langkah sangat kecil digunakan, lebih dari sejumlah besar langkah kesalahan mulai menumpuk dan estimasi menyimpang dari nilai fungsional aktual. Metode Euler digunakan untuk memperkirakan secara kasar koordinat titik berikutnya dalam solusi, dan dengan pengetahuan ini, perkiraan awal diprediksi ulang atau diperbaiki. Dengan asumsi kuantitas f(x,y) di sisi kanan persamaan dapat dianggap sebagai kemiringan dari solusi yang dicari di titik mana pun (x,y), ini dapat dikombinasikan dengan estimasi Euler dari titik berikutnya untuk memberikan kemiringan garis singgung di titik akhir kanan. Selanjutnya rata-rata kedua lereng digunakan untuk menemukan koordinat yang diperbaiki dari interval ujung kanan.
    
    Metode Euler mengandung dua macam galat, yaitu galat pemotongan (truncation error) dan galat longgokan (cumulative error).  Metode Euler memberikan hampiran solusi yang buruk, sehingga dalam praktek metode ini kurang disukai, namun metode ini membantu untuk memahami gagasan dasar metode penyelesaian PDB dengan orde yang lebih tinggi. Dapat dikatakan bahwa metode Euler mempunyai ketelitian yang rendah, karena galatnya besar (sebanding dengan h). Oleh karena itu, metode Euler diperbaiki oleh metode Heun (modified Euler's method).

2. Metode Heun 
    
    Metode Heun adalah salah satu metode numerik yang dapat digunakan untuk menyelesaikan berbagai persoalan matematika yang mempunyai masalah nilai awal. Metode ini melibatkan 2 buah persamaan. Persamaan pertama disebut sebagai persamaan prediktor yang digunakan untuk memprediksi nilai integrasi awal. Persamaan kedua disebut sebagai persamaan korektor yang mengoreksi hasil integrasi awal. 
    
     Metode Heun merupakan metode prediktor-korektor, akan tetapi bukan termasuk metode banyak langkah. Pada metode Heun, solusi dari metode Euler dijadikan sebagai solusi perkiraan awal (predictor). Selanjutnya, solusi perkiraan awal ini diperbaiki dengan metode Heun (corrector). Persamaan Heun: yr+1 = yr + h/2 [f(xr, yr) + f(xr+1, yr+1)]. Dalam persaman tersebut, suku ruas kanan mengandung yr+1. Nilai yr+1 ini adalah solusi perkiraan awal (predictor) yang dihitung dengan metode Euler. Karena itu, persamaan Heun dapat ditulis sebagai Predictor : y(0)r+1 = yr + hf(xr, yr) dan Corrector : yr+1 = yr + h/2 [f(xr, yr) + f(xr+1, y(0)r+1)] atau ditulis dalam satu kesatuan, yr+1 = yr + h/2[f(xr,yr) + f(xr+1, yr + hf(xr, yr)]. Keakuratan metode Euler hanya meningkat secara linier dengan ukuran langkah berkurang, sedangkan Metode Heun meningkatkan akurasi secara kuadratik.
  
# Kesan
  Ucapan terimakasih tidak lupa diberikan kepada asisten-asisten yang sudah mengajarkan kepada praktikan mengenai dasar-dasar metode numerik meskipun kondisi masih belum bisa offline. Belajar mengenai penyelesaian persaamaan yang tidak sederhana melalui komputer dijalankan oleh Python tentunya suatu pengalaman baru bagi praktikan untuk berkembang lagi dalam mencari ilmu. Terimakasih buat semua ilmu yang telah diberikan asisten dalam praktikum metode numerik di tahun ajaran 2020/2021 ini.
  
# Pesan
  Semoga praktikum kedepannya semakin rinci dalam menjelaskan mengenai script yang digunakan fungsi serta mengapa memakai hal tersebut agar praktikan lebih memahami lebih dalam lagi. Serta semoga modul praktikum semakin lengkap dengan penjelasan dari masing-masing script yang akan digunakan dan semoga ilmu yang dipelajari bisa bermanfaat digunakan dalam oseanografi.

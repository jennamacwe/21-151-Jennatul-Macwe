Nama	: Jennatul Macwe

NIM		: 210411100151



aplikasi yang dibutuhkan :

1. Postgres
2. Xammp
3. Power Bi
4. membuat akun elephantsql.com


Langkah-langkah untuk mengumpulkan data dari beberapa sumber database 

1. **database menggunakan server cloud** di postgres

   **langkah pertama** 

   membuat intance pada akun elephantsql.com yang diberi nama pendatab yang akan digunakan untuk server cloud.![Screenshot_20230302_041733](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_041733.png)

   ​

   **langkah kedua** menghubungkan server dari elephantsql.com ke postgress dengan cara :

   a. klik kanan pada server > klik menu registrasi > klik server![Screenshot_20230302_032703](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_032703.png)

   ​

   b. memberi nama server

   ![Screenshot_20230302_033732](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_033732.png)

   ​

   c. mengisi bagian connection sesuai dengan server pada intance pendata_b akun elephantsql.com

   - host name/address diisi dengan server

   - maintenance database dan username diisi dengan user & default database

   - password diisi dengan password yang tertera pada detail intance elephant

   - kemudian klik tombol save, maka server pendatab berhasil dibuat.

     ![Screenshot_20230302_041957](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_041957.png)

**langkah 3** membuat table data iris 

- membuka database berdasarkan nama user & default database dari intance akun elepant yaitu isndkxax

![Screenshot_20230302_041342](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_041342.png)

- klik kanan pada menu table dan pilih menu Query Tool

- pada bagian query tuliskan query create table dari data yang ingin dimasukan

  ![Screenshot_20230302_042438](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_042438.png)

  kemudian run code tersebut dan refres pada menu table > klik kanan > klik refresh untuk memunculkan table irish

  ![Screenshot_20230302_042820](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_042820.png)

  ​

  2. **database menggunakan localhost** di postgress

     **langkah pertama** membuat server bernama localpendatab, kemudian untuk connectionnya di isi di isi seperti dibawah ini dengan menyertakan password dari postgres

     ![Screenshot_20230302_043906](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_043906.png)

     **langkah selanjutnya** membuat table data iris

     a. membuat database terlebih dahulu bernama databaseiris

     ![Screenshot_20230302_044544](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_044544.png)

     b. membuat table iris dengan cara yang sama dengen pembuatan table iris server cloud

     c. pembuatan server local postgres yang berisi table iris telah berhasil dibuat



3. Power BI

   > **data iris yang terdapat pada database localhost** 

   **langkah pertama** export table iris menjadi file csv

   ![Screenshot_20230302_045551](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_045551.png)

   **langkah kedua** memasukan csv tadi dengan cara klik get data kemudian klik text/csv

   ![Screenshot_20230302_050013](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_050013.png)

   **langkah ketiga,** jika sudah berhasil memasukan data csv maka klik load

   ![Screenshot_20230302_050901](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_050901.png)

   **langkah ke empat,** jika sudah di load maka pada bagian kanan layar terdapat data iris yang harus di centang kemudian pilih menu bagan Clustered column chart untuk menampilkan data yang sudah di load tadi > selesai

   ![Screenshot_20230302_051340](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_051340.png)

   ​

   >  **data iris yang terdapat pada database cloud postgres** 

   **langkah pertama,** klik menu getdata > klik more > cari postgress database > klik postgress database > klik connect

   ![Screenshot_20230302_051956](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_051956.png)

   **langkah kedua,** memasukan nama server sesuai dengan yang terdapat di elephantsql.com yaitu mel.db.elephantsql.com dan nama databasenya disesuaikan dengan posgress > klik ok

   ![Screenshot_20230302_052400](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_052400.png)

   kemudian mengisi user name dan password yang terdapat pada akun elephantsql.com > klik connect

   ![Screenshot_20230302_052726](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_052726.png)

​	kemudian langkah-langkah selanjutnya sama dengan cara sebelumnya > setelah berhasil

​	connect > load > selesai

	> **data iris yang terdapat pada database MYSQL**

​	**langkah pertama,** klik menu getdata > klik more > cari MYSQL database > klik MYSQL database > 	

​	klik connect			![Screenshot_20230302_055217](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_055217.png)

​	kemudian mengisi nama server dengan localhost diikuti dengan port mysql pada XAMPP dan database 

​	sesuai dengan nama database yang terdapat di phpmyadmin	![Screenshot_20230302_055513](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_055513.png)

​	jika sudah tertampil seperti di bawah ini maka klik load

![Screenshot_20230302_055732](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_055732.png)

​	jika sudah tertampil di power BI maka pilihlah tampilan visual nya sebagai table maka terlihat seperti 

​	di bawah ini > selesai

![Screenshot_20230302_060056](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_060056.png)

3. data iris csv ke PHPMYadmin

   **langkah pertama,** menyalakan apache dan sql di XAMPP

   ![Screenshot_20230302_053625](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_053625.png)

   **langkah kedua** membuka phpmyadmin > membuat database baru bernama pendatairis

   **langkah ke tiga** mengimport csv ke PHPmyadmin

   ![Screenshot_20230302_054040](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_054040.png)

   jika data tertampil seperti dibawah ini maka telah berhasil.

   ![Screenshot_20230302_054154](C:\Users\lenovo\Pictures\Screenshots\Screenshot_20230302_054154.png)

   ​
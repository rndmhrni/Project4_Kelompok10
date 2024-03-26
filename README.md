# Project 4
## TASK 1
### Class MarketingDataETL
Pembuatan Class MarketingDataETL yang mana ini adalah kelas utama yang memiliki tiga metode: extract(), transform(), dan store().
### Metode extract()
1. Metode ini digunakan untuk mengekstrak data dari file CSV yang disebut "marketing_data.csv" yang terletak di direktori "/content/".
2. Data diekstrak menggunakan fungsi pd.read_csv() dari pandas dengan separator yang ditentukan sebagai ';'.
3. Setelah data diekstrak, metode mencetak data sebelum transformasi dilakukan dan mengembalikan data tersebut.
### Metode transform()
1. Metode ini melakukan transformasi pada data yang telah diekstrak.
2. Jika kolom 'purchase_date' ada dalam data, metode ini mengubah tipe data kolom tersebut menjadi tipe datetime menggunakan pd.to_datetime().
3. Kemudian, baris dengan nilai null dalam kolom 'purchase_date' dihapus menggunakan dropna().
4. Data yang telah ditransformasi dicetak ke konsol dan disimpan kembali dalam atribut data.
5. Metode ini mengembalikan data yang telah ditransformasi.
### Metode store()
1. Metode ini bertanggung jawab untuk menyimpan data yang telah diolah.
2. Jika objek kelas memiliki atribut data, metode ini menyimpan data tersebut dalam file CSV dengan nama "marketing_data_processed.csv" tanpa menyertakan indeks.
3. Jika tidak ada data yang tersedia, metode ini mencetak pesan bahwa tidak ada data untuk disimpan.
### Pemanggilan Metode
Setelah kelas MarketingDataETL diinisialisasi sebagai objek data, metode extract() dipanggil untuk mengekstrak data, diikuti oleh metode transform() untuk mentransformasi data tersebut, dan terakhir metode store() untuk menyimpan data yang telah diolah ke dalam file CSV.

## TASK 2


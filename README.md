# Praktikum5

Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut:

  - Program meminta memasukan data sebanyak-banyaknya (gunakan perulangan)
  - Tampilkan pertanyaan untuk menambah data (ya/tidak?), apabila jawaban "tidak", maka program akan menampilkan daftar datanya.
  - Nilai akhir diambil dari perhitungan 3 komponen nilai (Tugas: 30%, UTS: 35%, UAS: 35%)
  - Buat flowchart dan penjelasan programnya pada README.md.
  - Commit dan push repository ke github.
  
# Langkah-langkah:
    1. Buat programnya terlebih dahulu dengan source code

data =[]
while True :
    nama       = input    ("Nama        : ")
    nim        = input    ("NIM         : ")
    tugas      = int(input("Nilai Tugas : "))
    uts        = int(input("Nilai UTS   : "))
    uas        = int(input("Nilai UAS   : "))
    nilaiakhir = float(tugas)*30/100+(uts)*35/100+(uas)*35/100
    data.append([nama,nim,tugas,uts,uas,nilaiakhir])
    lagi= input("Tambah data (ya/tidak)? ")
    if lagi.lower() =="tidak":
        break


print("=====================================================================================");
print("|  No  |     Nama     |     NIM     |   Tugas   |   UTS   |   UAS   |  Nilai Akhir  |");
print("=====================================================================================");
i=0
for x in data:
    i+=1
    print("|  {6:2}  |  {0:10}  |  {1:9}  |  {2:7}  |  {3:5}  | {4:6}  |  {5:11.2f}  |"\
          .format (x[0][:9] , x[1][:9],x[2],x[3],x[4],x[5], i))
print("=====================================================================================");
   
   Tampilan source code dan output :
   ![image1.png](sikirinsot/prak41.png)

   
    2. Hasil Run
   ![image2.png](sikirinsot/prak42.png)

   
# Penjelasan Program :
    1. Buatlah list berupa Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS.
    2. Lalu inputlah Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS.
    3. Lalu mencari nilai akhir dengan perhitungan nilai tugas 30%, nilai uts 35%, dan uas 35% dengan perintah float
    4. Gunakan perintah append pada Nama, NIM, Nilai Tugas, Nilai UTS, Nilai UAS untuk menambahkan 1 item ke elemen terakhir.
    5. Jika ingin menambah list data ketik "ya" dan jika tidak ingin menambahkan data ke list ketik "tidak". Dengan perintah while jawab =="ya" dan if jawab =="tidak". Jawab imput ("Tambah data (ya/tidak)").
    6. Gunakanlah perulangan for dengan perintah for i in range (len(Nama)):. Fungsi "len" ialah untuk mengembalikan panjang (jumlah anggota) dari suatu objek.
    7. Lalu cetak dengan perintah print
    8. Selesai
    
# Flowchart Praktikum 4
  ![image3.png](sikirinsot/flowchartprak4.jpg)

  
# Sekian TerimaKasih
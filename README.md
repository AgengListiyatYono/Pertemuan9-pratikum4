# Pertemuan9-pratikum4

Repositiry ini dibuat untuk memenuhi tugas Pertemuan 9 - Bahasa Pemrograman (Module Praktikum 4)<br><br>
Nama : Ageng Listiyat Yono <br>
NIM : 312210082<br>
Dosen : Agung Nugroho, M.Kom<br>
Matkul : Bahasa Pemrograman<br>
Kelas : TI.22.B1<br>

Pada halaman ini (Tugas Pertemuan-9-Module Praktikum 4) Dosen memberi tugas sebagai berikut : <br>
Ada dua bahan praktik dimodule 4 kali ini yaitu :<br>

* Soal Latihan yang ada pada module praktikum 4
![SoalLatihan](https://user-images.githubusercontent.com/115475428/202908429-ac98b165-dbf5-4325-80d7-0a9b86c8fa7d.png)

<br>

* Berikut ini saya menulis syntax sekaligus menuliskan langkah-langkahnya sebagai berikut 

```python
# membuat list
print("Buat sebuah list sebanyak 5 elemen dengan nilai bebas")
list = [1, 2, 3, 4, 5]
print(list)
# mengakses list
print("Menampilkan elemen 3")
print(list[2])
print("ambil nilai elemen 2 sampai ke 4")
print(list[1:4])
print("ambil elemen terakhir")
print(list[-1])
# mengubah elemen list
print("ubah elemen 4 dengan nilai lainnya")
list[4]=10
print(list[3])
print("ubah elemen 4 sampai dengan elemen terakhir")
list[4:5]=[20,11]
print(list)
# Tambah elemen list
print("Ambil 2 bagian dari list pertama(A) dan jadikan list ke 2(B)")
list_pertama=list[3:5]
print(list_pertama)
print("tambah list B dengan nilai string")
list_pertama.append("guest")
print(list_pertama)
print("Tambah list B dengan 3 nilai")
list_pertama.append(["guest",7,8])
print(list_pertama)
print("Menggabungkan list B dengan list A")
gabung=list_pertama+list
print(gabung)
```
* Berikut hasil run syntax untuk memenuhi latihan module 4 diatas :<br>
![2022-11-20](https://user-images.githubusercontent.com/115475428/202908802-9cf45963-9caf-4d5f-bf31-9da3b2b22e53.png)<br>


* Soal Tugas praktikum module 4
![Tugas Pratikum](https://user-images.githubusercontent.com/115475428/202908869-4e336eb9-a9c3-46f4-87b7-1c910818d07b.png)

    <br>

* Pada soal tugas ini saya akan menulis dan menjelaskan syntax yang saya buat sebagai berikut<br>

```python
print("===================================================================")
print("Nama         :   Ageng Listiyat Yono")
print("NIM          :   312210082")
print("Kelas        :   TI.22.B1")
print("Mata Kuliah  :   Bahasa Pemrograman")
print("===================================================================")
print("Tugas Praktikum module 4")
# Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut: • Progam meminta
# memasukkan data sebanyak-banyaknya (gunakan perulangan) • Tampilkan pertanyaan untuk menambah data (y/t?),
# apabila jawaban t (Tidak), maka program akan menampilkan daftar datanya. • Nilai Akhir diambil dari perhitungan 3
# komponen nilai (tugas: 30%, uts: 35%, uas: 35%) • Buat flowchart dan penjelasan programnya pada README.md. • Commit
# dan push repository ke github.
from prettytable import PrettyTable
baris = []
stop = False
# masukan nilai
while (not stop):
    nama = input("Masukan Nama : ")
    nim = input("Masukan NIM : ")
    tugas = input("Masukan Nilai Tugas : ")
    uts = input("Masukan Nilai UTS : ")
    uas = input("Masukan Nilai UAS : ")
    nilai_akhir = 0.3 * float(tugas) + 0.35 * float(uts) + 0.35 * float(uas)
    baris.append([nama, nim, tugas, uts, uas, nilai_akhir])
    tanya = input("Tambah data? (y/n) : ")
    if (tanya == "n"):
        stop = True
# cetak nilai
print("===================================================================")
x = PrettyTable()
no = 0
for isi in baris:
    no += 1
    x.field_names = ["No", "Nama", "Nim", "Tugas", "UTS", "UAS", "Nilai Akhir"]
    x.add_row([no, isi[0], isi[1], isi[2], isi[3], isi[4], isi[5]])
print(x)
```
* Berikut hasil run syntax yang saya buat untuk memenuhi praktikum module 4 :<br>
![2022-11-20 (1)](https://user-images.githubusercontent.com/115475428/202911839-2c30d74d-3307-4a8b-a641-d56b505dde5f.png)<br>

* Flowchart program diatas adalah sebagai berikut <br>
![Flowchart](https://user-images.githubusercontent.com/115475428/202909447-7c8732ff-7dc6-4706-a1d6-07e2b79c0113.png)

<br>
> Penjelasan singkat tentang fungsi While untuk mengatur kondisi seperti while not stop dan jika tidak berhenti maka system akan terus menampilkan perintah user untuk meninputkan data . Untuk perhitungan nilai akhir sesuai ketentuan yang dosen inginkan. Sedangkan untuk menampilkan hasil dari inputan user tersebut menggunakan fungsi/module yang ada pada PrettyTable bisa mengakses link berikut ini untuk panduan installation : <br>
> [How to install PIP](https://phoenixnap.com/kb/install-pip-windows)<br>
>[How to install PrettyTable](https://pypi.org/project/prettytable/)<br>
>[How to install Numpy](https://stackoverflow.com/questions/60496280/python-error-modulenotfounderror-no-module-named-modulename/60496306#60496306?newreg=38536a77f74f40a691560e099363f4c3)<br>

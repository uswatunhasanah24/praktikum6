### PRAKTIKUM 6
### USWATUN HASANAH
### 312210343
### TI.22.A3
### LATIHAN DICTIONARY
### SOURCE CODE

![LATIHAN1](https://user-images.githubusercontent.com/115516474/204223756-12eba764-4b81-4aa5-98f6-c8c65bb0fcc8.png)

![LATIHAN2](https://user-images.githubusercontent.com/115516474/204223950-4ef27932-44f1-4d52-a364-6797961de6f0.png)

### PENJELASAN

1. Membuat kontak menggunakan 

`
r={'rose' : '081267888','jeni':'087677776'}.
`

2. Menampilkan kontak menggunakan `r['rose].` r adalah variable dictionary, sedangkan `['rose].` adalah keys dari sebuah dictionary. python:
`
print("menampilkan kontak rose:",r['rose]).
`

3. Menambahkan kontak baru dengan Variabel_dictonary.`['keys']=varibel;` pyhoton:`r['lisa']='087654544';`

4. Mengubah kontak yang lama menjadi baru menggunakan `Variabel_dictonary['keys]=volume;` contohnya mengnakan kontak dina yang awalnya
`'jeni':'08677776'`  menjadi
'r=['jeni']='0899976'`

5. menampilakan seluruh Nama pada kontak mengunakan `keys(). pyhoton: print(r.keys())`

6. Menampilkan seluruh nomer kontak mengunakan `volume(). pyhoton:print(r.items())`

7. Menampilkan seluruh nama beserta nomer kontak menggunakan `item(). pyhoton:print(r.item)`

8. Untuk menghapus salah satu kontak menggunakan statement `del`` variabel_doctinary[keys];. pyhoton:del r['jeni']`

### OUTPUT

![LATIHAN3](https://user-images.githubusercontent.com/115516474/204227231-8eb4d080-26f1-45fe-8844-a3446847a0cf.png)

![LATIHAN4](https://user-images.githubusercontent.com/115516474/204227282-dd29b52d-271d-443d-b643-a0d3a29e293e.png)

### PRAKTIKUM DICTIONARY

### PENJELASAN TUGAS

1. Membuat Dictionary lalu diinput dengan data ``` data={}``

2. Membuat peluang dengan while dan terdapat pilihan menu untuk menjalankan program.
`
while True:
    print()
    a=input("[(L)ihat, (T)amabah, (U)bah, (H)apus, (C)ari, (K)eluar]:")
    print()
    `
3. Menambahkan data NIM, NAMA, NILAI TUGAS, UTS, dan UAS. Data yang diinputkan akan masuk ke Dictionary, data dengan NIM kan sebagai Keys. 
   sedangkan nama, tugas, dan uts, uas akan menjadi data valuse.
    
    `if a=="t" or a=="T":
        print("TAMBAH DATA")
        print("-----------")
        nim=int(input("NIM\t:"))
        nama=input("Nama\t:")
        tugas=input("Tugas\t:")
        uts=input("UTS\t")
        uas=input("UAS\t")
        akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)
        data[nim]=nama,tugas,uts,uas,akhir
        print()
        `
4. Menambahkan atau melihat data. sebelum melihatdata kita haus mengimpu data terebih dahulu agar data yang udah di input bisa ditampilkan.
   jika belum mengiput data otomatis data yang ditambilkan akan bertulikan "Tidak ada data"
   
   `elif a=="l" or a=="L":
        if data.items():
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print("|{0:^10}|{1:^10}|{2:^6}|{3:>^6}|{4:^6}|{5:^12}|".format ("NIM", "NAMA", "TUGAS", "UTS", "UAS", "TUGAS"))
            print(72*"=")
            for item in data.items():
                print("|{0:>10}|{1:>10}|{2:>6}|{3:>6}|{4:>6}|{5:>12}|".format(nim, nama, tugas, uts, uas, akhir))
                print(72*"=")
                print()

        else:
            print("DAFTAR NILAI")
            print("------------")
            print(72*"=")
            print()
            print("|{0:^10}|{1:^10}|{2:6^}|{3:^6}|{4:^6}|{4:^6}|{5:^12}|".format("NIM","NAMA","TUGAS","UTAS","UAS","NILAI AKHIR"))
            print(72*"=")
            print("| TIDAK ADA DATA|")
            print(72*"=")
            print()
            `
            
5. Apa bila ingin mengubah data, kita di minta untuk mengiput NIM terlebih dulu. baru lah data bisa diubah.
  ` 
   elif a=="u"or a=="U":
        print("UBAH DATA")
        b=input("Masukan NIM Anda:")
        print()
        if data. keys():
            tugas=int(input("Tugas\t"))
            uts=int(input("UTS\t"))
            uas=int(input("UAS\t"))
            akhir=(int(tugas)*30/100)+(int(uts)*35/100)+(int(uas)*35/100)
            `
            
6. Apa bila ingin menghapus data. maka kita kan diminta untuk mengimput NIM terlebih dulu. lalu data yang telah diinput akan dihapus bersama
volues_nya(Nama, Tugas, uts, uas).
 `
 elif a=="h" or a=="H":
        print("HAPUS DATA")
        print("----------")
        b=input("Masukan NIM Anda:")
        print()
        if data.keys():
            del data[nim]
            `
            
7. Apa bila ingin menceri data. anda kan diminta untuk mengimput NIM. kemudian data yang di carikan keluar bersamaan NIM yang diinput tadi.
   `
   elif a=="c" or a=="C":
        print("CARI DATA")
        print("---------")
        b=input("Masukan NIM Anda:")
        print()
        if data.keys():
            print(72*"=")
            print("|{0:^10}|{1:^10}|{2:^6}|{3:^6}|{4:^6}|{5:^12}|".format("NIM","NAMA","TUGAS","UTS","UAS","NILAI AKHIR"))
            print(72*"=")
            print("|{0:>10}|{1:>10}|{2:>6}|{3:>6}|{4:>6}|{5:>12}|".format(nim,nama,tugas,uts,uas,akhir))
            print(72*"=")
            print()
            `
            
8. JIka sudah selesai data yang diinput anda bisa memilih menu "K" maka program akan terhenti otomais.
`
elif a=="k" or a=="K":
`
              break

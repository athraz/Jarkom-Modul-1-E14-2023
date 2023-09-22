# Jarkom-Modul-1-E14-2023

| Nama                      | NRP           |Username      |
|---------------------------|---------------|--------------|
|Muhammad Razan Athallah    |5025211008     |athraz        |
|Moh rosy haqqy aminy       |5025211012     |hqlco         |

## 1
### Soal
User melakukan berbagai aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file.

- Berapakah sequence number (raw) pada packet yang menunjukkan aktivitas tersebut? 
- Berapakah acknowledge number (raw) pada packet yang menunjukkan aktivitas tersebut? 
- Berapakah sequence number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
- Berapakah acknowledge number (raw) pada packet yang menunjukkan response dari aktivitas tersebut?
### Jawaban
Disebutkan bahwa **aktivitas dengan menggunakan protokol FTP. Salah satunya adalah mengunggah suatu file**
maka dapat menggunakan ```ftp.request.command == “STOR”``` untuk melakukan filter pada perintah tersebut.

Dapat dilihat pada paket nomer 147 dapat dilihat sequence number (raw) dan sequence number (raw)
![Alt text](<Screenshot 2023-09-21 172204.png>)

Respon ada pada paket 149 dapat dilihat sequence number (raw) dan sequence number (raw)
![Alt text](<Screenshot 2023-09-21 172415.png>)

**FLAG**
![Alt text](<Screenshot 2023-09-21 172459.png>)

## 2
### Soal
Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!
### Jawaban
Cari salah satu paket dengan protocol ```http``` setelah itu follow stream, didapat web server 
![Alt text](<Screenshot 2023-09-21 172606.png>)

**FLAG**
![Alt text](<Screenshot 2023-09-21 175059.png>)

## 3
### Soal
Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
- Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
- Protokol layer transport apa yang digunakan?

### Jawaban

## 4
### Soal
Berapa nilai checksum yang didapat dari header pada paket nomor 130?

### Jawaban

## 5
### Soal
Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
- Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
- Port berapakah pada server yang digunakan untuk service SMTP?
- Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

### Jawaban

## 6
### Soal
Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.

### Jawaban
Terdapat beberapa clue yang diberikan dari deskripsi tersebut, yaitu:
- Huruf kapital yang membentuk kata 'SUBSTITUSI'
- Source address 7812
- a1 e5 u21

Dari clue tersebut, didapatkan perintah untuk melakukan substitusi pada source adress packet 7812 menggunakan metode cipher a1z26. Source address pada packet 7812 adalah 104.18.14.101, jika dipisah sesuai rentang 1-26 didapatkan 10 4 18 14 10 1. Angka-angka tersebut jika disubstitusi menjadi huruf maka didapat JDRNJA.

**FLAG**
![Screenshot 2023-09-21 184849](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/38100d32-de2e-478d-920f-f82c965697ca)

## 7
### Soal
Berapa jumlah packet yang menuju IP 184.87.193.88?

### Jawaban
Filtering dengan query `ip.dst == 184.87.193.88` diperoleh hasil 6 packet sebagai berikut:
![Screenshot 2023-09-18 190644](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/00d81d6c-4139-4b95-be4d-6209e71581b7)


**FLAG**
![Screenshot 2023-09-18 190800](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/ac4f912a-d640-4432-a997-cd1c5f2afdf8)


## 8
### Soal
Berikan kueri filter sehingga wireshark hanya mengambil semua protokol paket yang menuju port 80! (Jika terdapat lebih dari 1 port, maka urutkan sesuai dengan abjad)

### Jawaban
Query adalah sebagai berikut: `tcp.dstport == 80 || udp.dstport == 80`.

**FLAG**
![Screenshot 2023-09-18 191533](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/73d6f8da-457b-4448-baf5-be54729eb2a2)

## 9
### Soal
Berikan kueri filter sehingga wireshark hanya mengambil paket yang berasal dari alamat 10.51.40.1 tetapi tidak menuju ke alamat 10.39.55.34!

### Jawaban
Query adalah sebagai berikut: `ip.src == 10.51.40.1 && ip.dst != 10.39.55.34`.

**FLAG**
![Screenshot 2023-09-18 200607](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/2199aa3b-c052-40e2-b794-bc8e56eb9460)

## 10
### Soal
Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet!

### Jawaban
Filtering dengan query `telnet contains "Login"` lalu follow TCP stream, didapatkan hasil username dan password sebagai berikut:
![Screenshot 2023-09-18 194550](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/056e6b36-b89a-4574-b623-f126b8231437)
![Screenshot 2023-09-18 194612](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/66d5cabb-34f8-484c-b71f-ec3fb7414eb0)

**FLAG**
![Screenshot 2023-09-18 194657](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/4ed8dcc8-c8d0-46de-b43e-0c219da0eb94)


![Screenshot 2023-09-18 213304](https://github.com/athraz/Jarkom-Modul-1-E14-2023/assets/96050618/df994f2b-f814-4243-bfa6-0a242a345774)



# Jarkom-Modul-1-E14-2023
| Nama                      | NRP           |Username      |
|---------------------------|---------------|--------------|
|TBA  |5025211009     |-     |
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
- erapa banyak packet yang berhasil di capture dari file pcap tersebut?
- Port berapakah pada server yang digunakan untuk service SMTP?
- Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?

### Jawaban
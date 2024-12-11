# **Hugging Face**

## **A. Deployment dan permasalahannya**

Untuk kebutuhan progress report, demo, dan pengambilan keputusan, aplikasi yang telah dibuat perlu diperlihatkan atau bisa digunakan terlebih dahulu oleh pihak lain (seperti user, supervisor, atau divisi lain). Aplikasi ini bisa berisi model machine learning, visualisasi, tabel, dashboard atau interface yang interaktif. 

Permasalahan muncul dimana sebenarnya kebanyakan dari pihak lain tersebut bukan berasal dari backgorund IT, sehingga akan tidak cocok jika mereka diserahkan aplikasi dalam bentuk file python atau ipynb. Berikut merupakan detil dari permasalahan tersebut:

* Mereka akan sulit dalam menentukan tombol apa yang perlu di-klik untuk menjalankan aplikasi, instalasi library atau dependency, atau yang lainnya. 
* Mereka juga akan terpaparkan script dari aplikasi yang sebenarnya mereka tidak butuh. Mereka hanya ingin melihat bentuk hasil akhir aplikasi, bukan bagaimana aplikasi tersebut dibuat.
* Script dari aplikasi yang terpaparkan bisa saja memiliki data sensitif yang dapat disalahgunakan.

Semua kondisi ini ditakutkan membuat proses progress report menjadi tidak efisien dan membutuhkan waktu yang lama.

## **B. Docker, keunggulan, dan permasalahannya**

Docker bisa digunakan untuk menyelesaikan masalah di atas. Docker dapat mengemas aplikasi beserta dependensinya sehingga aplikasi tersebut dapat dijalankan oleh siapa saja dengan device apa saja. Namun, Docker mengharuskan pihak lain untuk menggunakan device atau server dengan spesifikasi teretentu dan menginstal Docker untuk menjalankan aplikasi secara lokal. Kondisi ini dapat mengurangi efisiensi proses progress report.

## **C. Hugging Face dan Kelebihannya**

Untuk mengatasi tantangan tersebut, Hugging Face dapat digunakan. Hugging Face adalah platform untuk app deployment yang mudah. Berikut merupakan karakteristik dari Hugging Face:

* Memiliki fitur Spaces untuk meng-host aplikasi dan aplikasi ini bisa dibagi melalui URL yang dapat diakses oleh siapa pun. Sehingga, progress report akan menjadi lebih efisien karena pihak lain tidak menjalankan aplikasi yang sudah di-deploy secara langsung di device atau server lokal.
* Fitur Spaces memiliki spesifikasi (untuk versi gratis) 2 CPU cores, 16 GB RAM, dan 50 GB memori.
* Aplikasi di-host berdasarkan web interface, sehingga membutuhkan Library seperti Streamlit atau Gradio dalam Aplikasi.
* User dapat menentukan apakah script dari aplikasi bersifat publik atau tidak.
* Aplikasi yang sudah di-deploy dapat dengan mudah diubah.
* Dapat digunakan untuk kolaborasi layaknya GitHub.

## **D. Kekurangan Hugging Face**

Terlepas dari kelebihan tersebut, Hugging Face masih memiliki kekurangan tersendiri dibandingkan Docker. Hugging Face kurang cocok untuk membaca file requirements untuk infrastruktur yang kompleks. Lalu, Hugging Face juga tidak bisa menerapkan sistem multi-komponen dan deployment tingkat produksi. Kondisi tersebut tidak terjadi dalam Docker karena Docker memberikan kontrol penuh atas infrastruktur dan konfigurasi untuk deployment.

## **E. Kesimpulan**

Maka dari itu, sebagai app deployment, Hugging Face cocok untuk berbagi aplikasi sederhana yang mudah digunakan dengan cepat. Di sisi lain, Docker lebih cocok digunakan untuk berbagi aplikasi kompleks dan berskala besar (production).

## Eksplor repo ini untuk melihat cara menggunakan Hungging Face untuk App Deployment

[Sumber](https://www.geeksforgeeks.org/hugging-face-transformers/)

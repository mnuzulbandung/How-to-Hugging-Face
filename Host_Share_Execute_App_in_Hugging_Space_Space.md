### How to: Meng-host, membagi dan menjalankan aplikasi dengan Hugging Face Space

1.	Buat folder dengan nama apa pun (Contoh, deployment) di lokasi mana saja.

2.	Masukan aplikasi yang ingin di-host (Contoh, app.py) ke dalam folder poin 1. Berikut contoh dari aplikasi yang ingin di-host.

```
import pandas as pd

def data():
    data = {'Name': ['Adi', 'Budi', 'Cindi', 'Dedi'],
    'Age': [15, 16, 17, 18]}
    df = pd.DataFrame(data)
    print(df)

if __name__== '__main__':
    data()
```

3.	Masukkan file requirement.txt ke dalam folder Poin 1. File ini berisi library beserta versinya yang diperlukan untuk menjalankan aplikasi yang ingin di-host. Lihat link [ini](https://github.com/mnuzulbandung/How-to-Create-requirements.txt) untuk cara membuatnya.

4.	Buka laman [Hugging Face](https://huggingface.co/), buka akun atau lakukan login.

5.	Buka laman [New Space]( https://huggingface.co/new-space); isi nama dan deskripsi lain dari Space yang ingin dibuat (Contoh Nama, sample). Proses ini akan membuat link repo kosong ([Contoh](https://huggingface.co/spaces/mnuzulbandung/sample)).


6.	Untuk memasukkan aplikasi ke dalam Space ini, buka bagian Files; pilih Add File; pilih Upload Files; Upload file yang ada di dalam folder poin 1; pilih Commit Changes to main.

7.	Untuk menjalankan aplikasi di dalam Space ini, buka bagian App. Hugging Face akan secara otomatis menginstalasi dependency yang dibutuhkan.

8.	Untuk membagi aplikasi ke pihak lain, copy dan bagi link URL Space ini.

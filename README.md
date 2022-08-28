# Template Proyek Django PBP

Pemrograman Berbasis Platform (CSGE602022) - diselenggarakan oleh Fakultas Ilmu Komputer Universitas Indonesia, Semester Ganjil 2022/2023

## Pendahuluan

Repositori ini merupakan sebuah template yang dirancang untuk membantu mahasiswa yang sedang mengambil mata kuliah Pemrograman Berbasis Platform (CSGE602022) mengetahui struktur sebuah proyek aplikasi Django serta file dan konfigurasi yang penting dalam berjalannya aplikasi. Kamu dapat dengan bebas menyalin isi dari repositori ini atau memanfaatkan repositori ini sebagai pembelajaran sekaligus awalan dalam membuat sebuah proyek Django.

## Cara Menggunakan

Apabila kamu ingin menggunakan repositori ini sebagai repositori awalan yang nantinya akan kamu modifikasi,

1. Clone repositori ini ke lokal milikmu.
2. Masuk ke dalam repositori yang sudah di-clone dan jalankan perintah berikut untuk menyalakan virtual environment.
```
python -m venv env
```
3. Nyalakan environment dengan perintah berikut.
```bash
Linux/Unix: source env/bin/activate
Windows: env\bin\activate
```
4. Install dependencies yang dibutuhkan untuk menjalankan aplikasi dengan perintah berikut.
```
pip install -r requirements.txt
```
5. Jalankan aplikasi Django dengan perintah `manage.py runserver`
6. Bukalah `http://localhost:8000` pada browser favoritmu untuk melihat apakah aplikasi sudah berjalan dengan benar.
## Contoh Deployment 

Pada template ini, deployment dilakukan dengan memanfaatkan GitHub Actions sebagai _runner_ dan Heroku sebagai platform Hosting aplikasi. 

Untuk melakukan deployment, kamu dapat melihat instruksi yang ada pada [Tutorial-0](https://github.com/pbp-fasilkom-ui/ganjil-2023/blob/master/assignments/tutorial/tutorial-0.md).

Untuk contoh aplikasi Django yang sudah di deploy, dapat kamu akses di [https://django-pbp-template.herokuapp.com/](https://django-pbp-template.herokuapp.com/)

## Credits
Template ini dibuat berdasarkan [PBP Ganjil 2021](https://gitlab.com/PBP-2021/pbp-lab) yang ditulis oleh Tim Pengajar Pemrograman Berbasis Platform 2021 ([@prakashdivyy](https://gitlab.com/prakashdivyy)) dan [django-template-heroku](https://github.com/laymonage/django-template-heroku) yang ditulis oleh [@laymonage, et al.](https://github.com/laymonage). Template ini dirancang sedemikian rupa sehingga mahasiswa dapat menjadikan template ini sebagai awalan serta acuan dalam mengerjakan tugas maupun dalam berkarya.
# Hello Minikube
## Sumber : https://kubernetes.io/docs/tutorials/hello-minikube/

Tutorial ini menunjukkan kepada Anda cara menjalankan aplikasi Hello World Node.js sederhana di Kubernet menggunakan Minikube dan Katacoda. Katacoda menyediakan lingkungan Kubernetes dalam peramban gratis.


## Membuat Minikube Cluster
1. Klik Launch Terminal.
   
   ![00](gambar/a.PNG)
   
   Setelah diklik maka muncul tampilan sebagi berikut :
   ![00](gambar/1.PNG)
   
2. Buka dasbor Kubernetes di browser:
   ![00](gambar/2.PNG)
   
3. Klik tab Preview port 30000 dibagian atas.
   ![00](gambar/3.PNG)
   
4. Pada browser akan muncul tab baru, seperti pada gambar di bawah ini. Ketik 30000, lalu klik Display Port.
   ![00](gambar/4.PNG)
   

## Membuat Deployment

Kubernetes Pod adalah grup yang terdiri dari satu atau lebih Kontainer, diikat bersama untuk keperluan administrasi dan jaringan. Pod dalam tutorial ini hanya memiliki satu Kontainer. Penyebaran Kubernetes memeriksa kesehatan Pod Anda dan memulai kembali Kontainer Pod jika sudah berakhir. Penempatan adalah cara yang disarankan untuk mengelola pembuatan dan penskalaan Pod.

1. Gunakan perintah kubectl create untuk membuat Deployment yang mengelola Pod. Pod menjalankan Container berdasarkan pada gambar Docker yang disediakan.
   ![00](gambar/5.PNG)
   
2. Lihat Deployment, hasilnya akan mirip seperti ini :
   
   ![00](gambar/6.PNG)
   
3. Lihat Pod, hasilnya akan mirip seperti ini :
   ![00](gambar/7.PNG)
   
4. Lihat Cluster Events
   ![00](gambar/8.PNG)
   
5. Lihat kubectl
   
   ![00](gambar/9.PNG)
   
   
## Membuat Service

1. Paparkan Pod ke internet publik menggunakan perintah kubectl expose:
   ![00](gambar/10.PNG)
   
2. Lihat Layanan yang baru saja Anda buat:
   ![00](gambar/11.PNG)
   
3. Jalankan perintah berikut:
   ![00](gambar/12.PNG)
   
4. Hanya lingkungan Katacoda: Klik tanda plus, lalu klik Pilih port untuk dilihat di Host 1.

5. Hanya lingkungan Katacoda: Perhatikan nomor port 5 digit yang ditampilkan berlawanan dengan 8080 dalam output layanan. Nomor port ini dibuat secara acak dan bisa berbeda untuk Anda. Ketikkan nomor Anda di kotak teks nomor port, lalu klik Display Port. Menggunakan contoh dari sebelumnya, Anda akan mengetikkan 30369.
   ![00](gambar/13.PNG)
   
   Ini membuka jendela browser yang melayani aplikasi Anda dan menampilkan pesan "Hello World".
   ![00](gambar/14.PNG)



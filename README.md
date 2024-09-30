Praktikum 1: Membuat Project Flutter Baru

![Screenshot 2024-09-30 100932](https://github.com/user-attachments/assets/a7aad9d9-b39e-4269-9c22-1cb6cae8adc4)
Buat New Project, pilih gererators flutter, dan patch flutter sdk.

![Screenshot 2024-09-30 101124](https://github.com/user-attachments/assets/8986e34e-a470-4c6e-9637-140c5f6b6fe4)
ganti android language ke java.

Praktikum 2: Membuat Repository GitHub dan Laporan Praktikum

![Screenshot 2024-09-30 101444](https://github.com/user-attachments/assets/ddc9310d-636a-437a-968c-a9f7d2680927)
Buat new repository public

pada terminal adroidstudio ketikan perintah :
1. git init (Ini akan menginisialisasi repositori Git di folder proyek Android Studio Anda.)
2. git ad . (Menambahkan semua file proyek ke repositori Git.)
3. git commit -m "Pesan commit pertama" (commit untuk perubahan)
4. git remote add origin https://github.com/alfharisqi/widgetdasarflutterapp.git (menghubungkan repositori lokal dengan repositori GitHub.)
5. git push -u origin master (Kirim commit ke repositori GitHub.)

repository sudah siap
![Screenshot 2024-09-30 102002](https://github.com/user-attachments/assets/8c8c61be-54e8-4971-9dc3-49a07efb4330)

Praktikum 3: Menerapkan Widget Dasar

Buat folder baru basic_widgets di dalam folder lib. Kemudian buat file baru di dalam basic_widgets dengan nama text_widget.dart. Ketik atau salin kode program berikut ke project hello_world Anda pada file text_widget.dart.

import 'package:flutter/material.dart';

class MyTextWidget extends StatelessWidget {
  const MyTextWidget({Key? key}) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return const Text(
      "Nama saya Fulan, sedang belajar Pemrograman Mobile",
      style: TextStyle(color: Colors.red, fontSize: 14),
      textAlign: TextAlign.center);
  }
}

Lakukan import file text_widget.dart ke main.dart, lalu ganti bagian text widget dengan kode di atas. Maka hasilnya seperti gambar berikut. Screenshot hasil milik Anda.
![Screenshot 2024-09-30 103752](https://github.com/user-attachments/assets/e27fb641-43cd-4fb8-8a73-0101264709c2)

Langkah 2: Image Widget
Buat sebuah file image_widget.dart di dalam folder basic_widgets dengan isi kode berikut.
import 'package:flutter/material.dart';
class MyImageWidget extends StatelessWidget {
  const MyImageWidget({Key? key}) : super(key: key);
  @override
  Widget build(BuildContext context) {
    return const Image(
      image: AssetImage("logo.jpg")
    );
  }
}

Lakukan penyesuaian asset pada file pubspec.yaml dan tambahkan file logo Anda di folder assets project hello_world.
flutter:
  assets:
     - logo.jpg

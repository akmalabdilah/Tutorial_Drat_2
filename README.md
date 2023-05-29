# Pemograman_Mobile2-Latihan_Dart
## Latihan Menggunakan Bahasa Dart


<p align="center">
 <img src="https://user-images.githubusercontent.com/91085882/137566814-9c8c078c-1c3e-475c-b23d-7f4922f74beb.gif"/>
</p>
<p align="center">
<a href="https://github.com/akmalabdilah"><img title="Author" src="https://img.shields.io/discord/102860784329052160?color=BLUE&label=M.%20AKMAL%20AL%20ABDILAH1&logo=GITHUB&logoColor=BLACK&style=plastic"></a>
<p align="center">

<p align="center">
<a href="https://github.com/akmalabdilah/Pemograman_Mobile2-Latihan_Dart">Requirements</a> •
<a href="https://github.com/akmalabdilah/Pemograman_Mobile2-Latihan_Dart">Informasi</a> •
<a href="https://github.com/akmalabdilah/Pemograman_Mobile2-Latihan_Dart">Tutorial</a>
</p>
</div>

# Requirements
- [Dart](https://git-scm.com/download)

# Informasi Dart
Apa itu Dart?
<p>
Dart adalah bahasa pemrograman yang dikembangkan oleh Google. Dart didesain untuk membangun aplikasi lintas platform, termasuk aplikasi mobile untuk Android dan iOS, aplikasi web, dan juga aplikasi desktop. Dart memiliki sintaks yang mirip dengan bahasa pemrograman C dan JavaScript, sehingga relatif mudah dipelajari bagi para pengembang yang sudah memiliki pengalaman dengan bahasa-bahasa tersebut. Salah satu keunggulan Dart adalah fitur Just-in-Time (JIT) dan Ahead-of-Time (AOT) compilation yang memungkinkan aplikasi yang ditulis dengan Dart berjalan dengan performa tinggi. Dart juga dilengkapi dengan kerangka kerja Flutter yang populer untuk pengembangan aplikasi mobile dan UI yang kaya.
</p>

# Tutorial
- Pada saat pertama kali menggunakan Dart, perlu dilakukan penginstalan extension
di visual Studio Code. Jalankan perintah berikut:

```bash
> Dart
```


![Gambar 1](Screenshots/ss1.JPG)


- Setelah itu jalankan perintah Ctrl+Shift+P dan tulis Dart: New Project. untuk membuat repository 

- Untuk membuat file pilih yang bagian ke dua dan berilah nama sesuka kalian dan jika sudah di pindahkan ke halaman folder hapus isi yang ada di polder dan buat file baru di dalam polder tersebut.

- Dan ini adalah koding dart serta hasil runnya

- 0. buat kan codingan fungsi validasi login dalam bahasa dart, dengan kualifikasi berikut:

untuk user name
1. min 6 karakter.
Untuk password 
1. min 6 karakter.
2. harus ada huruf besar.
3. harus ada character.
4. harus ada angka.
5. harus ada huruf kecil.

![Gambar 2](Screenshots/ss2.JPG)

```dart
import 'dart:io';

void main() {
  // Memanggil fungsi login
  bool isLoggedIn = login();

  if (isLoggedIn) {
    print("Login berhasil");
  } else {
    print("Login gagal");
  }
}

bool login() {
  print("=== Menu Login ===");

  stdout.write("Masukkan username: ");
  String username = stdin.readLineSync()!;

  stdout.write("Masukkan password: ");
  String password = stdin.readLineSync()!;

  // Memeriksa panjang password
  if (password.length < 6) {
    print("Eror: Password harus memiliki setidaknya 6 karakter");
    return false;
  }

  // Memeriksa keberadaan huruf besar
  if (!password.contains(RegExp(r'[A-Z]'))) {
    print("Eror: Password harus mengandung setidaknya satu huruf besar");
    return false;
  }

  // Memeriksa keberadaan huruf kecil
  if (!password.contains(RegExp(r'[a-z]'))) {
    print("Eror: Password harus mengandung setidaknya satu huruf kecil");
    return false;
  }

  // Memeriksa keberadaan angka atau karakter khusus
  if (!password.contains(RegExp(r'[0-9\W]'))) {
    print(
        "Eror: Password harus mengandung setidaknya satu angka atau karakter khusus");
    return false;
  }

  // Jika semua persyaratan terpenuhi, login berhasil
  return true;
}

```

- Gambar run Eror: Password harus memiliki setidaknya 6 karakter

![Gambar 3](Screenshots/ss3.JPG)

- Gambar run Eror: Password harus mengandung setidaknya satu huruf besar

![Gambar 4](Screenshots/ss4.JPG)

- Gambar run Eror: Password harus mengandung setidaknya satu huruf kecil

![Gambar 5](Screenshots/ss5.JPG)

- Eror: Password harus mengandung setidaknya satu angka atau karakter khusus

![Gambar 6](Screenshots/ss6.JPG)




- Selesai


<div>
<h2 align="center">Thanks For Reading!!!</h2>
<div align="center">
<img src="https://user-images.githubusercontent.com/91085882/222731693-24383140-7623-4e7a-a528-6621380b7be8.gif">
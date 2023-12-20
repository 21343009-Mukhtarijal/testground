# PBJ1 - Pemrograman Berbasis Jaringan Menggunakan Node.js

## Deskripsi
Repository ini menyediakan panduan langkah-demi-langkah untuk memulai dengan Node.js untuk pemrograman berbasis jaringan. Panduan ini mencakup instruksi instalasi Visual Studio Code, Node.js, serta langkah-langkah dasar untuk membuat dan menjalankan program sederhana menggunakan Node.js.

## Persyaratan
Sebelum Anda memulai, pastikan Anda telah menginstal:
- [Visual Studio Code](https://code.visualstudio.com/)
- [Node.js](https://nodejs.org/)

## Instalasi

1. Download dan instal [Visual Studio Code](https://code.visualstudio.com/).
2. Jalankan installer Visual Studio Code (VSCodeUserSetup-{versi}.exe).
3. Kunjungi situs resmi [Node.js](https://nodejs.org/) dan unduh versi yang sesuai dengan sistem operasi Anda.
4. Jalankan installer Node.js.
5. Buka terminal atau command prompt, dan verifikasi instalasi Node.js dengan perintah `node -v` dan `npm -v`.
6. Jika perlu, atur PATH Node.js pada environment variables.

## Penggunaan

1. Buka Visual Studio Code dan buka folder proyek Anda.
2. Buat folder baru dengan nama "testground."
3. Dalam folder "testground," buat file bernama "hello.js" dan masukkan kode berikut:

    ```javascript
    console.log('Selamat datang di Node.js!');
    ```

4. Jalankan program melalui terminal dengan perintah:

    ```bash
    node testground/hello.js
    ```

5. Buat file baru bernama "hello-world.js" dengan kode berikut:

    ```javascript
    const http = require('http');
    const server = http.createServer((req, res) => {
        res.end('Hello, World!');
    });
    server.listen(3000, '127.0.0.1', () => {
        console.log('Server berjalan di http://127.0.0.1:3000/');
    });
    ```

6. Jalankan program tersebut dan buka http://127.0.0.1:3000/ di browser Anda.

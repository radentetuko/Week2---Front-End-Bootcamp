# Rangukam WEEK 2 - Front-end Bootcamp

## PropTypes

- ### **Apa itu PropTypes?**

  PropTypes merupakan library untuk menvalidasi props. Ini sangat membantu dalam meminimalkan bugs saat mengembangkan App besar. Jika props tidak benar type nya maka akan muncul warning.

  PropTypes mengirimkan berbagai jenis validator yang dapat digunakan untuk memastikan bahwa data yang diterima valid. Untuk alasan performa, propTypes hanya melakukan pengecekan di mode pengembangan atau development.

- ### Instalasi PropTypes

  ```
    npm install prop-types
  ```

## **React Router**

- ### **Apa itu React Router?**

  Routing adalah proses di mana pengguna diarahkan ke halaman yang berbeda berdasarkan tindakan atau permintaan user. React Router adalah sistem perpustakaan standar yang dibangun di atas React dan digunakan untuk membuat perutean di aplikasi React menggunakan Paket React Router.

- ### **Instalasi React Router**

  React berisi tiga paket berbeda untuk perutean. Ini adalah:

  - react-router: Ini menyediakan komponen dan fungsi perutean inti untuk aplikasi React Router.
  - react-router-native: Ini digunakan untuk aplikasi seluler.
  - react-router-dom: Digunakan untuk desain aplikasi web.

  Untuk menggunakan perutean react, pertama, kita perlu menginstal modul react-router-dom di aplikasi kita. Perintah di bawah ini digunakan untuk menginstal react router dom.

  ```
  $ npm install react-router-dom –save
  ```

- ### **Komponen di React Router**

  Ada dua jenis komponen router:

  `<BrowserRouter>`: Ini digunakan untuk menangani URL dinamis.

  `<HashRouter>`: Ini digunakan untuk menangani permintaan statis.

## **State Management Library (Redux)**

- ### **Apa itu State Management Library?**

  State management library adalah library yang digunakan untuk mengelola state pada suatu aplikasi JavaScript.

  Beberapa diantaranya:

  - Redux
  - MobX
  - Flux
  - Recoil

  Pada bagian ini kita akan membahas salah satu state management library yang popular digunakan pada React yaitu Redux.

  Redux adalah state container untuk aplikasi JavaScript.

- ### **Mengapa Redux?**

  Sebuah state bisa digunakan oleh banyak sekali component, seringkali state harus dipindah ke parent component (lifting up) agar state tersebut dapat digunakan oleh component lain.

  Ketika menggunakan React dengan Redux kita tidak perlu lagi memindahkan state dari satu component ke component lain, karena Redux mengubah state menjadi global state dan menempatkannya pada suatu tempat bernama store.

  Setiap component dapat menggunakan state yang ada di store secara langsung.

  Semua modifikasi state juga dilakukan melalui Redux, store pada Redux menjadi satu-satunya tempat untuk mengelola state(single source of truth).

  Aplikasi menjadi lebih konsisten dan mudah untuk ditest.

- ### **Konsep Dasar**

  Paling tidak ada 4 istilah yang digunakan dalam Redux yang wajib untuk diketahui.

  - Actions

    Sebuah JavaScript Object mewakili apa yang terjadi di dalam aplikasi.

  - Reducers

    Function yang menerima object state dan object action, bertugas menentukan bagaimana suatu state diubah. Output reducer adalah state baru.

    Syntax:` (state, action) => newState`

  - Store

    dimana global state disimpan.

  - Dispatch

    Satu-satunya cara untuk mengubah state di dalam store adalah dengan memanggil method bernama dispatch yang berisi object action, kemudian Redux akan mengeksekusi reducer yang sesuai.

  - Selector

    Function yang digunakan untuk mendapatkan data dari state yang ada di dalam store.

## **Async Action With Redux Thunk and Middleware**

- ### **Apa itu Redux Thunk?**

  Redux Thunk adalah middleware yang memungkinkan Anda memanggil pembuat aksi yang mengembalikan fungsi sebagai ganti objek aksi. Fungsi itu menerima metode pengiriman penyimpanan, yang kemudian digunakan untuk mengirim aksi sinkron di dalam isi fungsi setelah operasi asinkron selesai.

- ### **Instalasi Redux Thunk**
  ```
  npm install redux-thunk@2.3.0
  ```

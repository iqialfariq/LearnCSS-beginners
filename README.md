## Cara menghubungkan CSS ada 3 cara yaitu:

- **Inline CSS**  
  Menyisipkan style di setiap tag HTML.  
  ```html
  <p style="color: red; font-size: 18px;">
    Teks ini menggunakan Inline CSS
  </p>

- **Internal CSS**  
  Membuat file CSS dengan tag `<style>` pada bagian `<head>`.  
  ```html
  <head>
    <style>
      p {
        color: blue;
        font-size: 20px;
      }
    </style>
  </head>
  <body>
    <p>Teks ini menggunakan Internal CSS</p>
  </body>

- **External CSS**  
  Membuat file CSS terpisah dan menghubungkannya dengan `<link>`.  
  ```html
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <p>Teks ini menggunakan External CSS</p>
  </body>

# Property dan Value dasar CSS 

## Property CSS: Color

- **Color**  
  Untuk memberikan warna pada elemen HTML.  
  Value `color` ada 3 yaitu:  

  1. **Nama warna**  
     ```html
     <p style="color: red;">Teks warna merah</p>
     ```

  2. **RGB**  
     ```html
     <p style="color: rgb(0, 128, 0);">Teks warna hijau</p>
     ```

  3. **Hexadecimal**  
     ```html
     <p style="color: #0000FF;">Teks warna biru</p>
     ```

## Background Styling

- **Background-Color**  
  Untuk memberikan warna latar belakang pada elemen HTML.  
  Dengan ini, kamu bisa mengatur warna area di belakang teks, gambar, atau konten lain dalam sebuah elemen.  
  Value `background-color` ada 4 yaitu:  

  1. **Color (nama warna)**  
     ```html
     <div style="background-color: yellow;">
       Latar belakang kuning
     </div>
     ```

  2. **RGB**  
     ```html
     <div style="background-color: rgb(0, 128, 128);">
       Latar belakang hijau kebiruan
     </div>
     ```

  3. **Hexadecimal**  
     ```html
     <div style="background-color: #FF5733;">
       Latar belakang oranye
     </div>
     ```

  4. **Inherit**  
     ```html
     <div style="background-color: inherit;">
       Latar belakang mengikuti elemen induk
     </div>
     ```
     
- **Background-Image**  
  Untuk memberikan gambar latar belakang pada sebuah elemen HTML.  
  Value `background-image` ada 1 yaitu: `url()`.  

  ```html
  <div style="background-image: url('sample.jpg');">
    Konten dengan gambar latar belakang
  </div>

- **Background-Position**  
  Untuk mengatur posisi gambar latar belakang dalam sebuah elemen.  
  Dengan ini, kamu bisa menentukan apakah gambar berada di kiri, kanan, tengah, atas, bawah, atau posisi khusus menggunakan nilai koordinat.  
  Value `background-position` ada 7 yaitu:  

  1. **Top**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: top;">
       Latar belakang di atas
     </div>
     ```

  2. **Bottom**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: bottom;">
       Latar belakang di bawah
     </div>
     ```

  3. **Left**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: left;">
       Latar belakang di kiri
     </div>
     ```

  4. **Right**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: right;">
       Latar belakang di kanan
     </div>
     ```

  5. **Px (pixel)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 50px 100px;">
       Latar belakang dengan koordinat pixel
     </div>
     ```

  6. **% (persentase)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 50% 50%;">
       Latar belakang di tengah (persentase)
     </div>
     ```

  7. **em (relative unit)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-position: 2em 3em;">
       Latar belakang dengan posisi relatif em
     </div>
     ```
     
- **Background-Repeat**  
  Untuk mengatur apakah gambar latar belakang (`background-image`) diulang atau tidak, serta bagaimana pola pengulangannya ditampilkan dalam sebuah elemen.  
  Value `background-repeat` ada 6 yaitu:  

  1. **No-repeat**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: no-repeat;">
       Latar belakang tidak diulang
     </div>
     ```

  2. **repeat-x**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: repeat-x;">
       Latar belakang diulang secara horizontal
     </div>
     ```

  3. **repeat-y**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: repeat-y;">
       Latar belakang diulang secara vertikal
     </div>
     ```

  4. **space**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: space;">
       Latar belakang diulang dengan jarak antar gambar
     </div>
     ```

  5. **round**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: round;">
       Latar belakang diulang dan disesuaikan ukurannya
     </div>
     ```

  6. **space repeat**  
     ```html
     <div style="background-image: url('sample.jpg'); background-repeat: space repeat;">
       Kombinasi pengulangan dengan jarak dan pola
     </div>
     ```
     
- **Background-Size**  
  Untuk mengatur ukuran gambar latar belakang pada sebuah elemen.  
  Dengan ini, kamu bisa menentukan apakah gambar memenuhi seluruh area, menyesuaikan proporsi, atau menggunakan ukuran khusus.  
  Value `background-size` ada 4 yaitu:  

  1. **Cover**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: cover;">
       Latar belakang memenuhi seluruh area
     </div>
     ```

  2. **Contain**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: contain;">
       Latar belakang menyesuaikan proporsi
     </div>
     ```

  3. **Px (pixel)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: 200px 100px;">
       Latar belakang dengan ukuran khusus pixel
     </div>
     ```

  4. **% (persentase)**  
     ```html
     <div style="background-image: url('sample.jpg'); background-size: 50% 50%;">
       Latar belakang dengan ukuran persentase
     </div>
     ```
               

# Property dan Value dasar CSS 

---
## Inline CSS

Menyisipkan style di setiap tag HTML.

```html
<p style="color: red; font-size: 18px;">
  Teks ini menggunakan Inline CSS
</p>

---
## Internal CSS

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


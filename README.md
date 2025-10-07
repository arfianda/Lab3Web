```markdown
# Praktikum 3 – Membuat List, Table, dan Form  

Nama: Arfianda Firsta Satritama


NIM : 312410377

---
```

### 1️⃣ Membuat Ordered List  
Buat file baru bernama **`lab3_list.html`**, kemudian tambahkan struktur HTML dasar:  

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML Lanjutan</title>
</head>
<body>
  <header>
    <h1>Membuat List</h1>
  </header>

  <section id="order-list">
    <h2>Ordered List</h2>
    <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
    </ol>
  </section>
</body>
</html>
````

📸 **Screenshot Ordered List**

<img src="/img/ordered.png" width="700">

---

### 2️⃣ Membuat Unordered List

Tambahkan setelah ordered list:

```html
<section id="unorder-list">
  <h2>Unordered List</h2>
  <ul type="square">
    <li>Jaringan Komputer</li>
    <li>Struktur Data</li>
    <li>Algoritma & Pemrograman</li>
  </ul>
</section>
```

📸 **Screenshot Unordered List**

<img src="/img/unordered.png" width="700">

---

### 3️⃣ Membuat Description List

Tambahkan kode berikut:

```html
<section id="description-list">
  <h2>Description List</h2>
  <dl>
    <dt>Fakultas Teknik</dt>
    <dd>Teknik Industri</dd>
    <dd>Teknik Informatika</dd>
    <dd>Teknik Lingkungan</dd>

    <dt>Fakultas Ekonomi dan Bisnis</dt>
    <dd>Akuntansi</dd>
    <dd>Manajemen</dd>
    <dd>Bisnis Digital</dd>
  </dl>
</section>
```

📸 **Screenshot Description List**

<img src="/img/description.png" width="700">


---

### 4️⃣ Membuat Tabel

Buat file baru **`lab3_tabel.html`**, lalu tambahkan kode berikut:

```html
<table border="1" cellpadding="4" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
    </tr>
    <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
    </tr>
  </tbody>
</table>
```


---

### 5️⃣ Mengatur Margin dan Padding

Tambahkan atribut `cellpadding` dan `cellspacing`:

```html
<table border="1" cellpadding="6" cellspacing="0">
```


---

### 6️⃣ Menggabungkan Sel Data

Gunakan atribut `rowspan` dan `colspan`:

```html
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td rowspan="3">Teknik</td>
      <td>Teknik Informatika</td>
    </tr>
    <tr>
      <td>2.</td>
      <td>Teknik Industri</td>
    </tr>
    <tr>
      <td>3.</td>
      <td>Teknik Lingkungan</td>
    </tr>
  </tbody>
</table>
```

---

### 7️⃣ Membuat Form

Buat file baru **`lab3_form.html`**, kemudian tambahkan kode berikut:

```html
<form action="proses.php" method="post">
  <fieldset>
    <legend>Data Pelanggan</legend>
    <p>
      <label for="nama">Nama</label>
      <input type="text" id="nama" name="nama">
    </p>
    <p>
      <label for="alamat">Alamat</label>
      <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
      <label>Jenis Kelamin</label>
      <input id="jk_l" type="radio" name="kelamin" value="L" />
      <label for="jk_l">Laki-laki</label>
      <input id="jk_p" type="radio" name="kelamin" value="P" />
      <label for="jk_p">Perempuan</label>
    </p>
    <p><input type="submit" value="Login"></p>
  </fieldset>
</form>
``` 

---

### 8️⃣ Menambahkan Style pada Form

Tambahkan CSS agar tampilan lebih rapi:

```html
<style>
  form p > label {
    display: inline-block;
    width: 100px;
  }
  form input[type="text"], form textarea {
    border: 1px solid #197a43;
  }
  form input[type="submit"] {
    border: 1px solid #197a43;
    background-color: #197a43;
    color: #ffffff;
    font-weight: bold;
    padding: 5px 15px;
  }
</style>
```

📸 **Screenshot Form dengan CSS**

<img src="/img/css.png" width="700">

---

## 📚 Pertanyaan Praktikum

1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.


### 💡 Jawaban:

Contoh penerapan dropdown dan listbox multiple:

```html
<form>
  <p>
    <label for="jurusan">Pilih Jurusan</label>
    <select id="jurusan" name="jurusan">
      <option value="ti">Teknik Informatika</option>
      <option value="si">Sistem Informasi</option>
      <option value="mi">Manajemen Informatika</option>
    </select>
  </p>

  <p>
    <label for="hobi">Pilih Hobi</label>
    <select id="hobi" name="hobi" multiple size="3">
      <option value="coding">Coding</option>
      <option value="design">Desain Web</option>
      <option value="gaming">Gaming</option>
    </select>
  </p>
</form>
```

📸 **Screenshot Dropdown dan Listbox Multiple**

<img src="/img/multiple.png" width="700">

---


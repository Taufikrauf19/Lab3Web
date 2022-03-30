# Lab3Web

___
## NAMA     : MOH. TAUFIK RAUF
## NIM      : 312010151
## KELAS    : TI.20.A1
___


# 1. Membuat List
Buatlah dokumen HTML dengan nama file lab3_list.html seperti berikut.

Selanjutnya masuka contoh kode seperti di bawah ini
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML List</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```
Berikut perubahannya

![Membuat list](https://user-images.githubusercontent.com/101621391/160758590-89dd7144-dd65-424d-89cb-41de2b1bb879.png)

Selanjutnya menambahkan Unorderd List.

Masukan contoh kode seperti di bawah ini
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```
Berikut perubahannya
![Membuat Unorderd list](https://user-images.githubusercontent.com/101621391/160759089-3f042d18-10e4-4143-8d40-1a8a989c0aa6.png)

Langkah selanjutnya Menambahkan Description List

Masukan contoh kode berikut
```
<section id="unorder-list">
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






Berikut perubahannya

![Menambahkan Description List](https://user-images.githubusercontent.com/101621391/160760761-fcb99d8a-a554-4716-8c46-57ad10aae7ab.png)

# 2. Membuat Table
Buat file baru dengan nama lab3_tabel.html seperti berikut.

Setelah membuat file baru, selanjutnya masukan contoh kode di bawah ini
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Table</title>
</head>
<body>
    <header>
        <h1>Table Mahasiswa</h1>
    </header>
</body>
</html>
```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<table border="2" cellpadding="7" cellspacing="5">
    <thead>
        <tr>
            <th>No.</th>
            <th>Nama</th>
            <th>NIM</th>
            <th>Kelas</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Moh. Taufik Rauf</td>
            <td>312010151</td>
            <td>TI.20.A.1</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Bisma Putra</td>
            <td>312010443</td>
            <td>TI.20.A.1</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Denas Pamungkas</td>
            <td>312010234</td>
            <td>TI.20.A.1</td>
        </tr>
    </tbody>
</table>
```

Berikut perubahannya

![Membuat table](https://user-images.githubusercontent.com/101621391/160762261-4a15c072-8cda-42fe-bb89-401e434cacf4.png)

Selanjutnya jika ingin mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan
cellspacing pada tag table.

Masukan contoh kode berikut
```
<table border="2" cellpadding="7" cellspacing="5">
```

Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk
menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara
horizontal).

berikut contoh kodenya
```
<table border="2" cellpadding="7" cellspacing="5">
    <thead>
        <tr>
            <th>No.</th>
            <th>Nama</th>
            <th>NIM</th>
            <th>Kelas</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Moh. Taufik Rauf</td>
            <td>312010151</td>
            <td rowspan="3">TI.20.A.1</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Bisma Putra</td>
            <td>312010443</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Denas Pamungkas</td>
            <td>312010234</td>
        </tr>
    </tbody>
</table>
```

Berikut perubahannya

![Menyatukan Table Kelas](https://user-images.githubusercontent.com/101621391/160785256-901f23d0-7f8b-49e6-ab37-801e4c9cea46.png)

# 3. Membuat Form
Buatlah file baru denan nama lab3_form.html seperti berikut.
Masukan contoh kode berikut
```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Form</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:

```
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
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
        </p>
        <p>
            <input type="submit" value="Login"></p>
    </fieldset>
</form>
```

Berikut tampilan Form nya.

![Membuat Form](https://user-images.githubusercontent.com/101621391/160786575-be9a8a61-3c58-40a7-bef9-1c6fe7e9b97c.png)

Agar tampilan form lebih menarik, bisa ditambahkan CSS.
Buatlah dokumen CSS dengan nama style.css seperti berikut

Selanjutnya masukan kode seperti berikut di dokumen CSS yang telah dibuat.

```
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
```

Berikut perubahannya.

![menambahkan style css](https://user-images.githubusercontent.com/101621391/160787362-41459f13-4719-4c34-b050-b0504f548564.png)

>DEMIKIAN JIKA ADA SALAH - SALAH KATA MOHON DI MAAFKAN

>TERIMA KASIH

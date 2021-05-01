# Lab5Web

# Praktikum 5

# Pemograman WEB

~~~
Nama  : Isnaini Rizkyana
NIM   : 311910254
Kelas : TI.19.C1
~~~
## Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
~~~
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>Mengenal JavaScript</title>
    </head>
    <body>
        <h1>Pengenalan JavaScript</h1>
        <h3>Contoh document.write dan console.log</h3>
        <script>
            document.write("Hello World");
            console.log("Hello World");
        </script>
    </body>
</html>
~~~

![Skrip Javascript](https://user-images.githubusercontent.com/81541764/116781995-c28e3e00-aab0-11eb-8d4b-a370ccecdb57.JPG)


## Javasript Dasar
Pemakaian Alert sebagai property window.
~~~
<html>
    <head>
        <title>Alert Box</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
            window.alert("Ini merupakan pesan untuk anda");
            //-->
        </script>
    </body>
</html>
~~~
![Pemakaian Alert sebagai property window](https://user-images.githubusercontent.com/81541764/116781894-1c423880-aab0-11eb-8a32-b6494ebe4681.JPG)


Pemakaian method dalam objek
~~~
<html>
    <head>
        <title>Skrip JavaScript</title>
    </head>
    <body>
        Percobaan memakai javascript:<br>
        <script language = "javascript">
            <!--document.write("Selamat mencoba javascript<br>");
                document.write("Semoga Sukses!");
                -->
        </script>
    </body>
</html>
~~~
![Method](https://user-images.githubusercontent.com/81541764/116781935-62979780-aab0-11eb-84cf-c105e233da99.JPG)

Pemakaian Prompt
~~~
<html>
    <head>
        <title>Pemasukan data</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nama = prompt("Siapa nama anda?", "Masukan nama anda");
                document.write("Hai, " + nama);
                -->
        </script>
    </body>
</html>
~~~
![Pemakaian Prompt](https://user-images.githubusercontent.com/81541764/116781955-8529b080-aab0-11eb-973e-0160e846dbfa.JPG)

Pembuatan fungsi dan cara pemanggilannya
~~~
<html>
    <head>
        <title>Contoh program javascript</title>
        <script language="javascript">
            function pesan(){
                alert ("Memanggil javascript lewat body onload")
            }
        </script>
    </head>
    <body onload=pesan()>
    </body>
</html>
~~~
![Pembuatan fungsi dan cara pemanggilannya](https://user-images.githubusercontent.com/81541764/116782016-e3ef2a00-aab0-11eb-9382-4fe2dad77a62.JPG)

## Dasa Pemrograman Di Javascript
Operasi dasar aritmatika
~~~
<html>
    <head>
        <title>Contoh Program Javascript</title>

        <script language="Javascript">
            function test (val1,val2)
            {
                document.write("<br>"+"perkalian : val1*val2 "+"<br>")
                document.write(val1*val2)
                document.write("<br>"+"pembagian : val1/val2"+"<br>")
                document.write(val1/val2)
                document.write("<br>"+"penjumlahan : val1+val2"+"<br>")
                document.write(val1+val2)
                document.write("<br>"+"pengurangan : val1-val2"+"<br>")
                document.write(val1-val2)
                document.write("<br>"+"modulus : val1%val2"+"<br>")
                document.write(val1%val2)
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
    </body>
</html>
~~~
![Operasi Arithmetic 1`](https://user-images.githubusercontent.com/81541764/116782039-1436c880-aab1-11eb-972e-f05c43a6be13.JPG)

Seleksi kondisi (if..else)
~~~
<html>
    <head>
        <title>Contoh if-else</title>
    </head>
    <body>
        <script language = "javascript">
            <!--
                var nilai = prompt("nilai (0-100):", 0)
                var hasil = "";
                if (nilai >= 60)
                hasil = "lulus";
                else
                hasil = "tidak lulus";
                document.write("hasil: " + hasil);
                //-->
        </script>
    </body>
</html>
~~~
![Seleksi kondisi (if else)](https://user-images.githubusercontent.com/81541764/116782059-33cdf100-aab1-11eb-8cb7-bc8e0818e745.JPG)

Penggunaaan Operator Switch untuk seleksi kondisi
~~~
<html>
    <head>
        <title>Contoh Program javascript</title>

        <script language="javascript">
            function test ()
            {
                val1=window.prompt("input nilai (1-5):")
                switch (val1)
                {
                    case "1" :
                        document.write("bilangan satu")
                        break
                    case "2" :
                        document.write("bilangan dua")
                        break
                    case "3" :
                        document.write("bilangan tiga")
                        break
                    case "4" :
                        document.write("bilangan empat")
                        break
                    case "5" :
                        document.write("bilangan lima")
                        break
                    default :
                        document.write("bilangan lainnya")
                        break
                }
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
</html>
~~~
![operator switch untuk seleksi kondisi](https://user-images.githubusercontent.com/81541764/116782083-5cee8180-aab1-11eb-9e23-f026543d5c8e.JPG)

## Pembuatan Form
Form Input
~~~
<html>
    <head>
        <script language="javascript">
            function test () {
               var val1=document.kirim.T1.value
               if (val1%2==6)
                    document.kirim.T2.value="bilangan genap" 
                else
                    document.kirim.T2.value="bilangan ganjil"
            }
        </script>
    </head>
    <body>
        <form method="POST" name="kirim">
            <p>BIL <input type="text" name="T1" size="20">
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
        </form>
    </body>
</html>
~~~
![Form Input](https://user-images.githubusercontent.com/81541764/116782102-78f22300-aab1-11eb-957f-09b2313987a3.JPG)

Form Button.
~~~
<html>
    <head>
        <title>Object Document</title>
    </head>
    <body>
        <script language="javascript">
            <!--
                function ubahWarnaLB(warna) {
                    document.bgColor = warna;
                }
                function ubahWarnaLD(warna) {
                    document.bgColor = warna;
                }
                //-->
        </script>

        <h1>tes</h1>
        <form>
            <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
            <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
            <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
            <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
        </form>
        <script language="javascript">
            <!--
                document.write("Dimodifikasi terakhir pada "+
                document.lastModified);
                //-->
        </script>
    </body>
</html>
~~~
![Form Button](https://user-images.githubusercontent.com/81541764/116782120-91fad400-aab1-11eb-85fb-2dc8291eeac1.JPG)

## HTML DOM
### Pilihan menggunakan checkBox dengan perhitungan otomatis
~~~
<!--
    File: daftar_menu.html
//-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;
            
            if (ele.checked) {
                harga = ele.value;
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>    
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"> Ayam Goreng Rp. 5.000</label><br>
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"> Tempe Goreng Rp. 500</label><br>
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"> Telur Dadar Rp. 2.500</label><br>
    <strong>Total Bayar: Rp. <input id="total" type="text"/></strong>
</body>
</html>
~~~
![Checkbox](https://user-images.githubusercontent.com/81541764/116782572-26663600-aab4-11eb-9ef3-494c7b105311.JPG)

## Pertanyaan dan Tugas
1. Buat script untuk melakukan validasi pada isian form.

~~~
<!DOCTYPE html>
<html>
<head>
	<title>Membuat Form Validasi dengan Javascript</title>
	<link rel="stylesheet" type="text/css" href="style_form.css">
</head>
<body>
	<center><h2>PENGISIAN FORM</h2></center>
	<div class="login">
		<form action="#" method="POST" onSubmit="validasi()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
<script type="text/javascript">
	function validasi() {
		var nama = document.getElementById("nama").value;
		var email = document.getElementById("email").value;
		var alamat = document.getElementById("alamat").value;
		if (nama != "" && email!="" && alamat !="") {
			return true;
		} else {
			alert('Anda harus mengisi data dengan lengkap !');
		}
	}
</script>
</html>
~~~
![Form pengisian (Source)](https://user-images.githubusercontent.com/81541764/116782828-91643c80-aab5-11eb-8847-be26926b8af8.JPG)

Simpan dan refresh browser, kemudian lihat hasilnya seperti dibawah ini.
![Form pengisian](https://user-images.githubusercontent.com/81541764/116782763-32062c80-aab5-11eb-932a-feed13483f2c.JPG)


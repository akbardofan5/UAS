# UAS
username Dofan <br>
password 123456 <br>
https://akbardofan5.000webhostapp.com/ <br>
<br>
session_start(); digunakan untuk memulai session <br>
<br>
if(isset($_SESSION['id_user'])) { digunakan untuk mengecek apakah user sudah login atau tidak <br>
  header("Location: ./index.php"); redirect ke index.php jika login success <br>
  die(); <br>
} <br>
<br>
session_destroy(); digunakan untuk menghapus session yang aktif <br>
<br>
//skrip untuk menampilkan data dari database <br>
$sql = mysqli_query($conn, "SELECT * FROM covid19"); //script query untuk mengambil semua data dari table covid19 <br>
if(mysqli_num_rows($sql) > 0) { //mengecek apakah ada data di dalam table transaksi atau tidak, jika ada maka query akan di jalankan <br>
  while($row = mysqli_fetch_array($sql)) { <br>
<br>
$dt = new DateTime('now', new DateTimezone('Asia/Jakarta')); digunakan untuk menentukan timezone <br>
echo $dt->format("d F Y H:i:s"); digunakan untuk format waktu dan tanggal <br>
<br>
Comment yang lebih lengkap ada di filenya <br>

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

# UAS
username Dofan <br>
password 123456 <br>
https://akbardofan5.000webhostapp.com/

<?php
  //memulai session
  session_start();

  //jika ada session, maka akan diarahkan ke halaman dashboard admin
  if(isset($_SESSION['id_user'])){
      //mengarahkan ke halaman dashboard admin
      header("Location: ./index.php");
      die();
  }

  include "config.php";
?>

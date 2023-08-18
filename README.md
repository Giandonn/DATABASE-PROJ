# DATABASE-PROJ
<?php 
function openCon(){
$dbhost = "localhost";
$dbuser = "raineri";
$dbpass = "0512";
$db = "teste";
$conn = new mysqli($dbhost, $dbuser, $dbpass, $db) or die ("connection failed".$conn-> error);
return $conn;
}
function CloseCon($conn){
    $conn -> close();
}
?>

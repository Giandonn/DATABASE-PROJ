
<?php 
function openCon(){
$dbhost = "";
$dbuser = "";
$dbpass = "";
$db = "teste";
$conn = new mysqli($dbhost, $dbuser, $dbpass, $db) or die ("connection failed".$conn-> error);
return $conn;
}
function CloseCon($conn){
    $conn -> close();
}
?>

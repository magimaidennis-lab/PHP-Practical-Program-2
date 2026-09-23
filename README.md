# PHP-Practical-Program-2

<!DOCTYPE html>
<html>
<head>
<title>PHP Operations</title>
<style>
body{text-align:center;font-family:Arial;}
input{padding:8px;margin:5px;}
</style>
</head>

<body>
<h2>PHP Calculator</h2>

<form method="post">
<input type="number" name="a" placeholder="Number 1" required><br>
<input type="number" name="b" placeholder="Number 2" required><br>
<input type="submit" name="submit" value="Calculate">
</form>

<?php
if(isset($_POST['submit'])){
    $a=$_POST['a'];
    $b=$_POST['b'];

    echo "Addition = ".($a+$b)."<br>";
    echo "Subtraction = ".($a-$b)."<br>";
    echo "Multiplication = ".($a*$b)."<br>";
    echo "Division = ".($a/$b);
}
?>
</body>
</html>


Input 
Number 1 = 20
Number 2 = 5


Output 
Addition = 25
Subtraction = 15
Multiplication = 100
Division = 4

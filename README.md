# PHP-MySQL-Software-University
Homeworks from fast track PHP &amp; MySQL

<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title></title>
    </head>
    <body>
        <form method="post" action="index.php">
            <input type="text" name="number1">
            <input type="text" name="number2">
            <input type="submit" value="exchange">
        </form>
    </body>
</html>
        <?php
        $num1=$_POST['number1'];
        $num2=$_POST['number2'];
        if ($num1>$num2)
        {
            echo 'At start:'.'<t>'.'First number:'.$num1.'<br>'.'Second number:'.$num2.'<br><br>';
            $temp=$num1;
            $num1=$num2;
            $num2=$temp;
            echo 'At Last:'.'<t>'.'First number:'.$num1.'<br>'.'Second number:'.$num2;
        }
        else
        {
            echo 'Second number is greater or equal';
        }
        ?>

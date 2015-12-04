<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Регистр верхний и нижний</title>
    </head>
    <body>
        <script LANGUAGE="JavaScript" TYPE="text/javascript">
            function my_on_click() {
                alert("Вы ввели "+document.forms["myform"].elements[0].value);      
                letter= document.forms["myform"].elements[0].value;
                alert (letter);    
                x= letter.charAt(0);
                alert (x);     
                    if (x.toUpperCase()==x) alert('Верно');
                    else alert('Первая буква должна быть большой');

                 var c= letter.length;
                 alert ("Число букв " +(c));    

                for (i=1;i<c;i++)
                 {
                    var n=i+1;
                    alert ("буква " + (letter.charAt(i)));
                    if (letter.charAt(i).toUpperCase() == letter.charAt(i)) alert((n) + "-ая буква должна быть маленькой");
                }    
            }
        </script>
        <form name="myform">
            Введите что нибудь: <input type="text" name="TextBox" size="20">
            <input type="submit" value="Submit" name="ButtonOk" onClick="my_on_click()">
            <input type="reset" value="Reset" name="ButtonCancel">
        </form>
    </body>
</html>

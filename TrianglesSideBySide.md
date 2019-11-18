```php
<?php
header('Content-Type: text/plain');
function DrawFirst(int $levels, int $i)
{
    for($j=0;$j<floor($levels-$i);$j++)
               echo " ";
       for($j=0;$j<(2*$i)-1;$j++)
               echo "*";
}

function DrawOneMore(int $levels, int $i)
{
    for($j=0;$j<2*floor($levels-$i);$j++)
               echo " ";
       for($j=0;$j<(2*$i)-1;$j++)
               echo "*";
}

$levels = 10;
for($i=0;$i<$levels;$i++){

        DrawFirst($levels,$i);
        DrawOneMore($levels,$i);
        DrawOneMore($levels,$i);
        DrawOneMore($levels,$i);
        
echo "\n";
}
?>

```
```
output:
                                                                      
         *                  *                  *                  *
        ***                ***                ***                ***
       *****              *****              *****              *****
      *******            *******            *******            *******
     *********          *********          *********          *********
    ***********        ***********        ***********        ***********
   *************      *************      *************      *************
  ***************    ***************    ***************    ***************
 *****************  *****************  *****************  *****************
 ```
```php
<?php

function DrawOneMore(int $levels, int $i)
{
    for($j=0;$j<2*floor($levels-$i);$j++)
               echo " ";
       for($j=0;$j<(2*$i)-1;$j++)
               echo "*";
}
header('Content-Type: text/plain');
$levels = 10;

for($i=0;$i<$levels;$i++){

       for($j=0;$j<floor($levels-$i);$j++)
               echo " ";
       for($j=0;$j<(2*$i)-1;$j++)
               echo "*";

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
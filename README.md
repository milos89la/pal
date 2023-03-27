# pal
pal


<?php

function Palindrom($string) {

if ((strlen($string) == 1) || (strlen($string) == 0)) {
    echo " STRING JESTE PALINDROM";
}

else {

    if (substr($string,0,1) == substr($string,(strlen($string) - 1),1)) {
        return Palindrom(substr($string,1,strlen($string) -2));
    }
    else { echo " STRING NIJE PALINDROM"; }
}
}


Palindrom("anavolimilovana");

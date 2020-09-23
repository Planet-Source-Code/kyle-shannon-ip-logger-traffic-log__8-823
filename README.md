<div align="center">

## IP Logger / Traffic Log


</div>

### Description

Logs IP addresses and Traffic
 
### More Info
 
make iplog.txt and CHMOD 777

IP and Date


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Kyle Shannon](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/kyle-shannon.md)
**Level**          |Beginner
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__8-1.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/kyle-shannon-ip-logger-traffic-log__8-823/archive/master.zip)





### Source Code

```
<?php
//       (( Script Written By Kyle Shannon ))
// ((           www.myownpill.com            ))
// __________________________________________________________________________
// Instructions
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
// CHMOD iplog.txt to 777
// Put this script inside a .php file on your site
// For each person who visits their IP address will be logged in the iplog.txt
// __________________________________________________________________________
// The Code
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
//
$td = date("F jS");
 $ip = $REMOTE_ADDR; // Set the variable as their ip address
 $fh = fopen("iplog.txt",'a+'); // Open the text file and tell it to add
  fputs($fh, "$ip : $td<br><br>"); // Add the ip address onto the next line
  fclose($fh); // Close the text file
//
// __________________________________________________________________________
// End Code
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
//
?>
```


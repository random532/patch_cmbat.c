# patch_cmbat.c
This adds battery warning levels to FreeBSD control method batteries - highly experimental :-)

Catch the warnings via "CMBAT" devd notify events.<br>
The patch applies to the file (/usr/src/)sys/dev/acpica/cmbat.c<br>
Up to three new sysctls:<br> 
dev.cmbat.0.Any<br>
dev.cmbat.0.Low<br>
dev.cmbat.0.CriticallyLow<br>
<br>
It probably crashes if you have more than one battery.

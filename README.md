# reset-NX-OS
Procédure de reset pour NX-OS

CTRL + C
bootflash://m9100-s5ek9-kickstart-mz.6.2.25.bin
switchboot#configure terminal
switch(boot-config)#admin-password password
switch(boot-config)#exit

switchboot#
switch(boot)#load bootflash:m9100-s5ek9-mz.6.2.25.bin

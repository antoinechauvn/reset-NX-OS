# reset-NX-OS
Procédure de reset pour Cisco Nexus (NX-OS)

### Image Kickstart
L'image Kickstart contient le noyau Linux, les pilotes de base et le système de fichiers initial.

### Image Système
L'image système contient le logiciel système et le code d'infrastructure.

## Procédure
1. Lorsque le switch démarre, lancer le bootloader avec la séquence `CTRL + C`
2. Charger l'image kickstart en utilisant la commande `bootflash://m9100-s5ek9-kickstart-mz.6.2.25.bin`
3. Entre en mode configuration `switchboot#configure terminal`
4. Changer le mot de passe `switch(boot-config)#admin-password password`
5. Charger l'image système `switch(boot)#load bootflash:m9100-s5ek9-mz.6.2.25.bin`

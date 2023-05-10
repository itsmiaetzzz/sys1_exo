# Level Telnet - Authentification 
# Level goal : 
Retrouvez le *mot de passe de l’utilisateur *dans cette *capture réseau de session TELNET*.



# Etapes à suivre:

- _Télécharger le lien_:
Clic droit sur le bouton *démarrer le challenge* , copier le lien et l'ouvrir sur un autre onglet pour le télecharger . 

- _Chercher le mot de passe_ : 
Ouvrir le fichier sur Wireshark . 
Choisir un paquet à protocole *Telnet* et clic droit pour pouvoir *suivre* ce protocole et appuyer sur le flux TCP.
```
........... ..!.."..'.....#..%..%........... ..!..".."........P. ....".....b........b....	B.
........................"......'.....#..&..&..$..&..&..$.. .....#.....'........... .9600,9600....#.bam.zing.org:0.0....'..DISPLAY.bam.zing.org:0.0......xterm-color.............!.............."............
OpenBSD/i386 (oof) (ttyp1)

login: .."........"ffaakkee
.
Password:user
.
Last login: Thu Dec  2 21:32:59 on ttyp1 from bam.zing.org
Warning: no Kerberos tickets issued.
OpenBSD 2.6-beta (OOF) #4: Tue Oct 12 20:42:32 CDT 1999

Welcome to OpenBSD: The proactively secure Unix-like operating system.

Please use the sendbug(1) utility to report bugs in the system.
Before reporting a bug, please try to reproduce it with the latest
version of the code.  With bug reports, please try to ensure that
enough information to reproduce the problem is enclosed, and if a
known fix for it exists, include that as well.


```
Le password est affiché à la partieà côté de * password:*, que l'on entrera ensuite sur l'input du site : Entrer le mot de passe . 







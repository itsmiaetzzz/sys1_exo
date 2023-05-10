# Level FTP - Authentification 
# Level goal : 
Un échange authentifié de fichier réalisé grâce au protocole FTP. Retrouvez le *mot de passe utilisé par l’utilisateur*.

# Etapes à suivre:

- _Télécharger le lien_:
Clic droit sur le bouton *démarrer le challenge* , copier le lien et l'ouvrir sur un autre onglet pour le télecharger . 

- _Chercher le mot de passe_ : 
Ouvrir le fichier sur Wireshark . 
Choisir un paquet à protocole TCP et clic doit pour pouvoir suivre ce protocole et appuyer sur le flux TCP.
```
220-QTCP at fran.csg.stercomm.com.
220 Connection will close if idle more than 5 minutes.
USER cdts3500
331 Enter password.
PASS cdts3500
230 CDTS3500 logged on.
SYST
215  OS/400 is the remote operating system. The TCP/IP version is "V5R2M0".
SITE NAMEFMT
250  Now using naming format "0".
PWD
257 "CDTS3500" is current library.
PASV
227 Entering Passive Mode (10,20,144,151,62,141).
RETR qgpl/apkeyf.apkeyf
150 Retrieving member APKEYF in file APKEYF in library QGPL.
250 File transfer completed successfully.
QUIT
221 QUIT subcommand received.

```
Le password est affiché à la partie en-dessous de *Enter password*, que l'on entrera ensuite sur l'input du site : Entrer le mot de passe . 







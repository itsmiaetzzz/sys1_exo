# Level Telnet - Authentification 
# Level goal : 
Retrouvez les *données normalement confidentielles* contenues dans cette trame.


# Etapes à suivre:

- _Télécharger le lien_:
Clic droit sur le bouton *démarrer le challenge* , copier le lien et l'ouvrir sur un autre onglet pour le télecharger . 

- _Chercher les données confidentielles_ : 


```

00 05 73 a0 00 00 e0 69 95 d8 5a 13 86 dd 60 00
00 00 00 9b 06 40 26 07 53 00 00 60 2a bc 00 00
00 00 ba de c0 de 20 01 41 d0 00 02 42 33 00 00
00 00 00 00 00 04 96 74 00 50 bc ea 7d b8 00 c1
d7 03 80 18 00 e1 cf a0 00 00 01 01 08 0a 09 3e
69 b9 17 a1 7e d3 47 45 54 20 2f 20 48 54 54 50
2f 31 2e 31 0d 0a 41 75 74 68 6f 72 69 7a 61 74
69 6f 6e 3a 20 42 61 73 69 63 20 59 32 39 75 5a
6d 6b 36 5a 47 56 75 64 47 6c 68 62 41 3d 3d 0d
0a 55 73 65 72 2d 41 67 65 6e 74 3a 20 49 6e 73
61 6e 65 42 72 6f 77 73 65 72 0d 0a 48 6f 73 74
3a 20 77 77 77 2e 6d 79 69 70 76 36 2e 6f 72 67
0d 0a 41 63 63 65 70 74 3a 20 2a 2f 2a 0d 0a 0d
0a
```
-Convertir la série : 
Cette série est écrit en écriture *hexadécimale*. 
Il est donc nécessaire de le convertir en *type ASCII* pour pouvoir afficher le texte . 

Pour cela , on va devoir trouver un site sur Google qui permet cette conversion . 
HexToASCII[https://www.rapidtables.com/convert/number/hex-to-ascii.html].

Celà nous donnera un texte : 

```
...
Authorization: Basic Y29uZmk6ZGVudGlhbA==
User-Agent: InsaneBrowser
Host: www.myipv6.org
```

Nous remarquerons ensuite qu'il y a   Authorization : Basic + une série en Bite64 
Bite64 : c'est une sérue de chiffre et de lettre précédé par un == ou un = .

Nous allons donc devoir decode la série Bite64 sur le site Base64[https://www.base64decode.org/].





# Level  Authentification Twitter
# Level goal : 
Une session d’authentification twitter a été capturée.
Retrouvez le *mot de passe de l’utilisateur dans cette capture réseau*. 



# Etapes à suivre:

- _Télécharger le lien_:
Clic droit sur le bouton *démarrer le challenge* , copier le lien et l'ouvrir sur un autre onglet pour le télecharger . 

- _Chercher le mot de passe_ : 
Ouvrir le fichier sur Wireshark . 
Choisir un paquet à protocole *HTTP* et clic droit pour pouvoir *suivre* ce protocole et appuyer sur le flux HTTP.
```

GET /statuses/replies.xml HTTP/1.1
User-Agent: CFNetwork/330
Cookie: _twitter_sess=BAh7CDoJdXNlcjA6B2lkIiVmZGQ2ODc5MTMwMWFhOTFiMWExZDViZmQwMGEz%250AOWNkMyIKZmxhc2hJQzonQWN0aW9uQ29udHJvbGxlcjo6Rmxhc2g6OkZsYXNo%250ASGFzaHsABjoKQHVzZWR7AA%253D%253D--ea12e7bc090d05202cd7e3f972c2b4414a97f657
Accept: */*
Accept-Language: en-us
Accept-Encoding: gzip, deflate
Authorization: Basic dXNlcnRlc3Q6cGFzc3dvcmQ=
Connection: keep-alive
Host: twitter.com


```
Nous remarquerons ensuite qu'il y a Authorization : Basic + une série en Bite64 Bite64 : c'est une sérue de chiffre et de lettre précédé par un == ou un = .

Nous allons donc devoir decode la série Bite64 sur le site [Base64](https://www.base64decode.org/).

Le password est affiché à la partie decode , que l'on entrera ensuite sur l'input du site : Entrer le mot de passe .








# Level Telnet - Authentification 
# Level goal : 
Votre ami travaillant à l’ANSSI a récupéré un fichier illisible dans l’ordi d’un hacker. Tout ce qu’il sait est que cela provient d’un échange entre un ordinateur et un téléphone. A vous d’en apprendre le plus possible sur ce téléphone.

La réponse est le *hash SHA1 de la concaténation de l’adresse MAC* (en majuscules) et du* nom du téléphone*.
```


Exemple :
AB:CD:EF:12:34:56monTelephone -> 836eca0d42f34291c5fefe91010873008b53c129
```



# Etapes à suivre:

- _Télécharger le lien_:
Clic droit sur le bouton *démarrer le challenge* , copier le lien et l'ouvrir sur un autre onglet pour le télecharger . 

- _Chercher le mot de passe_ : 
Ouvrir le fichier sur Wireshark . 
Il faut commencer par chercher le nom du téléphone : 
on va dans "Wireless" puis on appuie sur Equipement bluetooth et là on voit la colonne Nom du télephone que l'on notera . 
et l'adresse Mac se situe sous la section BD_ADDR .

Pour effectuer la concaténation , il est nécessaire de changer les lettres minuscules de l'adresse MAC en majuscules et ajouter le nom du telephone à côté de l'adresse MAC.

On accède ensuite au site [SHA](https://10015.io/tools/sha1-encrypt-decrypt).

On encrypte pour avoir la réponse.








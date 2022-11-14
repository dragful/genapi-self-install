<!-- Installation de poste sous sous Genapi -->


![This is an image](https://i.ibb.co/b7StCSQ/Sans-titre.png)

# Installation de poste sous Genapi Inot #

![](https://img.shields.io/github/workflow/status/yzhang-gh/vscode-markdown/CI?style=flat-square) ![](https://img.shields.io/github/contributors/yzhang-gh/vscode-markdown.svg?style=flat-square)

*Fonctionne sous windows 10 et 11 (64 bits)*

- [Installation de poste sous Genapi Inot](#installation-de-poste-sous-genapi-inot)
  - [Prérequis](#prérequis)
    - [Installation de windows professionnel 10 ou 11 en 64 bits](#installation-de-windows-professionnel-10-ou-11-en-64-bits)
    - [Raccordement au domaine local de l'étude après création d'un utilisateur directement sur le serveur](#raccordement-au-domaine-local-de-létude-après-création-dun-utilisateur-directement-sur-le-serveur)
    - [Modification des messages d'alerte](#modification-des-messages-dalerte)
    - [Installation d'office](#installation-doffice)
    - [Logiciels complémentaires](#logiciels-complémentaires)
  - [Modifier le fichier host de windows](#modifier-le-fichier-host-de-windows)
  - [Connecter le dossier local F:](#connecter-le-dossier-local-f)
  - [Installer la version mobilité d’Inot](#installer-la-version-mobilité-dinot)
  - [Remplacer les proxy du système](#remplacer-les-proxy-du-système)
- [Disclaimer](#disclaimer)






## Prérequis

Il est nécessaire que les paramètres suivants ayant été configurés avant de réaliser l'installation d'Inot sur le poste.

### Installation de windows professionnel 10 ou 11 en 64 bits

[Téléchargez windows 10 pro](https://wid.lecrabeinfo.net/?file=Win10_22H2_French_x64)
ou
[Téléchargez windows 11 pro](https://wid.lecrabeinfo.net/?file=Win11_22H2_v1_French_x64)

### Raccordement au domaine local de l'étude après création d'un utilisateur directement sur le serveur
### Modification des messages d'alerte
### Installation d'office
Supprimer la préinstallation d'office dans Windows (Programmes / supprimer le programme)
[Téléchargez MS Office Professionnel Plus 2021](https://wid.lecrabeinfo.net/?file=ProPlus2021Retail)
Veiller à installer la version 32bits et non 64 bits !

### Logiciels complémentaires ##

*Installer les logiciels dans leur ordre de numérotation*

1. Pack securité Real / lire le Readme dans le dossier avant de lancer l'installation
2. Flash player
3. Acrobat Reader
4. Fonts
   1. Selectionner tous les polices en meme temps (sauf dossier "reg")
   2. Clic-droit : installer
5. Java runtime
6. Silverlight
7. Dans l'hypothèse où Office 2021 ne peut être installé en 32 bits (voir supra), utiliser cette version de l'installeur, puis au moment d'entrer votre clef 2021, accepter la mise à jour (longue) vers office 2021.
8. En toute fin de l'installation du poste, dans l'hypothèse où le tableau de bord ne s'installe pas correctement (voir infra), utiliser cette version à la place.



## Modifier le fichier host de windows ##



Aller à
>C:\windows\system32\drivers\etc\

Ajouter la ligne suivante en bas du fichier : 
>192.168.2.8         *NOM DU SERVEUR*

(adapter selon la configuration de votre serveur IP – NOM)

## Connecter le dossier local F: ##


## Installer la version mobilité d’Inot ##

http://*nom_du_serveur*:55555/inot/GenApi.TableauDeBord.application
 
> adapter le nom du serveur selon !
 

## Remplacer les proxy du système ##

adresse:
> http=127.0.0.1:80;https=proxy.notaires.fr:8080

sauf : 

> 192.168.2.*;sr12-prod-2016*;*wsoid*;192.168.0.*;127.0.0.*;*.DROIT.LOCAL;*.genapi.espace.notaires.fr;sr12-prod-2016;sr12-prod-2016.droit.local;sr16-dc-2018;g002482-vm10-01;192.168.43.*;100.80.159.*;10.16.5.*;10.37.4.*;*.integral-voice.com*;*.lifesizecloud.com;wsoid.*
 
*(les modifier dans les paramètres proxy (taper « touche windows » puis le mot « proxy » au clavier et remplacer les paramètres existants.*
 






***
# Disclaimer

*Ce protocole d'installation n'est pas agréé par Septeo / Genapi / inot, il s'agit d'un tutoriel incitant les utilisateurs à mieux comprendre leurs outils de travail.
Le rédacteur de ce tutoriel ne  peut en aucun cas être tenu responsable des conséquences d'une telle installation qui n'a pas vocation à être utilisé dans un environnement de production sécurisé.*
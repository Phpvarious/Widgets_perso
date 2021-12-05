# Widget Info du jour.

![](doc/images/capture1.png)

## 1) Téléchargement du Widget.
- Fichier source à récupérer sous :
  - /widgets_perso/Info_du_jour/cmd.info.string.Info_du_jour.html
- Puis déposer ce fichier (avec JeeXplorer ...) dans le dossier :
  - /html/data/customTemplates/dashboard/
 
 ![](doc/images/capture2.png)

## 2) Création d'un virtuel.
- Commande info Autre, puis sauvegarder (1).
- Attention, ne pas historiser (2).
- Associer le widget à la commande info.(3, 4 et 5).

![](doc/images/installation_virtuel2.png)
![](doc/images/installation_virtuel3.png)


- Paramètres Optionnels :

     couleurText :       	Couleur du texte - . Exemple : white, #ffffff ..... [Défaut : #c3c3c3]

## 3) Création du scénario.

- Fichier source à télécharger :
  - /widgets_perso/Info_du_jour/Info du jour.json
  
- une fois le scénario téléchargé créér un nouveau scénario puis ajouter un template :

![](doc/images/scenario1.png)

- Charger un template et ajouter le fichier téléchargé précedemment (Info du jour.json):

![](doc/images/scenario2.png)

- Une fois chargé, celui-ci devrait apparaitre dans le menu de gauche, cliquez dessus :

![](doc/images/scenario3.png)

- (1) allez rechercher le virtuel créé précedemment.
- (2) Appliquer les modifications.
- une fenêtre demandera une confirmation, cliquez OK. puis sauvegardez le scénario.

![](doc/images/scenario4.png)

Le scénario a un CRON de 1 minute par défaut.

[SUITE =>](README2.md)
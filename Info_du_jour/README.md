# Widget Info du jour.

![](doc/images/capture1.png)

- Info disponible sur le widget :
  - Date du jour.
  - Saint du jour (et du lendemain au survol).
  - Mode Jour/nuit. (changement de couleur du Background)
  - Férié. (Prochain férié au survol)
  - Week-end.
  - Vacances. (Infos/prochaines au survol)
  - coucher/lever du soleil. (avec animation de l'élévation en cours)
  - Saison. (représentée par l'image haut a droite)

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
  
- une fois le fichier téléchargé crééz un nouveau scénario puis ajouter un template :

![](doc/images/scenario1.png)

- Charger un template et ajouter le fichier téléchargé précedemment (Info du jour.json):

![](doc/images/scenario2.png)

- Une fois chargé, celui-ci devrait apparaitre dans le menu de gauche, cliquez dessus :

![](doc/images/scenario3.png)
- Dans la nouvelle fenêtre :
  - allez rechercher le virtuel créé précedemment (1).
  - Appliquer les modifications (2).
  - une fenêtre demandera une confirmation, cliquez OK. puis sauvegardez le scénario.

![](doc/images/scenario4.png)

Le scénario a un CRON de 5 minutes par défaut.

## 4) Configuration.
Une fois toutes ces étapes faites, ouvrez le scénario et modifiez la zone vous concernant pour les vacances scolaire.

![](doc/images/config1.png)

Ensuite il faudra configurer la zone géographique dans la configuration Jeedom.
- Pour ceci rendez-vous dans Réglages/Sytème/Configuration.
- puis dans l'onglet général, en bas renseignez les informations :

![](doc/images/config2.png)

## 5) Options.

Il est possible d'extraire plus d'infos du scénario.
Il vous faudra creer de nouvelles actions (event) dans celui-ci et ajouter des infos dans votre virtuel.

|Tag scénario|Type Info virtuel|Détail|
|---|---|---|
|tag(leverSoleilScenario)|Numérique|Exemple : 831 (8h31)
|tag(zenithSoleilScenario)|Numérique|Exemple : 1249 (12h49) |
|tag(coucherSoleilScenario)|Numérique|Exemple : 1707 (17h07) |
|tag(saintJour)|Autre| Saint du jour|
|tag(saintDemain)|Autre| Saint du lendemain|
|tag(daynumber)|Numérique| |
|tag(modeJourBinaire)|Binaire|1=Jour|
|tag(ferie)|Binaire| 1=Férié|
|tag(weekend)|Binaire| 1=WE|
|tag(vacancesEnCours)|Binaire| 1=Vacances|
|tag(saison)|Autre| Printemps/Eté...|

![](doc/images/scenario4.png)



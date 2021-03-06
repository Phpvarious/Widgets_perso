# Widget swiper Battery Jeedom

![](doc/images/capture1.gif)

## 1) Téléchargement du Widget
- Fichier/dossier source à récupérer sous :
  - (dossier) /widgets_perso/swiper_battery_jeedom/cmd.info.string.swiper_battery_jeedom
  - (fichier) /widgets_perso/swiper_battery_jeedom/cmd.info.string.swiper_battery_jeedom.html
- Puis déposer ce fichier et dossier (avec JeeXplorer ...) dans le dossier :
  - /html/data/customTemplates/dashboard/
 
 ![](doc/images/capture3.png)

## 2) Création d'un virtuel
- Ajoutez une commande Info/Autre, puis sauvegarder (1).
- Attention, ne pas historiser (2).
- Associez le widget à la commande Info/Autre,(3, 4 et 5).

![](doc/images/installation_virtuel2.png)
![](doc/images/installation_virtuel3.png)

## 3) Paramètres Optionnels.

     effect : [Numérique 0 à 5] - 	Type de widget. [Défaut : 0 -> coverflow, 1 -> cube, 2 -> flip, 3 -> fade, 4 -> cards, 5 -> creative]
	 (1) disponible uniquement si "effect" = 0
	 slidesPerView (1) [Numérique, ou auto] - 	Nombres de tuiles à afficher en même temps. [Défaut : auto]
     centeredSlides (1) : [Binaire] - 	1ère tuile centrée au widget. [Défaut : 1 = centrer]
     rotate (1) : [Numérique] - 	Effet de rotaion de la tuile. [Défaut : 10]
	 depth (1) : [Numérique] - 	Effet de profondeur du widget. [Défaut : 200]
	 paginationType : [Numérique 0 à 5] - 	Type de pagination. [Défaut : 1 -> Bullets, 0 -> masquée, 2 -> dynamicBullets, 3 -> progressbar, 4 -> fraction]
	 swiperButton : [Binaire] - 	Masque les flêches de navigation  [Défaut : 1 -> afficher]
	 (2) disponible uniquement pour "effect" = 0, 1 et 2
	 freeMode (2) : [Binaire] - 	Effet d'inertie lors d'un swippe. [Défaut : 0 -> désactiver]
	 grabCursor : [Binaire] - 	Curseur "grab" sur les tuiles. [Défaut : 1 -> activer]
	 (3) Attention lorsque cette option est activée, il n'est plus possible de redimensionner la tuile sur le dashboard.
	 backgroundColor : Couleur de fond de la tuile. [Défaut : white]
	 loop (3) : [Binaire] - 	Boucle sur le widget [Défaut : 0 -> désactiver]
	  
- Exemple de paramètres optionnels :

![](doc/images/installation_virtuel4.png)


# Change Log

     
     /!\ Attention, n'oubliez pas de reconfigurer le paramètre "$zone" dans le bloc code, si vous mettez a jour le scénario, car celui-ci sera reconfiguré en zone B par défaut.
     

- 05/12/2021 : Création.
- 23/01/2022 : [scénario] Remplacement de la fonction sun_pos(), qui générait des erreurs dans le log "scenario_execution"
par [getSunPosition()](https://github.com/KiboOst/php-sunPos/blob/master/phpSunPos.php) qui est de plus, plus précise.
- 21/02/2022 : [scénario] Bugfix sur la date du dernier jour de vacances.
Rajout des dates de vacances jusqu'au 2023/09/01
- 20/06/2022 : [widget] 
  - Ajout de paramètres optionnels. [Demande](https://community.jeedom.com/t/widget-perso-info-du-jour/86118)
  - Modification de la taille du widget par défaut.
- 20/06/2022 : [widget]
  - Bugfix lorsque l'option "Centrage vertical des tuiles" est cochées dans l'interface Jeedom. (Merci @jpty)
- 21/06/2022 : [widget]
  - Ajouts / Modification des paramètres optionnels.
- 18/09/2022 :
  - Ajout des dates de vacances jusqu'au 2023/09/01. [scénario]
  - Modification de l'affichage : St -> Saint et Ste -> Sainte. [scénario]
  - Affichage de tous les tag disponibles, dans le log. [scénario]
  - mise a dispo du tag « dureeJourEcart » en secondes. [scénario]
  - Restructuration du code, il est possible de désactiver chaque catégorie (vacances, saint, soleil, widget ...) individuellement. [scénario]
  - Affichage de la durée du jour (par paramètre optionnel) entre lever et coucher du soleil. [widget]
 - 09/03/2023 :
  - Restructuration du code, compatibité Core V4.2 V4.3 V4.4
  - Ajout des dates de vacances jusqu'au 2026/09/01. [scénario]
  - Ajout de l'écart de durée du jour avec la veille. [widget]
  - Ajout de tag (aubeCivil, crepusculeCivil, aubeNautique, crepusculeNautique, aubeAstronomique, crepusculeAstronomique) Thanks @prfalken.  [scénario]
  - En mode themeJeedom, le widget change de thème lors de l'évènement du core, plus besoin d'attendre le lancement du scénario. [widget]

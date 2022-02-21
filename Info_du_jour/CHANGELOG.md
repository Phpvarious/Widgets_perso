# Change Log

     
     /!\ Attention, n'oubliez pas de reconfigurer le paramètre "$zone" dans le bloc code, si vous mettez a jour le scénario, car celui-ci sera reconfiguré en zone B par défaut.
     

- 05/12/2021 : Création.
- 23/01/2022 : [scénario] Remplacement de la fonction sun_pos(), qui générait des erreurs dans le log "scenario_execution"
par [getSunPosition()](https://github.com/KiboOst/php-sunPos/blob/master/phpSunPos.php) qui est de plus, plus précise.
- 21/02/2022 : [scénario] Bugfix sur la date du dernier jour de vacances.
Rajout des dates de vacances jusqu'au 2023/09/01
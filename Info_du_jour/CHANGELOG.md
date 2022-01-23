# Change Log
- 05/12/2021 : Création.
- 23/01/2022 : [scénario] Remplacement de la fonction sun_pos(), qui générait des erreurs dans le log "scenario_execution"
par [getSunPosition()](https://github.com/KiboOst/php-sunPos/blob/master/phpSunPos.php) qui est de plus, plus précise.


    /!\ Attention, n'oubliez pas de reconfigurer le paramètre "$zone" dans le bloc code, si vous mettez a jour le scénario, car celui-ci sera reconfigurer en zone B.
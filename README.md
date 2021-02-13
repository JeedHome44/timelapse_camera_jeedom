# timelapse_camera_jeedom
Explication des scénarios pour réussir à faire des timelapse avec les caméras sur Jeedom

- Choisir entre l'une des 3 étapes 0 selon votre caméra pour le scénario d'enregistrement (1 scénario par caméra)
- Faire ensuite les étapes 1, 2, 3, 4 pour toutes vos caméras. Il faudra donc faire un seul scénario pour chaque étape avec autant de bloc Code que de caméras.
- Si vous avez un serveur NAS sur lequel vous voulez mettre les vidéos, 2 choix s'offre à vous:
    - Faire juste une synchronisation basique via la bloc code 5.1 pour chaque caméra.
    - Faire une copie de chaque vidéo sur le NAS et les organiser par dossier par jour en suivant les étapes 5.2, 6, 7 et 8.
    
Pour enchainer les différents scénario, mettre l'étape 1 avec un déclenchement chaque heure à XX:00.
A la fin de l'étape 1 lancer l'étape 2 quand la 1 est fini et ainsi de suite.
Pour l'étape 4 ou/et 8, lancez les chaque jour à 00:30 par exemple.
    
Pensez à bien remplacer dans les blocs code:
- IP_FIXE_JEEDOM
- NOM_CAMERA
- USER_SSH
- PASSWORD_SSH
- NUM_DOSSIER_CAMERA

Edit: il n'y a pas besoin de connexion SSH lorsqu'on exécute les blocs pour la machine local, j'ai donc modifié les blocs pour supprimer le SSH

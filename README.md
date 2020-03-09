# timelapse_camera_jeedom
Explication des scénarios pour réussir à faire des timelapse avec les caméras sur Jeedom

- Choisir entre l'une des 3 étapes 0 selon votre caméra pour le scénario d'enregistrement.
- Faire ensuite les étapes 1, 2, 3, 4 pour toutes vos caméras. Il faudra donc faire un seul scénario pour l'étape 1 avec autant de bloc Code que de caméras.
- Si vous avez un serveur NAS sur lequel vous voulez mettre les vidéos, 2 choix s'offre à vous:
    - Faire juste une synchronisation basique via la bloc code 5.1 pour chaque caméra.
    - Faire une copie de chaque vidéo sur le NAS en suivant les étapes 5.2, 6, 7 et 8.
    
Pensez à bien remplacer des les blocs code:
- IP_FIXE_JEEDOM
- NOM_CAMERA
- USER_SSH
- PASSWORD_SSH
- NUM_DOSSIER_CAMERA

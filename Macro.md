![image](https://github.com/Eloura74/Sauvegarde_Config/blob/main/Image/Installation.webp)

## Étape 4 : Ajout de la Macro dans klipper:

1. Aller dans votre printer.cfg, ou alors là ou vous mettez vos macros:
2. Ajouter celles-ci:

```
 [gcode_shell_command backup_cfg]
 command: /usr/bin/bash /home/pi/printer_data/config/autocommit.sh
 timeout: 30
 verbose: True

 [gcode_macro BACKUP_CFG]
 description: Backs up config directory GitHub
 gcode:
     RUN_SHELL_COMMAND CMD=backup_cfg
```
3. Mettez a jours commande shell avec ceci:

```
 wget -O /home/pi/klipper/klippy/extras/gcode_shell_command.py https://raw.githubusercontent.com/th33xitus/kiauh/master/resources/gcode_shell_command.py
```

Ou alors avec Kiauh en allant dans:
<br>
Option (4)
<br>


Félicitations ! Vous avez maintenant sauvegardé votre configuration Klipper sur GitHub. Vous pouvez accéder à cette sauvegarde à tout moment à partir de n'importe quel appareil connecté à Internet et la partager avec d'autres personnes si vous le souhaitez.

N'hésitez pas à consulter la documentation de Klipper et de Git pour en savoir plus sur les fonctionnalités avancées et les bonnes pratiques de gestion de version. Amusez-vous bien avec Klipper et l'impression 3D !

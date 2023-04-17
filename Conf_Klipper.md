![image](https://github.com/Eloura74/Sauvegarde_Config/blob/main/Image/Installation.webp)

## Étape 3 : Ajout et sauvegarde de la configuration Klipper

1. Connecter vous en SSH à votre Raspberry.
2. Modifiez les répertoires dans votre configrépertoire, où se trouvent tous vos fichiers de configuration, pour ma part:

```
cd ~/printer_data/config
```

3. Téléchargez le autocommit.shfichier à l'aide de la commande ci-dessous : :

```
 wget -O /home/pi/printer_data/config/autocommit.sh https://raw.githubusercontent.com/EricZimmerman/VoronTools/main/autocommit.sh
```
4. Modifiez le fichier pour votre cas d'utilisation particulier à l'aide de la commande ci-dessous. 
<br>
Par exemple, si vous utilisez Mainsail, commentez la **fluidd_folderligne** avec # , et decommentez **mainsail_folderet** en enlevant le #.

```
 nano /home/pi/printer_data/config/autocommit.sh
```

5. Enregistrez le fichier. Si vous utilisez nano, appuyez sur Ctrl-o (o, pas zéro).
 <br>
 Vérifiez le nom du fichier qui doit être **autocomiit.sh** en bas à gauche et appuyez sur **Entrer**
 
6. Quittez l'éditeur nano avec **"Ctrl + X"**

7. Nous devons modifier les autorisations sur le fichier afin qu'il puisse être exécuté facilement. 
 <br>
 Tapez la commande suivante:
 
```
chmod +x autocommit.sh
```

8. Vérifions que cela à fonctionné:
 
```
ls -la autocommit.sh
```




On va simplement accéder à la vérification de la sauvegarde sur [GitHub](https://github.com/Eloura74/Sauvegarde_Config/blob/main/V%C3%A9rification.md). 

![image](https://github.com/Eloura74/Sauvegarde_Config/blob/main/Image/Installation.webp)

## Étape 2 : Clonage du dépôt GitHub

1. Copiez l'URL du dépôt GitHub que vous venez de créer.

![image](https://github.com/Eloura74/Sauvegarde_Config/blob/main/Image/Parie2.png)

2. Ouvrez un terminal sur votre ordinateur et utilisez la commande pour cloner le dépôt GitHub localement sur votre Raspberry :


```
git clone <URL_DU_DEPOT_GITHUB>
```

3. Nous allons générer un jeton d'accès:
<br> <br>
Acceder à ["Personnal Acces Tokens"](https://github.com/settings/tokens).
<br> <br>
Sur le côté gauche, assurez vous que vous avez sélectionné "Token Classic".
<br> <br>
Aller ensuite dans "Generate new token" et sélectionner l'option "Classic".
<br> <br>
Il vous sera peut être demander de vous identifier par mesure de sécurité.
<br> <br>
Dans "Note" vous allez donner un nom a votre jeton d'acceès.
<br> <br>
Et dans "Expiration" sélectionner bien "No expiration".
<br> <br>
Cocher les option suivante:
<br> <br>
-repo (d'origine cocher)
<br> <br>
-workflow
<br> <br>
-read:org
<br> <br>
Tout en bas vous pouvez cliquer sur "Generate Token".
<br> <br>
Attention la clé générée sera unique, et c'est votre chance de la voir, vous devez bien la conservée.
<br> <br> <br>

4. Naviguez dans le répertoire du dépôt local en utilisant la commande :

```
cd <NOM_DU_DEPOT_LOCAL>
```

Passons ensuite à la configuration de [Klipper](https://github.com/Eloura74/Sauvegarde_Config/blob/main/Conf_Klipper.md)

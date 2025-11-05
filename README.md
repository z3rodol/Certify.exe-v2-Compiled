Compilation de Certify v2
1. Téléchargement et extraction
- Télécharge [Visual Studio Community 2022](https://visualstudio.microsoft.com/fr/vs/)
- Télécharge le dépôt au format ZIP depuis [GhostPack/Certify](https://github.com/GhostPack/Certify) et extrais-le dans un répertoire de ton choix.

2. Préparation de l’environnement

- Place toi dans le répertoire `Certify-main\Certify-main\`
- Clique droit sur le fichier `Certify.sln` et ouvre le avec **Visual Studio Community 2022**
- Ouvre un terminal en cliquant en haut sur la barre de navigation Affichage -> Terminal

3. Restauration des dépendances

- Restaure les packages NuGet via la CLI .NET :

```dotnet restore Certify.sln```

Cette commande télécharge automatiquement toutes les dépendances nécessaires.

4. Compilation du projet

- Compile le projet en mode Release pour toutes les plateformes :
  
```msbuild Certify.sln /p:Configuration=Release /p:Platform="Any CPU"```


5. Récupération de l’exécutable

- Une fois la compilation terminée, l’exécutable Certify.exe sera disponible dans :
  
```Certify-main\Certify-main\Certify\bin\Release\```



Remarques

Assure-toi d’avoir .NET SDK et MSBuild installés sur ta machine.
Si tu utilises Visual Studio 2022, tu peux aussi ouvrir le fichier .sln et compiler directement depuis l’IDE (menu Build > Build Solution).

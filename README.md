Programmation Java @ Et3
<br>
Polytech Paris-Saclay | 2045-25

___

# Configuration d'un IDE pour le TP1

Instructions pour configurer IntelliJ ou VSCode pour programmer avec JavaFX.

-------

## Configuration d'IntelliJ

### A. Téléchargement du projet.
1. Faites *New* -> *Project from version control*.

2. Renseignez 
- *URL* : l'adresse de ce repo git : https://github.com/kunchtler/TP1-squelette
- *Directory* : le répertoire où se situera le projet sur votre machine.

3. Faites *Clone*.

### B. Configuration / Installation de la version de Java à utiliser.
1. Allez dans *File* -> *Project Structure*.

2. Renseignez :
- *SDK* avec une version de Java (au moins 17, au plus 21) qui est sur votre machine.
    Si aucune version de Java ne vous est proposé, faites *Download JDK*, sélectionnez comme *Version* 21, puis faites *Download*.  

3. Faites *Apply*, puis *OK*.

### C. Configuration de l'outil de compilation Maven.

1. Identifiez un fichier appelé "pom.xml" et faites clic droit dessus, et faites dans *Maven* -> *Reload project*.

2. Cliquez sur *Current File* en haut de l'écran, et faites *Edit configurations*.

3. Cliquez sur *Add new run configuration...* -> *Application*.

4. Il y a un encadré rouge où est écrit *Main class*. Cliquez sur l'icône à droite de cet encadré, puis faites *OK*.

5. Faites *OK*.

### D. Execution du projet.

Félicitations, vous devriez avoir mis en place IntelliJ pour utiliser ce projet.

Essayez de cliquer sur l'icône Play en haut de l'écran pour vérifier qu'une fenêtre (vide) s'affiche bien.

----------------------

## Configuration de VSCode

### A. Téléchargement du projet.

Procurez vous le repo git à cet adresse : https://github.com/kunchtler/TP1-squelette
- ou bien en utilisant git si vous savez faire.
- ou bien en cliquant sur l'onglet vert *<> Code*, puis en faisant *Download ZIP*. Décompressez l'archive obtenue sur votre machine.

### B. Installation de l'outil de compilation Maven (à ne faire qu'une fois).
- Sous Windows
    
    (Suivre ceci : https://maven.apache.org/install.html)
    
    En résumé : 

    1. Téléchargez l'archive "apache-maven-3.9.9-bin.zip" disponible [ici](https://maven.apache.org/download.cgi). 

    2. Extrayez l'archive au bon endroit et ajoutez le chemin d'accès (typiquement `C:\Users\Username\...\apache-maven-3.9.9\bin`) dans la variable d'environement 'Path' (Menu Windows: 'Modifier les variables d'environnement système'>'Variables d'environnement'>'Path'>'Ajouter...').

    3. Fermez et rouvrez VSCode. Vérifier l'installation dans le terminal avec la commande : 
    ``` 
    mvn -v
    ```

- Sous Linux

    1. Vous pouvez installer Maven via le gestionnaire de paquets de votre distribution Linux. Par exemple, en faisant dans le terminal :
    ```
    sudo apt install maven
    ```

    2. Fermez et rouvrez VSCode. Vérifier l'installation dans le terminal avec la commande : 
    ``` 
    mvn -v
    ```

### C. Configuration de VSCode.

1. (A ne faire qu'une fois) Dans VSCode, installez et activez la suite de plugins dédiée à Java : [Extension pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack).
Vous pouvez l'installer en cliquant sur l'icône avec 4 carrés dans la barre de gauche, et en tapant dans le champ de recherche des extensions : *Extension pack for Java*.

2. Ouvrez le projet en faisant *File* -> *Open Folder* et en choisissant le dossier où vous avez décompressé le TP.

3. Cliquez sur l'icône d'engrenage en bas à gauche de l'écran, et faites *Command Palette*. Tapez et sélectionnez "Java: Configure Java Runtime".

4. Il vous faut choisir dans JDK une version de Java (au moins 17, au plus 21). Si aucune version de Java n'est listée:
    - Faites *Download a new JDK*
    - Choisissez la version 21, et faites *Download*. Une fenêtre de navigateur devrait s'ouvrir.
    - Une fois el téléchargement terminé, décompressez l'archive quelque part sur votre machine.
    - Revenez à la fenêtre de VSCode où choisir le SDK Java. Faites *Find a new local JDK*, et choisissez le chemin vers le dossier précédemment téléchargé.

5. Faites *Apply Settings*.

### D. Execution du projet.

Félicitations, vous devriez avoir mis en place IntelliJ pour utiliser ce projet.

Essayez d'appuyer sur la touche F5 pour vérifier qu'une fenêtre (vide) s'affiche bien.
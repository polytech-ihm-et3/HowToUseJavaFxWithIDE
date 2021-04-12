Programmation Java @ Et3
<br>
Polytech Paris-Saclay | 2020-21

___

Voici un petit tutoriel pour utiliser JavaFX avec Eclipse ou IntelliJ. Je précise qu'ici, l'ordinateur est configuré en anglais, donc bien évidemment, les commandes seront peut-être en français pour certains d'entre vous.

# Comment utiliser JavaFX sous Eclipse ?

1. **Installation du Plugin *e(fx)clipse* :**

1.1. Connectez-vous au [MarketPlace de Eclipse](https://marketplace.eclipse.org/) et chercher *e(fx)clipse*.

> <br><div align="center"><img src="images/eclipse_step1.1.jpg"></img></div><br>
>
> <br><div align="center"><img src="images/eclipse_step1.2.jpg"></img></div><br>

1.2. Pour intégrer ce plugin à Eclipse, il faut glisser et déposer le bouton *Install* dans Eclipse.

> <br><div align="center"><img src="images/eclipse_step1.3.jpg"></img></div><br>
> 
> <br><div align="center"><img src="images/eclipse_step1.4.jpg"></img></div><br>

1.3. Une fenêtre de confirmation apparaîtra alors. Veillez à sélectionner *e(fx)clipse* et confirmez.

> <br><div align="center"><img src="images/eclipse_step1.5.jpg"></img></div><br>

1.4. Patientez pendant l'installation.

> <br><div align="center"><img src="images/eclipse_step1.6.jpg"></img></div><br>

1.5. Une fois l'installation terminez, acceptez les conditions d'utilisations.

> <br><div align="center"><img src="images/eclipse_step1.7.jpg"></img></div><br>
> <br><div align="center"><img src="images/eclipse_step1.8.jpg"></img></div><br>

1.6. Finalement, redémarrez Eclipse.

> <br><div align="center"><img src="images/eclipse_step1.9.jpg"></img></div><br>

2. **Changement de plateforme :**

2.1. Allez dans les préférences d'Eclipse (*Window* > *Preferences*).

> <br><div align="center"><img src="images/eclipse_step2.1.jpg"></img></div><br>

2.2. Sélectionnez *Plug-in Development* > *Target Platform* et ciquez sur *Add ...* pour en ajouter une nouvelle.

> <br><div align="center"><img src="images/eclipse_step2.2.jpg"></img></div><br>

2.3. Sélectionnez "Nothing: start with an empty target definition" et validez en cliquant sur *Next >*.

> <br><div align="center"><img src="images/eclipse_step2.3.jpg"></img></div><br>

2.4. Dans *name*, indiquez "e(fx)clipse" et cliquez sur *Add ...*.

> <br><div align="center"><img src="images/eclipse_step2.4.jpg"></img></div><br>

2.5. Sélectionnez "Software Site" et cliquez sur *Next >*.

> <br><div align="center"><img src="images/eclipse_step2.5.jpg"></img></div><br>

2.6. Dans *Work with:* entrez "[http://download.eclipse.org/efxclipse/runtime-released/2.0.0/site](http://download.eclipse.org/efxclipse/runtime-released/2.0.0/site)". Cochez *Target Platform Features*. Plus bas, décochez *Include required software* et validez en cliquant sur *Finish*.

> <br><div align="center"><img src="images/eclipse_step2.6.jpg"></img></div><br>

2.7. Patientez pendant l'installation.

> <br><div align="center"><img src="images/eclipse_step2.7.jpg"></img></div><br>

2.8. Cliquez sur *Finish*.

> <br><div align="center"><img src="images/eclipse_step2.8.jpg"></img></div><br>

2.9. Vérifiez que la nouvelle plateforme "e(fx)clipse" est bien sélectionnée et cliquez sur *Apply and Close*.

> <br><div align="center"><img src="images/eclipse_step2.9.jpg"></img></div><br>

3. **Installation d'un JRE (Java Runtime Environment) approprié :**

3.1. Rendez-vous sur le site d'[Oracle pour télécharger une version récente du JRE 8](https://www.oracle.com/fr/java/technologies/javase-jre8-downloads.html). Choisissez la version qui convient pour votre ordinateur.

> <br><div align="center"><img src="images/eclipse_step3.1.jpg"></img></div><br>

3.2. Acceptez les conditions d'utilisation et validez votre téléchargement (il est possible que cette étape vous demande de vous connecter à un compte Oracle, si vous n'en avez pas, créez-en un).

> <br><div align="center"><img src="images/eclipse_step3.2.jpg"></img></div><br>

3.3. Lancez l'installation du JRE.

> <br><div align="center"><img src="images/eclipse_step3.3.jpg"></img></div><br>

3.4. Patientez pendant l'installation.

> <br><div align="center"><img src="images/eclipse_step3.4.jpg"></img></div><br>

3.5. Fermez la fenêtre.

> <br><div align="center"><img src="images/eclipse_step3.5.jpg"></img></div><br>

4. **Enregistrement d'un nouveau JRE dans Eclipse :**

4.1. Retournez dans les préférences de Eclipse (*Window* > *Preferences*).

> <br><div align="center"><img src="images/eclipse_step4.1.jpg"></img></div><br>

4.2. Allez dans *Installed JREs* et cliquez sur *Add ...*.

> <br><div align="center"><img src="images/eclipse_step4.2.jpg"></img></div><br>

4.3. Sélectionnez *Standard VM* et cliquez sur *Next >*.

> <br><div align="center"><img src="images/eclipse_step4.3.jpg"></img></div><br>

4.4. Dans *JRE home:*, entrez le chemin vers le répertoire d'installation de votre JRE, puis cliquez sur *Finish*.

> <br><div align="center"><img src="images/eclipse_step4.4.jpg"></img></div><br>

4.5. Cliquez sur *Apply and Close*.

> <br><div align="center"><img src="images/eclipse_step4.5.jpg"></img></div><br>

5. **Création d'un nouveau projet avec JavaFx :**

5.1. Démarrez un nouveau projet (*File* > *New* > *Project...*).

> <br><div align="center"><img src="images/eclipse_step5.1.jpg"></img></div><br>

5.2. Sélectionnez *JavaFX*, puis *JavaFX Project* et cliquez sur *Next >*.

> <br><div align="center"><img src="images/eclipse_step5.2.jpg"></img></div><br>

5.3. Choisissez un nom pour votre projet. Cochez *Use a project specific JRE* puis selectionnez la version de JRE récemment installée. Finalement, cliquez sur *Finish*.

> <br><div align="center"><img src="images/eclipse_step5.3.jpg"></img></div><br>

5.4. Votre projet JavaFX devrait fonctionner correctement, sans erreurs :trophy: :trophy: :trophy:

> <br><div align="center"><img src="images/eclipse_step5.4.jpg"></img></div><br>

# Comment utiliser JavaFX sous IntelliJ ?

1. Vérifier 

1.1. Allez dans les paramètres de IntelliJ (*File* > *Settings...*).

> <br><div align="center"><img src="images/intellij_step1.1.jpg"></img></div><br>

1.2. Sélectionnez *Plugin* et vérifiez que *JavaFX* est bien coché dans les plugins installés. Si oui, fermez la fenêtre et passez à l'étape suivante, sinon, cochez la case correspondante et redémmarez IntelliJ.

> <br><div align="center"><img src="images/intellij_step1.2.jpg"></img></div><br>

2. **Installer un JDK approprié et démarrer un nouveau projet :**

2.1. Commencez un nouveau projet (*File* > *New* > *Projet...*).

> <br><div align="center"><img src="images/intellij_step2.1.jpg"></img></div><br>

2.2. Sélectionnez *javaFX* sur la gauche. Dans *Project SDK:* Sélectionnez "Download JDK..."

> <br><div align="center"><img src="images/intellij_step2.2.jpg"></img></div><br>

2.3. Une nouvelle fenêtre s'affiche. Choisissez la version "1.8", sélectionnez un vendeur et cliquez sur *Download*.

> <br><div align="center"><img src="images/intellij_step2.3.jpg"></img></div><br>

2.4. Patientez le temps de l'installation. Vous pouvez la suivre en bas à droite de la fenêtre d'IntelliJ.

> <br><div align="center"><img src="images/intellij_step2.4.jpg"></img></div><br>

2.5. Quand l'installation est terminée, cliquez sur *Next*.

> <br><div align="center"><img src="images/intellij_step2.5.jpg"></img></div><br>

2.6. Nommez votre nouveau projet et cliquez sur *Finish*.

> <br><div align="center"><img src="images/intellij_step2.6.jpg"></img></div><br>

2.7. Votre projet JavaFX devrait fonctionner correctement, sans erreurs :trophy: :trophy: :trophy: (Quand vous créerez un nouveau projet, vous pourrez simplement sélectionner le JDK 1.8 déjà installé)

> <br><div align="center"><img src="images/intellij_step2.7.jpg"></img></div><br>

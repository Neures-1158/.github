# Guide GitHub NEURES
> **Note :** Nous  travaillons initialement sur des dépôts privés. Toutes les contributions, développements et partages doivent se faire dans des repositories privés afin de garantir la confidentialité des projets.

Ce document décrit les règles internes pour l’utilisation de GitHub dans le groupe.

## Avant de commencer

- **Avoir un compte GitHub personnel** et être ajouté au groupe NEURES.  
  Les adresses `@sorbonne-universite.fr` sont éligibles à GitHub Pro via [GitHub Education](https://education.github.com/discount_requests/student_application).
  Cela donne accès gratuitement à GitHub Copilot (assistant IA de programmation) et à de nombreuses ressources premium (actions, codespaces, outils avancés, etc.) utiles pour le développement et la collaboration.
- **Installer un outil Git** :
  - option simple : [GitHub Desktop](https://desktop.github.com) (interface graphique) ;
  - option avancée : [Git en ligne de commande](https://git-scm.com/downloads) (`git`) + éditeur (VS Code, RStudio, etc.) 


## Vocabulaire rapide

- **Git** : l’outil qui versionne les fichiers (fonctionne sur votre ordinateur).
- **GitHub** : la plateforme en ligne où l’on partage les dépôts Git et collabore.
- **Dépôt (repository, repo)** : dossier d’un projet suivi par Git.
- **Commit** : enregistrement d’un ensemble de modifications avec un message.
- **Branche** : ligne de travail parallèle pour isoler vos modifications.
- **Pull Request (PR)** : demande de relecture et de fusion de votre branche vers `main`.

## Organisation du travail avec GitHub

### La branche principale : `main`
- **C’est quoi ?**  
  La branche `main` contient la version la plus à jour et stable du travail du groupe.
- **Important :**  
  _On ne modifie jamais directement `main`._ Cela évite les erreurs et protège le travail de tout le monde.

### Créer sa propre branche pour travailler
- **Comment faire ?**  
  Chaque membre crée une branche à son nom pour travailler sur un sujet précis.
- **Format recommandé :**  
  `prenom-sujet`  
  Par exemple :  
  - `alice-preparation-donnees`  
  - `charles-figures-these`
- **Pourquoi ?**  
  Cela permet de séparer les travaux et d’éviter les conflits entre les modifications de chacun.

### Les étapes pour contribuer

1. **Créer une branche** (voir ci-dessus)
2. **Faire ses modifications** (ajouter ou modifier des fichiers)
3. **Enregistrer ses changements** (“commits” – voir plus bas)
4. **Push régulier de votre branche pour sauvegarder votre travail en distant**  
   _Pensez à synchroniser fréquemment votre branche sur GitHub pour ne pas perdre vos modifications en cas de problème local._
5. **Toujours tester localement avant PR**  
   _Assurez-vous que tout fonctionne sur votre ordinateur avant de proposer vos changements._
6. **Ouvrir une Pull Request (PR)**  
   _Une PR sert à proposer que vos modifications soient ajoutées à la branche `main`._
7. **Faire relire sa PR**  
   _Au moins une autre personne doit lire et approuver avant que les changements soient acceptés._
8. **Fusionner la PR**  
   _Après validation, vos modifications seront ajoutées à `main`._

### Workflow

**Interface web GitHub**  
1. Mettre `main` à jour : bouton `Update branch` (si besoin) pour synchroniser avec la version la plus récente du dépôt.  
  _NB : Nous ne travaillons pas avec des forks, mais uniquement avec des branches sur un dépôt privé du groupe sauf cas spécifiques._
2. Créer une branche : bouton `Branch: main` → `Find or create a branch` → nommer `prenom-sujet`.  
3. Modifier, créer un/des fichiers
4. Enregistrer l’étape : remplir le message de commit et cliquer sur `Commit changes`.  
5. Ouvrir la Pull Request : bannière « Compare & pull request » → compléter la description et `Create pull request`.  
_Pour aller plus loin : [Travailler avec des fichiers sur GitHub.com](https://docs.github.com/fr/repositories/working-with-files/managing-files/editing-files)._ 

**GitHub Desktop**  
1. Mettre `main` à jour : `Fetch origin` puis `Pull`.  
2. Créer une branche : `Current Branch` → `New Branch` → nommer `prenom-sujet`.  
3. Sauvegarder une étape : vérifier les fichiers dans `Changes`, écrire un message clair puis `Commit to prenom-sujet`.  
4. Envoyer sur GitHub : bouton `Push origin`.  
5. Ouvrir la Pull Request : bouton `Create pull request` sur GitHub.com.  
_Pour aller plus loin : [Guide officiel GitHub Desktop](https://docs.github.com/fr/desktop/overview/getting-started-with-github-desktop)._ 

**Visual Studio Code (Source Control)**  
1. Mettre `main` à jour : onglet `Source Control` → menu `…` → `Pull`.  
2. Créer une branche : cliquer sur le nom de branche (barre de statut) → `Create new branch` → nommer `prenom-sujet`.  
3. Sauvegarder une étape : sélectionner les fichiers (`+`), écrire le message dans `Message` puis `Commit`.  
4. Envoyer sur GitHub : menu `…` → `Push` (la première fois, choisir `Publish Branch`).  
5. Ouvrir la Pull Request : lien proposé dans la notification ou sur GitHub.com.  
_Pour aller plus loin : [VS Code & GitHub Guide](https://code.visualstudio.com/docs/sourcecontrol/github)._ 

**Commandes avancées**  
Si vous souhaitez apprendre la ligne de commande Git (`git pull`, `git rebase`, etc.), appuyez-vous sur la [documentation officielle Git](https://git-scm.com/doc) ou le [guide GitHub pour Git en terminal](https://docs.github.com/fr/get-started/using-git/about-git).

---

## Écrire des messages de commit clairs

- Un **commit** enregistre une étape de votre travail.
- **Le message doit être court et précis.**
- **Exemples :**
  - `fix(donnees): corrige valeurs manquantes`
  - `feat(figure): ajoute graphique vitesse`
- **Astuce :**  
  Utilisez le format `type(sujet): description`  
  - `fix` = correction de bug  
  - `feat` = nouvelle fonctionnalité  
  - `docs` = documentation  
  - _etc..._
- **Comment faire concrètement ?**
  1. Vérifiez les fichiers modifiés : `git status`.
  2. Sélectionnez ce que vous voulez enregistrer : `git add chemin/vers/fichier` (ou via GitHub Desktop → `Changes` → cocher les fichiers).
  3. Contrôlez une dernière fois : `git status` doit afficher « changes to be committed ».
  4. Écrivez un message clair puis validez : `git commit -m "docs: clarifie workflow"`.
  5. Répétez dès que vous terminez une idée (petits commits = relectures plus simples).

---

## Gestion et stockage des données

- **Ne pas ajouter de données patient ni sensibles dans GitHub**  
  _Aucune donnée identifiable ou confidentielle ne doit être déposée sur GitHub, même temporairement._
- **Les données (“data”) sont stockées localement et sur le NAS**  
  Chaque membre garde les données sur son ordinateur et une copie complète est sauvegardée sur le NAS du laboratoire.
- **Le dossier `data` est dans le `.gitignore`**  
  Cela signifie que Git ignore ce dossier : il n’est pas suivi ni synchronisé sur GitHub.  
  _C’est pour éviter de partager accidentellement des fichiers volumineux ou sensibles._
- **C’est aussi le cas pour d’autres fichiers lourds**  
  Par exemple, le dossier `output` (sorties d’analyse, images brutes, etc.) doit aussi être dans le `.gitignore`.
- **Seuls les petits fichiers de résultats pour les statistiques peuvent être partagés**  
  Si un fichier de résultats est léger (par exemple dans le dossier `results`), il peut être suivi par Git et partagé dans le dépôt.
- **Voir le template de dépôt pour plus de détails**  
  _Consultez le [modèle de dépôt NEURES](https://github.com/Neures-1158/Neures_template)._

---

## Quelques conseils pratiques

- **Demandez de l’aide si besoin !**  
  Personne n’attend de vous que vous sachiez tout : demandez à un membre plus expérimenté.
- **Gardez votre branche à jour**  
  Avant d’ouvrir une PR, pensez à synchroniser votre branche avec `main` pour éviter les conflits.
- **Pas de panique en cas de conflit**  
  Cela arrive à tout le monde. N’hésitez pas à demander de l’aide pour les résoudre.
- **Gardez une trace de vos questions**  
  Notez ce qui vous a bloqué et enrichissez la FAQ interne pour aider les suivants.

### Checklist avant d’ouvrir une PR

- `main` est à jour sur votre ordinateur (`git pull origin main`).
- Votre branche est à jour avec `main` (`git merge main` ou `git rebase main`).
- Vous avez relu vos fichiers modifiés (`git diff` ou aperçu GitHub Desktop).
- Les instructions/tests locaux s’exécutent correctement.
- La description de la PR explique le contexte, la méthode et comment vérifier.

### Faire relire efficacement

- Donnez le contexte dans la PR : _Pourquoi ce changement ? Comment vérifier ?_
- Mentionnez les reviewers concernés (`@prenom`).
- Restez disponible pour répondre et ajuster rapidement.
- Quand tout est approuvé, fusionnez via le bouton `Merge` (pas de `git merge` local sur `main`).

---

## Ressources

- https://docs.github.com/fr

---

## Rappel des règles principales

- **Jamais de modification directe sur `main`**
- **Travailler toujours avec des chemins relatifs sans quoi votre code ne sera pas transportable**
- **Toujours passer par une branche personnelle**
- **Toujours ouvrir une Pull Request pour proposer ses changements**
- **Toujours demander au moins une relecture avant de fusionner**
- **Toujours tester localement avant PR**
- **Push régulier de votre branche pour sauvegarder votre travail**
- **Ne jamais ajouter de données patient ni sensibles dans GitHub**

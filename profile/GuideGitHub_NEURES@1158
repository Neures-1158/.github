# Guide GitHub NEURES@1158

Ce document décrit les règles internes pour l’utilisation de GitHub dans le groupe.

## 1. Organisation du travail avec GitHub

### a. La branche principale : `main`
- **C’est quoi ?**  
  La branche `main` contient la version la plus à jour et stable du travail du groupe.
- **Important :**  
  _On ne modifie jamais directement `main`._ Cela évite les erreurs et protège le travail de tout le monde.

### b. Créer sa propre branche pour travailler
- **Comment faire ?**  
  Chaque membre crée une branche à son nom pour travailler sur un sujet précis.
- **Format recommandé :**  
  `prenom-sujet`  
  Par exemple :  
  - `alice-preparation-donnees`  
  - `charles-figures-these`
- **Pourquoi ?**  
  Cela permet de séparer les travaux et d’éviter les conflits entre les modifications de chacun.

### c. Les étapes pour contribuer

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

---

## 2. Écrire des messages de commit clairs

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

---

## 3. Gestion et stockage des données

- **Ne pas ajouter de données patient ni sensibles dans GitHub**  
  _Aucune donnée identifiable ou confidentielle ne doit être déposée sur GitHub, même temporairement._
- **Les données (“data”) sont stockées localement et sur le NAS**  
  Chaque membre garde les données sur son ordinateur et une copie complète est sauvegardée sur le NAS du laboratoire.
- **Le dossier `data` est dans le `.gitignore`**  
  Cela signifie que Git ignore ce dossier : il n’est pas suivi ni synchronisé sur GitHub.  
  _C’est pour éviter de partager accidentellement des fichiers volumineux ou sensibles._
- **C’est aussi le cas pour d’autres fichiers lourds**  
  Par exemple, le dossier `output` (sorties d’analyse, images brutes, etc.) doit aussi être dans le `.gitignore`.
- **Seuls les petits fichiers de résultats statistiques peuvent être partagés**  
  Si un fichier de résultats est léger (par exemple dans le dossier `results`), il peut être suivi par Git et partagé dans le dépôt.
- **Voir le template de dépôt pour plus de détails**  
  _Consultez le modèle de dépôt NEURES pour la structure recommandée et les liens utiles._

---

## 4. Quelques conseils pratiques

- **Demandez de l’aide si besoin !**  
  Personne n’attend de vous que vous sachiez tout : demandez à un membre plus expérimenté.
- **Gardez votre branche à jour**  
  Avant d’ouvrir une PR, pensez à synchroniser votre branche avec `main` pour éviter les conflits.
- **Pas de panique en cas de conflit**  
  Cela arrive à tout le monde. N’hésitez pas à demander de l’aide pour les résoudre.

---

## 5. Ressources utiles pour débuter

- [Introduction à Git et GitHub (français)](https://www.pentalog.fr/blog/formation-git-github/)
- [Guide officiel GitHub pour les débutants (anglais)](https://docs.github.com/en/get-started/quickstart)
- [Glossaire GitHub](https://docs.github.com/fr/get-started/quickstart/github-glossary)
- [Template NEURES pour dépôt GitHub](lien_vers_le_template) <!-- À remplacer par le lien réel -->

---

## 6. Rappel des règles principales

- **Jamais de modification directe sur `main`**
- ** Travailler toujours avec des chemins relatifs sans quoi votre code ne sera pas transportable**
- **Toujours passer par une branche personnelle**
- **Toujours ouvrir une Pull Request pour proposer ses changements**
- **Toujours demander au moins une relecture avant de fusionner**
- **Toujours tester localement avant PR**
- **Push régulier de votre branche pour backuper votre travail**
- **Ne jamais ajouter de données patient ni sensibles dans GitHub**



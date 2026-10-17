# Cycle badminton · Seconde et Terminale

Outil de terrain pour un cycle de badminton en CA4, au lycée Georges Pompidou de Castelnau-le-Lez : 9 séances par niveau, une évaluation en S9, 7 terrains, 32 élèves.

**En ligne :** https://yannickdartois-hue.github.io/cycle-badminton/

## Contenu

- **Cycle guidé**, en Seconde et en Terminale : 9 séances prêtes de 75 min de pratique. Chaque séance a son déroulé, ses fiches d'exercices avec schémas, ses consignes, ses critères de réussite et les rôles (joueur, arbitre, observateur, coach).
- **Travail en autonomie** (démarche GAREEPS) : 9 leçons. Chaque élève part de son problème, se situe sur son étoile, pioche dans un catalogue de 14 thèmes et tient son carnet d'entraînement.
- **Tournois** : montante-descendante sur demi-terrain ou sur grand terrain, poules de 4 ou 5, rencontres entre binômes, ronde suisse et défi ATP. Saisie des scores, classement, minuteur, export et import.
- **Évaluation** : fiche d'évaluation finale, avec la saisie des notes et la grille imprimable.
- **Préparation** : banque d'exercices, échauffement d'équipe, débutants, différenciation, fiche coaching.

## Utilisation sur le terrain

- **Séance du jour** : sur une page de séance, appuie sur « Marquer comme séance du jour ». Les séances précédentes passent en « Faite ». Le bouton « Séance du jour » de la navigation y ramène directement. Seconde et Terminale ont chacune leur propre choix.
- **Vue terrain / vue préparation** : la vue terrain n'affiche que l'essentiel (schéma, rôles, critère de réussite). La vue préparation affiche la fiche complète.
- **Minuteur** : appuie sur un bloc de la frise de la séance pour lancer un minuteur de la durée du bloc.
- **Impression** : chaque séance s'imprime en fiche complète, même depuis la vue terrain. Les mêmes fiches existent en PDF, dans le dossier `pdf/`.

## Sur l'écran d'accueil

- **iPad** : dans Safari, Partager → « Sur l'écran d'accueil ».
- **Tablette Android** : dans Chrome, menu ⋮ → « Installer l'application » ou « Ajouter à l'écran d'accueil ».

L'outil installé garde ses propres données, séparées de celles du navigateur. Choisis l'une des deux façons de l'ouvrir et garde-la.

## Où sont gardées les données

Les tournois, les notes, la séance du jour et les listes de classe sont enregistrés **dans le navigateur de l'appareil**, sans compte et sans serveur.

- Rien ne passe d'un appareil à l'autre. Pour transférer les données de l'iPad vers l'ordinateur, utilise **Exporter** puis **Importer** sur la page Tournois.
- Si tu effaces les données de navigation, tout est perdu. Exporte régulièrement.
- Une connexion internet est nécessaire pour ouvrir l'outil.

## Fichiers

```
index.html             l'outil complet (un seul fichier)
manifest.webmanifest   nom et icônes de l'outil installé sur l'écran d'accueil
icon-180.png           icône de l'iPad (écran d'accueil)
icon-192.png           icônes Android
icon-512.png
pdf/              les 36 fiches à imprimer
  2de-S1 … S9     séances de Seconde
  Tle-S1 … S9     séances de Terminale
  Auto-L1 … L9    leçons du travail en autonomie
  Cycle-*.pdf     chaque cycle en un seul document
  Banque-exercices, Catalogue-autonomie, Carnet-entrainement,
  Fiche-echauffement-equipe, Fiche-evaluation-finale,
  Autonomie-etoile-grille
```

Les boutons « PDF » de l'outil vont chercher les fichiers dans `pdf/`. Garde ces noms exacts : GitHub distingue majuscules et minuscules.

## Mise à jour

Pour mettre à jour, envoie le fichier modifié avec le même nom (Add file → Upload files). Il remplace l'ancien, et GitHub Pages republie en une à deux minutes.

## Sources

Les situations sont tirées des cycles et des fiches des collègues EPS du lycée : C., T., T., A. B., et du carnet GAREEPS de D. et Y. Elles ont été adaptées à 7 terrains et 32 élèves, à partir du référentiel badminton CA4 du lycée. Les seuils de réussite sont des repères de départ.

## Design commun (17/10/2026)
- `eps-design.css` et `eps-commun.js` : socle visuel partagé par tous les cycles (volley, badminton, demi-fond, tennis de table, step). Le fichier est identique dans chaque dépôt : en cas de modification, recopier la même version partout.
- Couleur de l'activité : ligne `<style>:root{--sport:…}</style>` dans `index.html`.
- **Mode gymnase** : bouton en haut à droite. Actif par défaut quand l'appli est ouverte depuis l'écran d'accueil de l'iPad.
- `index-old.html` : la version d'avant, gardée telle quelle (bandeau jaune « Ancienne version »).

---
title: "S16 – Les boucles humaines"
niveau: "6e"
duree: "55 minutes"
periode: "P2 – Devenir chercheur"
univers_principal: "Programmer"
collection: "Algorithmique débranchée"
rituel: "CAN-03 – Boucles de calcul"
competences:
  - Repérer une séquence d'instructions répétée
  - Remplacer des répétitions par une boucle
  - Exécuter littéralement un programme
  - Déterminer le contenu et le nombre de répétitions
  - Comparer deux programmes équivalents
  - Déboguer une boucle
statut: "Version 1"
---

# S16 – Les boucles humaines

## Idée générale

Après le robot maladroit et le programme saboté, les élèves découvrent une nouvelle instruction :

```text
RÉPÈTE ... FOIS
```

La boucle permet de remplacer une longue suite d'instructions identiques ou répétitives par un programme plus court.

Les élèves ne passent pas encore sur Scratch. Ils utilisent :

- un robot humain ;
- des cartes-instructions ;
- des plateaux quadrillés ;
- des programmes développés puis compressés ;
- des programmes contenant une boucle incorrecte.

La séance fait comprendre qu'une boucle doit préciser deux éléments :

1. **ce qui est répété** ;
2. **combien de fois la séquence est répétée**.

---

# Ressources associées

## Rituel

```text
05-Ressources/
└── 01-Rituels/
    └── Course-aux-nombres/
        └── CAN-03-Boucles-de-calcul.md
```

## Activité principale

```text
05-Ressources/
└── 02-Collections/
    └── Programmer/
        └── Algorithmique-debranchee/
            └── Boucles-humaines/
                ├── Boucles-humaines-Cartes-commandes.svg
                ├── Boucles-humaines-Plateaux.svg
                ├── Boucles-humaines-Fiche-eleve.md
                ├── Boucles-humaines-Defis-avances.md
                └── Boucles-humaines-Reperes-enseignant.md
```

---

# Mission du jour

> Un robot doit suivre plusieurs parcours, mais sa mémoire est presque pleine.  
> Vous devez raccourcir ses programmes sans modifier le trajet obtenu.

## Nouvelles instructions

```text
AVANCE 1
TOURNE À DROITE
TOURNE À GAUCHE
PRENDS LE JETON
STOP
```

Une boucle s'écrit :

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
```

## Règle fondamentale

Le robot exécute **toutes** les instructions placées dans la boucle, puis recommence depuis la première instruction de la boucle.

Une instruction placée après `FIN DE BOUCLE` n'est exécutée qu'une seule fois.

---

# Organisation

Équipes de quatre élèves.

## Rôles

### Robot

- se place sur le plateau ;
- regarde dans la direction indiquée ;
- exécute exactement les instructions ;
- n'anticipe jamais la cible.

### Lecteur

- lit une instruction à la fois ;
- annonce le début de chaque répétition ;
- ne corrige pas le robot pendant l'exécution.

### Programmeur

- organise les cartes ;
- propose la boucle ;
- note la version développée et la version raccourcie.

### Contrôleur

- suit le nombre de répétitions ;
- vérifie l'orientation ;
- repère le premier écart ;
- compare les deux programmes.

Les rôles tournent après chaque mission.

---

# Préparation de l'enseignant

## Matériel par équipe

- un jeu de cartes-commandes ;
- les quatre plateaux ;
- une fiche élève ;
- un pion orienté ou une flèche en papier ;
- quatre jetons ;
- un crayon ;
- éventuellement une petite grille au sol.

## Avant la séance

- découper les cartes-commandes ;
- préparer les plateaux A à D ;
- vérifier les orientations initiales ;
- conserver les défis avancés pour la fin ;
- prévoir un espace permettant à un élève de jouer le robot ;
- préparer au tableau une paire de programmes équivalents.

---

# Déroulement détaillé

## 1. Rituel – 5 minutes

Utiliser :

**CAN-03 – Boucles de calcul**

Les élèves exécutent plusieurs fois la même opération et cherchent une écriture plus compacte.

---

## 2. Échauffement humain – 5 minutes

Donner oralement :

```text
AVANCE
AVANCE
AVANCE
AVANCE
AVANCE
```

Puis demander :

> Comment dire la même chose plus rapidement sans changer le résultat ?

Faire apparaître :

```text
RÉPÈTE 5 FOIS
    AVANCE
FIN DE BOUCLE
```

Deuxième exemple :

```text
FRAPPE DANS TES MAINS
TOURNE D'UN QUART DE TOUR
FRAPPE DANS TES MAINS
TOURNE D'UN QUART DE TOUR
FRAPPE DANS TES MAINS
TOURNE D'UN QUART DE TOUR
FRAPPE DANS TES MAINS
TOURNE D'UN QUART DE TOUR
```

Version comprimée :

```text
RÉPÈTE 4 FOIS
    FRAPPE DANS TES MAINS
    TOURNE D'UN QUART DE TOUR
FIN DE BOUCLE
```

Faire exécuter les deux versions.

---

## 3. Mission A – La ligne trop longue – 6 minutes

Le robot part de `A`, orienté vers l'est, et doit atteindre `B`, cinq cases plus loin.

## Programme développé

```text
AVANCE 1
AVANCE 1
AVANCE 1
AVANCE 1
AVANCE 1
STOP
```

## Travail demandé

1. exécuter le programme ;
2. entourer la partie répétée ;
3. écrire une boucle équivalente ;
4. comparer le nombre de blocs.

## Réponse attendue

```text
RÉPÈTE 5 FOIS
    AVANCE 1
FIN DE BOUCLE
STOP
```

---

## 4. Mission B – Le carré parfait – 9 minutes

Le robot part du coin inférieur gauche d'un carré de deux cases de côté, orienté vers la droite.

Il doit :

- parcourir tout le contour ;
- revenir au point de départ ;
- retrouver son orientation initiale.

## Programme développé

```text
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
STOP
```

## Questions

- Quelle séquence se répète ?
- Combien de fois ?
- Pourquoi la rotation doit-elle être dans la boucle ?
- Où se trouve le robot après trois répétitions ?
- Où regarde-t-il à la fin ?

## Réponse attendue

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
STOP
```

---

## 5. Mission C – La ronde des quatre jetons – 10 minutes

Le robot parcourt le même carré.

Un jeton se trouve à chaque sommet atteint après un déplacement.

Le robot doit :

- atteindre un sommet ;
- prendre le jeton ;
- tourner ;
- recommencer ;
- revenir au point de départ après avoir pris le quatrième jeton.

## Programme attendu

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    PRENDS LE JETON
    TOURNE À GAUCHE
FIN DE BOUCLE
STOP
```

## Point de vigilance

L'instruction `PRENDS LE JETON` appartient à la boucle.

Si elle est placée après la boucle, le robot ne la réalise qu'une seule fois.

## Vérification

Le contrôleur complète :

| Répétition | Position atteinte | Jeton pris ? | Orientation après rotation |
|---:|---|:---:|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |
| 4 | | | |

---

## 6. Mission D – Les boucles sabotées – 10 minutes

Trois programmes sont proposés pour le carré.

### Programme D1

```text
RÉPÈTE 3 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
STOP
```

### Programme D2

```text
RÉPÈTE 4 FOIS
    AVANCE 2
FIN DE BOUCLE
TOURNE À GAUCHE
STOP
```

### Programme D3

```text
RÉPÈTE 4 FOIS
    TOURNE À GAUCHE
    AVANCE 2
FIN DE BOUCLE
STOP
```

## Travail demandé

Pour chaque programme :

1. prévoir le trajet sans déplacer le robot ;
2. exécuter pour vérifier ;
3. repérer le premier écart ;
4. expliquer la cause ;
5. proposer la correction minimale.

## Corrections attendues

### D1

Remplacer `3` par `4`.

### D2

Placer `TOURNE À GAUCHE` dans la boucle.

### D3

Inverser les deux instructions dans la boucle.

---

## 7. Comparer deux programmes – 5 minutes

Comparer :

### Programme P

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
```

### Programme Q

```text
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
AVANCE 2
TOURNE À GAUCHE
```

Questions :

- Les deux programmes produisent-ils le même trajet ?
- Lequel est le plus court ?
- Lequel est le plus facile à modifier pour tracer un hexagone ?
- Un programme plus court est-il forcément plus facile à comprendre ?

Faire apparaître la notion de programmes **équivalents**.

---

## 8. Bilan – 5 minutes

Faire compléter :

```text
Une boucle est utile lorsque…
Le nombre après RÉPÈTE indique…
Les instructions entre RÉPÈTE et FIN DE BOUCLE…
Une instruction placée après la boucle…
Pour déboguer une boucle, je vérifie d'abord…
```

Synthèse :

> Une boucle raccourcit un programme en répétant exactement la même séquence. Il faut choisir correctement le nombre de répétitions et les instructions placées à l'intérieur.

---

# Trace de fin de séance

```text
Une boucle contient :
______________________________________________________

Dans le programme du carré, la séquence répétée est :
______________________________________________________

Elle est répétée ______ fois.

L'instruction TOURNE doit être dans la boucle parce que :
______________________________________________________

Deux programmes sont équivalents lorsqu'ils :
______________________________________________________
```

---

# Différenciation

## Aide légère

- entourer la première occurrence du motif ;
- demander de retrouver les occurrences identiques ;
- utiliser une couleur pour le déplacement et une autre pour la rotation.

## Aide intermédiaire

Fournir le cadre :

```text
RÉPÈTE ____ FOIS
    ______________________
    ______________________
FIN DE BOUCLE
```

## Aide renforcée

- faire manipuler les cartes avant d'écrire ;
- limiter à une seule instruction dans la boucle ;
- utiliser une bande numérotée pour compter les répétitions ;
- faire annoncer : « répétition 1 », « répétition 2 »…

## Élèves rapides

Utiliser :

**Boucles-humaines-Defis-avances.md**

Défis possibles :

1. construire une boucle pour un triangle équilatéral symbolique ;
2. créer un programme développé et sa version compressée ;
3. trouver plusieurs boucles équivalentes ;
4. corriger un programme contenant deux erreurs ;
5. introduire une boucle contenant une action avant et après la répétition ;
6. créer un défi à tester par une autre équipe.

---

# Observation de l'enseignant

Observer notamment :

- le repérage exact de la séquence répétée ;
- le choix du nombre de répétitions ;
- la distinction intérieur/extérieur de la boucle ;
- l'exécution littérale ;
- l'orientation du robot ;
- la localisation du premier écart ;
- la correction minimale ;
- la comparaison de programmes équivalents.

La réussite ne consiste pas seulement à raccourcir. Le programme comprimé doit produire exactement le même résultat.

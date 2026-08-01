---
title: "EUR-03 – Les quatre reines"
niveau: "6e"
type: "Énigme de placement"
duree: "6 minutes"
utilisation: "S11 – Échecs : capturer ou protéger ?"
statut: "Version 1"
---

# EUR-03 – Les quatre reines

## Énigme

Place quatre reines sur un échiquier de `4 × 4` de manière qu'aucune reine ne puisse en capturer une autre.

Une reine attaque :

- toute sa ligne ;
- toute sa colonne ;
- les deux diagonales passant par sa case.

```text
┌───┬───┬───┬───┐
│   │   │   │   │
├───┼───┼───┼───┤
│   │   │   │   │
├───┼───┼───┼───┤
│   │   │   │   │
├───┼───┼───┼───┤
│   │   │   │   │
└───┴───┴───┴───┘
```

## Organisation

- 3 minutes de recherche individuelle ou en binôme ;
- 2 minutes de comparaison ;
- 1 minute de correction.

## Une solution

En numérotant les colonnes de 1 à 4, placer les reines :

```text
ligne 1 : colonne 2
ligne 2 : colonne 4
ligne 3 : colonne 1
ligne 4 : colonne 3
```

Représentation :

```text
· D · ·
· · · D
D · · ·
· · D ·
```

L'autre solution est obtenue par symétrie :

```text
· · D ·
D · · ·
· · · D
· D · ·
```

## Stratégie à valoriser

Une fois une reine placée, barrer mentalement ou au crayon :

- sa ligne ;
- sa colonne ;
- ses diagonales.

L'énigme prépare la lecture des lignes d'attaque sur un échiquier.

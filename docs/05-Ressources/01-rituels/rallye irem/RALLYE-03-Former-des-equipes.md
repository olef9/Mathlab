---
title: "RALLYE-03 – Former des équipes"
niveau: "6e"
type: "Énigme rapide issue du Rallye cycle 3"
duree: "6 minutes"
utilisation: "S15 – Le code des Mayas"
source: "Adaptation de l'épreuve Équipes, niveau facile, Rallye cycle 3 2026, IREM Paris-Nord"
statut: "Version 1"
---

# RALLYE-03 – Former des équipes

## Énigme

Un groupe de **17 participants** doit être réparti uniquement en :

- équipes de deux ;
- équipes de trois.

Trouve **toutes les répartitions possibles**.

## Tableau de recherche

| Équipes de 2 | Équipes de 3 | Nombre total |
|---:|---:|---:|
| | | |
| | | |
| | | |
| | | |

## Solutions

```text
7 équipes de 2 et 1 équipe de 3
7 × 2 + 1 × 3 = 17
```

```text
4 équipes de 2 et 3 équipes de 3
4 × 2 + 3 × 3 = 17
```

```text
1 équipe de 2 et 5 équipes de 3
1 × 2 + 5 × 3 = 17
```

Il existe donc trois répartitions.

## Méthode à valoriser

Commencer par le plus grand nombre possible d'équipes de trois, puis diminuer ce nombre de deux en deux :

```text
5 équipes de 3 → il reste 2
3 équipes de 3 → il reste 8
1 équipe de 3 → il reste 14
```

Les restes sont alors divisibles par deux.

## Prolongement express

Pourquoi le nombre d'équipes de trois doit-il être impair ?

Parce que :

- `17` est impair ;
- un nombre d'équipes de deux représente toujours un nombre pair de personnes ;
- il faut donc qu'un nombre impair de groupes de trois fournisse une contribution impaire.

## Source

Adaptation du niveau facile de l'épreuve **Équipes**, Rallye mathématique cycle 3 2026 de l'IREM Paris-Nord.

---
title: "CAN-02 – Calculs en chaîne"
niveau: "6e"
type: "Course aux nombres"
duree: "5 minutes"
utilisation: "S08 – Le programme saboté"
statut: "Version 1"
---

# CAN-02 – Calculs en chaîne

## Consigne

> Chaque résultat sert de départ au calcul suivant.  
> Écrivez tous les résultats intermédiaires.

## Chaîne principale

Départ : `12`

| Étape | Instruction | Résultat |
|---:|---|---:|
| 1 | Ajouter 8 | 20 |
| 2 | Multiplier par 3 | 60 |
| 3 | Retirer 15 | 45 |
| 4 | Diviser par 5 | 9 |
| 5 | Ajouter 31 | 40 |
| 6 | Prendre la moitié | 20 |
| 7 | Multiplier par 4 | 80 |
| 8 | Retirer 19 | 61 |

## Bonus

Départ : `25`

```text
× 4 → − 30 → ÷ 7 → + 6
```

Résultats :

```text
25 → 100 → 70 → 10 → 16
```

## Stratégie à valoriser

Une erreur dans une étape modifie tous les résultats suivants.

Pour retrouver une erreur, il faut vérifier les calculs dans l'ordre et repérer la première étape incorrecte.

Le rituel prépare directement la démarche de débogage.

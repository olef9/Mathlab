---
title: "La numération des Trioz – Repères enseignant"
niveau: "6e"
collection: "Chercher – Numérations"
seance_associee: "S05 – La numération des Trioz"
support: "Yvan Monka – Maths et Tiques"
statut: "Version 1"
---

# La numération des Trioz – Repères enseignant

## Principe mathématique

La numération des Trioz est une numération de position en base 3.

Les symboles représentent :

| Symbole trioz | Valeur |
|---|---:|
| `⊚` | 0 |
| `⫯` | 1 |
| `♋` | 2 |

Les valeurs de position, de droite à gauche, sont :

```text
1 ; 3 ; 9 ; 27 ; 81 ; ...
```

Une écriture `abcd` représente donc :

```text
a × 27 + b × 9 + c × 3 + d
```

---

# Réponses au document

## Tableau A

| Terre | Triozon |
|---:|---|
| 0 | `⊚` |
| 1 | `⫯` |
| 2 | `♋` |
| 3 | `⫯ ⊚` |
| 4 | `⫯ ⫯` |
| 5 | `⫯ ♋` |
| 6 | `♋ ⊚` |
| 7 | `♋ ⫯` |
| 8 | `♋ ♋` |
| 9 | `⫯ ⊚ ⊚` |
| 10 | `⫯ ⊚ ⫯` |

## Question 2

Le premier nombre nécessitant quatre symboles est :

```text
27 = ⫯ ⊚ ⊚ ⊚
```

## Question 3

```text
⫯ ♋ ⊚ ♋
```

correspond à :

```text
1 × 27 + 2 × 9 + 0 × 3 + 2
= 27 + 18 + 2
= 47
```

## Question 4

```text
45 = ⫯ ♋ ⊚ ⊚
```

car :

```text
45 = 1 × 27 + 2 × 9
```

et :

```text
62 = ♋ ⊚ ♋ ♋
```

car :

```text
62 = 2 × 27 + 0 × 9 + 2 × 3 + 2
```

---

# Tableau B – Calculs

## Première ligne

```text
2 × 4 = 8
```

Chez les Trioz :

```text
♋ × ⫯ ⫯ = ♋ ♋
```

## Deuxième ligne

```text
2 × 5 = 10
```

Chez les Trioz :

```text
♋ × ⫯ ♋ = ⫯ ⊚ ⫯
```

## Troisième ligne

```text
2 × 3 = 6
```

Chez les Trioz :

```text
♋ × ⫯ ⊚ = ♋ ⊚
```

## Quatrième ligne

```text
4 × 10 = 40
```

Chez les Trioz :

```text
⫯ ⫯ × ⫯ ⊚ ⫯ = ⫯ ⫯ ⫯ ⫯
```

---

# Tableau C – Régularités

## Première ligne

```text
2 × 3 = 6
```

Chez les Trioz :

```text
♋ × ⫯ ⊚ = ♋ ⊚
```

## Deuxième ligne

```text
5 × 3 = 15
```

Chez les Trioz :

```text
⫯ ♋ × ⫯ ⊚ = ⫯ ♋ ⊚
```

## Troisième ligne

```text
2 × 9 = 18
```

Chez les Trioz :

```text
♋ × ⫯ ⊚ ⊚ = ♋ ⊚ ⊚
```

## Quatrième ligne

```text
3 × 9 = 27
```

Chez les Trioz :

```text
⫯ ⊚ × ⫯ ⊚ ⊚ = ⫯ ⊚ ⊚ ⊚
```

## Remarque attendue

Dans la numération des Trioz :

- multiplier par `⫯ ⊚`, c'est-à-dire par 3, ajoute un zéro à droite ;
- multiplier par `⫯ ⊚ ⊚`, c'est-à-dire par 9, ajoute deux zéros à droite.

C'est le même principe que dans notre numération décimale lorsque l'on multiplie un entier par 10 ou par 100.

---

# Méthodes de conversion

## De Triozon vers la Terre

Exemple :

```text
♋ ⊚ ♋ ♋
```

Tableau de position :

| Symbole | 2 | 0 | 2 | 2 |
|---|---:|---:|---:|---:|
| Valeur du rang | 27 | 9 | 3 | 1 |
| Contribution | 54 | 0 | 6 | 2 |

Total :

```text
54 + 0 + 6 + 2 = 62
```

## De la Terre vers Triozon

### Méthode par décomposition

Pour 45 :

```text
45 = 27 + 18
45 = 1 × 27 + 2 × 9 + 0 × 3 + 0
```

donc :

```text
45 = ⫯ ♋ ⊚ ⊚
```

### Méthode par divisions successives

Pour 62 :

```text
62 ÷ 3 = 20 reste 2
20 ÷ 3 = 6 reste 2
6 ÷ 3 = 2 reste 0
2 ÷ 3 = 0 reste 2
```

Les restes lus de bas en haut donnent :

```text
2022
```

soit :

```text
♋ ⊚ ♋ ♋
```

La méthode par divisions successives peut être réservée aux élèves qui la découvrent ou à un prolongement.

---

# Progression des aides

## Aide 1 – Poursuivre la suite

Faire écrire :

```text
0 ; 1 ; 2 ; 10 ; 11 ; 12 ; 20 ; ...
```

avec les chiffres terrestres avant de revenir aux symboles trioz.

## Aide 2 – Comparer à un compteur

Demander :

> Que fait un compteur terrestre après 9 ?  
> Que doit faire un compteur trioz après 2 ?

## Aide 3 – Valeurs de position

Donner :

```text
tout à droite : 1
puis : 3
puis : 9
puis : 27
```

## Aide 4 – Jetons et échanges

Matérialiser :

```text
3 unités = 1 paquet de trois
3 paquets de trois = 1 paquet de neuf
3 paquets de neuf = 1 paquet de vingt-sept
```

## Aide 5 – Décomposition partielle

Pour 47, écrire :

```text
47 = 27 + 18 + ...
```

et laisser l'élève terminer.

---

# Erreurs fréquentes

## Lire `⫯ ⊚` comme « dix »

Le symbole ressemble à notre écriture 10, mais sa valeur est 3.

Réponse possible :

> Les symboles sont les mêmes positions, mais les échanges se font après 2 et non après 9.

## Additionner les symboles

Par exemple, interpréter `⫯ ♋ ⊚ ♋` comme `1 + 2 + 0 + 2`.

Faire rappeler que la position modifie la valeur.

## Utiliser un chiffre 3

En base 3, seuls 0, 1 et 2 sont autorisés.

## Confondre nombre et écriture

Le nombre 3 existe chez les Trioz, mais il s'écrit `⫯ ⊚`.

## Oublier un rang nul

Pour 45, certains élèves écrivent `⫯ ♋` au lieu de `⫯ ♋ ⊚ ⊚`.

Faire utiliser le tableau des rangs.

## Croire que quatre symboles commencent à 10

Le nombre d'écritures possibles avec trois positions est :

```text
3 × 3 × 3 = 27
```

Les quatre symboles commencent donc à 27.

---

# Bilan conseillé

Ne pas commencer par annoncer « base 3 ».

Faire d'abord expliquer :

- les trois chiffres disponibles ;
- le passage après 2 ;
- la valeur des positions ;
- un exemple de conversion.

Puis donner le vocabulaire :

> Les Trioz utilisent une numération de position en base 3.

Question centrale :

> Qu'est-ce qui ressemble à notre système décimal et qu'est-ce qui change ?

Réponses attendues :

- ressemblance : la position d'un chiffre détermine sa valeur ;
- différence : les échanges se font par groupes de 3 au lieu de groupes de 10.

---

# Préparation d'une future vidéo

Cette séance peut servir plus tard de sujet à une capsule réalisée par un groupe.

La vidéo pourrait expliquer :

1. les trois symboles ;
2. comment compter de 0 à 10 ;
3. une conversion dans chaque sens ;
4. la règle de multiplication par `⫯ ⊚`.

Pour une diffusion publique, utiliser des exemples et des visuels créés par les élèves. Le document original comporte une mention limitant sa reproduction hors du cadre de la classe : ne pas afficher ou republier la fiche intégrale sans autorisation.

---

# Source

Yvan Monka, Académie de Strasbourg, **La numération des Trioz**, Maths et Tiques.

Conserver l'attribution sur le document original.

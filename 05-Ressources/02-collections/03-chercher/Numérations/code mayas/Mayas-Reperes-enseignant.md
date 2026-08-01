---
title: "Le code des Mayas – Repères enseignant"
niveau: "6e"
seance_associee: "S15 – Le code des Mayas"
statut: "Version 1"
---

# Repères enseignant – Le code des Mayas

## Précision historique et mathématique

La numération maya utilise couramment :

- un point pour `1` ;
- une barre pour `5` ;
- un signe en forme de coquillage pour `0`.

Les chiffres de `0` à `19` combinent ces symboles.

Dans une écriture positionnelle purement vigésimale :

```text
niveau 1 : 1
niveau 2 : 20
niveau 3 : 400
niveau 4 : 8000
```

Les niveaux de poids plus élevé sont placés au-dessus.

## Variante calendaire

Le calendrier maya utilise une adaptation dans laquelle un des niveaux vaut `360` plutôt que `400`.

Pour éviter de mélanger deux systèmes lors d'une première découverte, toute la séance utilise la version pure en base 20.

Le préciser seulement si la question apparaît.

---

# Lecture des chiffres de 0 à 19

Pour un chiffre `n` :

```text
nombre de barres = quotient entier de n par 5
nombre de points = reste de la division par 5
```

Exemples :

| Nombre | Barres | Points |
|---:|---:|---:|
| 3 | 0 | 3 |
| 5 | 1 | 0 |
| 8 | 1 | 3 |
| 13 | 2 | 3 |
| 19 | 3 | 4 |

Le zéro est représenté par le coquillage.

---

# Tablette mystère – Corrections

## Première série

| Inscription | Valeur |
|---|---:|
| 1 point | 1 |
| 4 points | 4 |
| 1 barre | 5 |
| 1 barre et 3 points | 8 |
| 2 barres et 3 points | 13 |
| 3 barres et 4 points | 19 |

## Deuxième série

### 20

```text
niveau 2 : 1
niveau 1 : 0
```

Calcul :

```text
1 × 20 + 0 = 20
```

### 21

```text
niveau 2 : 1
niveau 1 : 1
```

### 25

```text
niveau 2 : 1
niveau 1 : 5
```

### 39

```text
niveau 2 : 1
niveau 1 : 19
```

### 45

```text
niveau 2 : 2
niveau 1 : 5
```

### 400

```text
niveau 3 : 1
niveau 2 : 0
niveau 1 : 0
```

---

# Cartes experts

## Carte A – Décoder

Inscription :

```text
niveau 2 : 2
niveau 1 : 7
```

Calcul :

```text
2 × 20 + 7 = 47
```

## Carte B – Coder 239

Division par 20 :

```text
239 = 11 × 20 + 19
```

Inscription :

```text
niveau 2 : 11
niveau 1 : 19
```

## Carte C – Identifier 405

Décomposition :

```text
405 = 1 × 400 + 0 × 20 + 5
```

Inscription correcte :

```text
niveau 3 : 1
niveau 2 : coquillage
niveau 1 : 5
```

Le zéro intermédiaire ne peut pas être supprimé.

## Carte D – Corriger la traduction

Inscription :

```text
niveau 3 : 2
niveau 2 : 0
niveau 1 : 5
```

La traduction `205` est fausse.

Calcul correct :

```text
2 × 400 + 0 × 20 + 5 = 805
```

Erreur probable :

le scribe a lu les niveaux comme les chiffres décimaux `2`, `0`, `5`.

---

# Défi collectif

## Inscription 1 ; 0 ; 18

```text
1 × 400 + 0 × 20 + 18 = 418
```

## Nombre 799

```text
799 ÷ 400 = 1 reste 399
399 ÷ 20 = 19 reste 19
```

Donc :

```text
niveau 3 : 1
niveau 2 : 19
niveau 1 : 19
```

---

# Aides progressives

## Aide 1 – Décomposer chaque chiffre

Faire écrire :

```text
13 = 2 × 5 + 3
```

## Aide 2 – Lire du bas vers le haut

Numéroter les niveaux :

```text
1 en bas
2 au milieu
3 en haut
```

## Aide 3 – Tableau des poids

| Niveau | Poids |
|---:|---:|
| 3 | 400 |
| 2 | 20 |
| 1 | 1 |

## Aide 4 – Matériel

Utiliser :

- cailloux ou jetons pour les points ;
- bâtonnets pour les barres ;
- carte vide pour le zéro.

Regrouper vingt unités pour fabriquer un jeton au niveau supérieur.

## Aide 5 – Partir du calcul

Pour coder `239`, fournir :

```text
239 = 11 × 20 + 19
```

L'élève doit seulement traduire les deux chiffres.

---

# Erreurs fréquentes

## Lire de haut en bas comme un nombre décimal

Une inscription `2 ; 0 ; 5` ne vaut pas `205`.

## Oublier le zéro intermédiaire

Sans le niveau zéro, les positions se décalent.

## Utiliser cinq points

Les cinq points sont remplacés par une barre.

## Mettre quatre barres dans un niveau

Quatre barres valent `20` et doivent être regroupées au niveau supérieur.

## Inverser unités et vingtaines

Le niveau du bas est celui des unités.

## Utiliser 400 trop tôt

Laisser d'abord les élèves stabiliser les deux niveaux.

---

# Comparaison avec les Trioz

## Point commun

Les deux écritures sont positionnelles :

```text
valeur du chiffre × valeur de la position
```

## Différences

| Trioz | Maya |
|---|---|
| base 3 | base 20 |
| trois chiffres possibles | vingt chiffres possibles de 0 à 19 |
| écriture horizontale dans l'activité | écriture verticale |
| chaque chiffre possède un symbole | un chiffre combine points et barres |

Cette comparaison permet de comprendre qu'une base ne correspond pas nécessairement au nombre de symboles graphiques élémentaires.

---

# Défis avancés – Corrections

## Défi 1 – Addition

Addition :

```text
(2 ; 17) + (1 ; 8)
```

Valeurs décimales :

```text
57 + 28 = 85
```

Calcul direct en base 20 :

```text
17 + 8 = 25 = 1 vingtaine + 5 unités
2 + 1 + 1 retenue = 4 vingtaines
```

Résultat :

```text
4 ; 5
```

## Défi 2 – Trois barres et quatre points

On cherche des nombres à deux niveaux.

Chaque niveau doit contenir au moins un point ou une barre.

### Plus petit

Mettre le minimum au niveau des vingtaines :

```text
niveau 2 : 1 point
niveau 1 : 3 barres et 3 points = 18
```

Valeur :

```text
1 × 20 + 18 = 38
```

### Plus grand

Mettre le maximum au niveau des vingtaines tout en conservant un symbole pour les unités :

```text
niveau 2 : 3 barres et 3 points = 18
niveau 1 : 1 point
```

Valeur :

```text
18 × 20 + 1 = 361
```

## Défi 3 – Coder 1234

```text
1234 = 3 × 400 + 34
34 = 1 × 20 + 14
```

Inscription :

```text
niveau 3 : 3
niveau 2 : 1
niveau 1 : 14
```

## Défi 4 – Créer une erreur

Vérifier que :

- l'inscription respecte les chiffres de 0 à 19 ;
- la traduction fausse est plausible ;
- la correction utilise les poids des niveaux.

## Défi 5 – Trois écritures

Choisir par exemple `47`.

```text
décimal : 47
maya : 2 ; 7
Trioz : 1202 en base 3
```

Vérification Trioz :

```text
1 × 27 + 2 × 9 + 0 × 3 + 2 = 47
```

---

# Sources documentaires

- Mathematical Association of America, présentation du système numérique maya et distinction entre numération pure et calendrier.
- Article pédagogique « The Ludic and Powerful Mayan Mathematics for Teaching », système positionnel de base 20 utilisant points, barres et zéro.
- Rallye mathématique cycle 3 2026 de l'IREM Paris-Nord, épreuve « Équipes » pour le rituel.

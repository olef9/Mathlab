---
title: "Les territoires aux champignons – Repères enseignant"
niveau: "6e"
seance_associee: "S18 – Les territoires aux champignons"
statut: "Version 1"
---

# Repères enseignant – Les territoires aux champignons

## Source et adaptation

La séance est une création Math’Lab inspirée de l’épreuve 7 du Rallye cycle 3 2022 de l’IREM Paris-Nord.

L’épreuve officielle demande de partager des terrains contenant plusieurs espèces de champignons avec des contraintes sur la nature des frontières, notamment :

- trois droites ;
- une droite et deux arcs de cercle.

La présente adaptation transpose l’idée sur quadrillage et ajoute :

- l’égalité des aires ;
- la connexité ;
- un exemplaire de chaque espèce ;
- la recherche de plusieurs solutions ;
- la comparaison de la longueur des frontières.

Le support officiel n’est pas reproduit.

---

# Données du grand terrain

Grille :

```text
6 × 6 = 36 cases
```

Nombre de territoires :

```text
4
```

Aire de chaque territoire :

```text
36 ÷ 4 = 9 cases
```

## Position des symboles

Les coordonnées sont données sous la forme :

```text
(ligne, colonne)
```

avec des numéros allant de `1` à `6`.

### Ronds

```text
(1,1)
(2,4)
(4,2)
(5,5)
```

### Triangles

```text
(1,5)
(3,3)
(5,1)
(6,6)
```

### Carrés

```text
(2,2)
(3,6)
(4,4)
(6,3)
```

Chaque ligne et chaque colonne contient exactement deux symboles.

---

# Échauffement `4 × 4`

Symboles :

- ronds en haut à gauche et en bas à droite ;
- triangles en haut à droite et en bas à gauche.

Solutions possibles :

- séparation verticale ;
- séparation horizontale ;
- plusieurs frontières en escalier.

Chaque territoire contient huit cases, un rond et un triangle.

---

# Solution 1 – Quatre carrés

Tracer :

- une frontière verticale entre les colonnes 3 et 4 ;
- une frontière horizontale entre les lignes 3 et 4.

On obtient quatre carrés `3 × 3`.

## Vérification

### Territoire supérieur gauche

```text
rond (1,1)
carré (2,2)
triangle (3,3)
```

### Territoire supérieur droit

```text
triangle (1,5)
rond (2,4)
carré (3,6)
```

### Territoire inférieur gauche

```text
rond (4,2)
triangle (5,1)
carré (6,3)
```

### Territoire inférieur droit

```text
carré (4,4)
rond (5,5)
triangle (6,6)
```

Chaque territoire possède neuf cases.

## Longueur des frontières intérieures

```text
6 + 6 = 12 segments-unités
```

---

# Solution 2 – Frontières en escalier horizontal

Conserver une frontière horizontale complète entre les lignes 3 et 4.

## Dans la moitié supérieure

Le territoire gauche contient :

```text
ligne 1 : colonnes 1 à 2
ligne 2 : colonnes 1 à 3
ligne 3 : colonnes 1 à 4
```

Aire :

```text
2 + 3 + 4 = 9
```

Le territoire droit est le complément dans les trois premières lignes.

## Dans la moitié inférieure

Le territoire gauche contient :

```text
ligne 4 : colonnes 1 à 4
ligne 5 : colonnes 1 à 3
ligne 6 : colonnes 1 à 2
```

Aire :

```text
4 + 3 + 2 = 9
```

Le territoire droit est le complément.

## Propriétés

- quatre territoires connectés ;
- aucun territoire rectangulaire ;
- un symbole de chaque espèce ;
- chaque territoire touche le bord extérieur.

## Longueur des frontières

```text
16 segments-unités
```

---

# Solution 3 – Escaliers verticaux

Conserver une frontière verticale complète entre les colonnes 3 et 4.

## Dans la moitié gauche

Le territoire supérieur contient :

```text
colonne 1 : lignes 1 à 2
colonne 2 : lignes 1 à 3
colonne 3 : lignes 1 à 4
```

Aire :

```text
2 + 3 + 4 = 9
```

Le territoire inférieur est le complément.

## Dans la moitié droite

Le territoire supérieur contient :

```text
colonne 4 : lignes 1 à 4
colonne 5 : lignes 1 à 3
colonne 6 : lignes 1 à 2
```

Aire :

```text
4 + 3 + 2 = 9
```

Le territoire inférieur est le complément.

## Propriétés

- solution distincte sur le terrain fixe ;
- aucun territoire rectangulaire ;
- longueur intérieure `16` ;
- un exemplaire de chaque symbole.

---

# Vérification de la connexité

## Méthode des élèves

Choisir une case du territoire.

La marquer, puis marquer toutes les cases accessibles en passant uniquement par un côté commun.

Le territoire est connecté si les neuf cases peuvent être atteintes.

## Méthode avec jetons

Placer un jeton sur une case du territoire.

Faire avancer le jeton de case en case sans sortir de la région.

## Erreur classique

Deux groupes de cases se touchant uniquement par un coin ne forment pas un seul territoire.

---

# Compter les frontières

Une arête intérieure compte une fois, même si elle borde deux territoires.

## Méthode

- repasser les frontières intérieures ;
- compter les segments horizontaux ;
- compter les segments verticaux ;
- additionner.

Ne pas compter le bord extérieur.

## Solutions connues

| Solution | Longueur intérieure |
|---|---:|
| Quatre carrés | 12 |
| Escaliers horizontaux | 16 |
| Escaliers verticaux | 16 |

Ne pas affirmer sans preuve que `12` est la longueur minimale parmi toutes les solutions possibles.

---

# Aides progressives

## Aide 1

```text
36 ÷ 4 = 9
```

## Aide 2

Faire repérer quatre groupes diagonaux de trois symboles dans les carrés `3 × 3`.

## Aide 3

Colorier légèrement les quatre carrés sans tracer les frontières.

## Aide 4

Pour la deuxième solution, donner les nombres :

```text
2 – 3 – 4
```

et demander de les interpréter comme longueurs de lignes.

## Aide 5

Tracer seulement les deux premiers segments de l’escalier.

## Aide 6

Donner une solution comportant deux cases volontairement échangées.

---

# Erreurs fréquentes

## Oublier l’aire

Une région peut contenir les bons symboles mais avoir huit ou dix cases.

## Créer un territoire en deux morceaux

Souvent provoqué par une case isolée près d’un symbole.

## Compter une diagonale comme connexion

Rappeler la connexion par les côtés.

## Modifier une frontière sans compensation

Si un territoire gagne une case, un autre doit la perdre.

## Vérifier uniquement les symboles

Les six règles sont indépendantes.

## Colorier trop tôt

Faire tracer les frontières au crayon avant le coloriage.

---

# Questions de mise en commun

- Comment avez-vous trouvé la première solution ?
- Comment avez-vous déformé une frontière en conservant l’aire ?
- Quelle contrainte était la plus fragile ?
- Comment vérifier rapidement une région de neuf cases ?
- Plusieurs solutions peuvent-elles avoir la même longueur de frontière ?
- Une forme originale est-elle forcément plus difficile à vérifier ?

---

# Patrimoine Math’Lab

Conserver :

- le terrain de départ ;
- deux solutions d’une même équipe ;
- les tableaux de validation ;
- la comparaison des frontières ;
- un défi créé.

Dossier conseillé :

```text
10-Patrimoine-MathLab/
└── Recherches/
    └── S18-Territoires-aux-champignons/
```

---
title: "Le coffre des quatre verrous – Repères enseignant renforcés"
niveau: "6e"
seance_associee: "S10 – Le coffre des quatre verrous"
statut: "Version 2"
---

# Repères enseignant – Version renforcée

## Vue d'ensemble

| Symbole | Énigme | Résultat | Chiffre |
|---|---|---:|---:|
| Carré | Compter tous les carrés d'une grille `3 × 3` | 14 | 4 |
| Cercle | Chemins les plus courts évitant un segment | 6 | 6 |
| Étoile | Différence égale à `3 × Cercle` | `32 − 14 = 18` | 3 |
| Triangle | Différence égale à `5 × Carré − 1` | `72 − 53 = 19` | 7 |

Ordre final :

```text
Étoile – Cercle – Carré – Triangle
```

Code :

```text
3647
```

---

# Carte Carré

## Énoncé

Compter tous les carrés d'une grille `3 × 3`.

Le résultat comporte deux chiffres. Le verrou conserve le chiffre des unités.

## Dénombrement

- `9` carrés `1 × 1` ;
- `4` carrés `2 × 2` ;
- `1` carré `3 × 3`.

Total :

```text
9 + 4 + 1 = 14
```

Le chiffre du verrou est donc :

```text
4
```

## Exigence de justification

Refuser une réponse `14` obtenue sans classement.

L'objectif est de montrer que toutes les tailles ont été prises en compte.

---

# Carte Cercle

## Configuration

Le quadrillage nécessite :

- trois déplacements vers la droite ;
- deux déplacements vers le bas.

Sans interdiction, le nombre de chemins courts est :

```text
10
```

Le segment interdit relie les points `(1,1)` et `(2,1)` horizontalement.

## Dénombrement des chemins interdits

Pour atteindre le début du segment interdit `(1,1)`, il existe deux possibilités :

```text
DB
BD
```

Après avoir traversé le segment interdit, il reste un déplacement vers la droite et un vers le bas, dans deux ordres :

```text
DB
BD
```

Nombre de chemins utilisant le passage interdit :

```text
2 × 2 = 4
```

Nombre de chemins autorisés :

```text
10 − 4 = 6
```

Le chiffre Cercle est donc :

```text
6
```

## Méthode alternative

Les élèves peuvent lister les dix mots formés de trois `D` et deux `B`, puis barrer ceux qui traversent le passage interdit.

---

# Carte Étoile

## Données

Utiliser une fois chacun les chiffres :

```text
1, 2, 3 et 4
```

Former deux nombres à deux chiffres.

Leur différence doit être :

```text
3 × Cercle
```

Comme `Cercle = 6` :

```text
3 × 6 = 18
```

Le plus grand nombre doit être pair.

## Possibilités donnant 18

```text
32 − 14 = 18
41 − 23 = 18
```

La contrainte « le plus grand nombre est pair » élimine `41 − 23`.

Il reste :

```text
32 − 14 = 18
```

Le chiffre Étoile est le chiffre des dizaines du plus grand nombre :

```text
3
```

---

# Carte Triangle

## Données

Utiliser une fois chacun les chiffres :

```text
2, 3, 5 et 7
```

Former deux nombres à deux chiffres.

La différence doit être :

```text
5 × Carré − 1
```

Comme `Carré = 4` :

```text
5 × 4 − 1 = 19
```

## Solution

```text
72 − 53 = 19
```

Le chiffre Triangle est le chiffre des dizaines du plus grand nombre :

```text
7
```

## Vérification de l'unicité

L'élève peut classer les essais selon le chiffre des dizaines du plus grand nombre.

Avec `7` comme dizaine, les possibilités pertinentes sont :

```text
72 − 53 = 19
73 − 52 = 21
75 − 32 = 43
```

Les autres dizaines ne permettent pas d'obtenir 19 avec les quatre chiffres utilisés une seule fois.

---

# Ordre final

Contraintes :

```text
1. Triangle immédiatement après Carré.
2. Cercle ni premier ni dernier.
3. Étoile avant Carré.
```

Le bloc :

```text
Carré – Triangle
```

ne peut pas occuper les positions 1-2, car Étoile doit être avant Carré.

S'il occupe 2-3 :

- Étoile doit être première ;
- Cercle serait quatrième, ce qui est interdit.

Le bloc doit donc occuper les positions 3-4.

Parmi les deux places restantes :

- Cercle ne peut pas être premier ;
- Cercle est donc deuxième ;
- Étoile est première.

Ordre unique :

```text
Étoile – Cercle – Carré – Triangle
```

Code :

```text
3647
```

---

# Aides progressives

## Carré

1. Combien de petits carrés ?
2. Combien de carrés formés de quatre cases ?
3. Existe-t-il un carré encore plus grand ?

## Cercle

1. Écrire tous les chemins avec trois `D` et deux `B`.
2. Repérer les chemins traversant le segment marqué.
3. Classer selon les deux premiers déplacements.

## Étoile

1. Calculer `3 × Cercle`.
2. Chercher toutes les soustractions donnant 18.
3. Utiliser ensuite la parité.

## Triangle

1. Calculer `5 × Carré − 1`.
2. Commencer par les nombres dont la dizaine est 7.
3. Conserver les chiffres déjà utilisés.

---

# Erreurs fréquentes

- Carré : oublier les carrés `2 × 2`.
- Cercle : compter des chemins comportant un détour.
- Étoile : utiliser deux fois le même chiffre.
- Étoile : conserver `41 − 23` malgré la contrainte de parité.
- Triangle : annoncer `72 − 53` sans chercher l'unicité.
- Ordre : interpréter « immédiatement après » comme « quelque part après ».

---

# Gestion des rythmes

## Groupe en difficulté

Valider deux cartes complètes et accompagner les deux cartes dépendantes.

## Groupe dans le rythme

Résoudre les quatre cartes et justifier l'ordre.

## Groupe rapide

Commencer par le défi de la grille `4 × 4`, puis le deuxième passage interdit.

## Groupe très rapide

Créer un coffre cohérent pour une autre équipe.

---

# Bilan conseillé

Comparer les quatre démarches :

- classer par taille ;
- dénombrer des chemins ;
- chercher toutes les soustractions possibles ;
- raisonner sur des positions.

Faire émerger :

> Une même mission coopérative peut réunir plusieurs formes de raisonnement mathématique.

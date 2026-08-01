---
title: "Les territoires aux champignons – Défis avancés"
niveau: "6e"
seance_associee: "S18 – Les territoires aux champignons"
statut: "Version 1"
---

# Défis avancés

## Défi 1 – Une troisième solution

Trouve une troisième solution différente des deux premières.

Elle doit respecter toutes les règles.

Pour prouver qu’elle est nouvelle, indique au moins deux cases qui changent de territoire.

---

# Défi 2 – Frontière de longueur 16

Construis un partage valide dont les frontières intérieures mesurent exactement :

```text
16 segments-unités
```

Méthode possible :

- commencer par une frontière horizontale ;
- construire deux frontières en escalier ;
- compter chaque côté de case séparant deux territoires.

---

# Défi 3 – Tous au bord

Trouve une solution dans laquelle chacun des quatre territoires touche le bord extérieur du grand carré.

Précise pour chacun :

| Territoire | Bord touché |
|---|---|
| 1 | |
| 2 | |
| 3 | |
| 4 | |

Un même territoire peut toucher plusieurs bords.

---

# Défi 4 – Créer un nouveau terrain

Sur une grille `6 × 6` vide, place :

- quatre ronds ;
- quatre triangles ;
- quatre carrés.

Ton terrain doit posséder :

- une solution en quatre carrés `3 × 3` ;
- une deuxième solution sans territoire rectangulaire.

Fournis :

- le terrain ;
- les deux solutions ;
- les quatre tableaux de vérification.

---

# Défi 5 – Le champignon déplacé

Déplace exactement un symbole d’une case.

Questions :

- l’ancienne solution reste-t-elle valide ?
- peut-on réparer le partage en modifiant une seule frontière ?
- combien de cases doivent changer de territoire ?

Conserve le terrain avant et après.

---

# Défi 6 – Droites et arcs

Le Rallye cycle 3 2022 proposait de partager des terrains contenant plusieurs espèces de champignons en imposant des frontières constituées de droites ou d’arcs.

Crée un petit terrain non quadrillé contenant trois espèces.

Propose deux versions :

```text
Version A : trois droites
Version B : une droite et deux arcs de cercle
```

Chaque région finale ne doit contenir qu’une seule espèce.

Teste ton dessin sur une autre équipe.

---

# Défi 7 – Argument d’impossibilité

Une équipe affirme avoir partagé une grille de `6 × 6` en cinq territoires possédant tous le même nombre entier de cases.

Explique pourquoi c’est impossible.

## Réponse

```text
36 n’est pas divisible par 5.
```

Les cinq territoires ne peuvent donc pas avoir exactement la même aire exprimée en cases entières.

---
title: "S10 – Le coffre des quatre verrous"
niveau: "6e"
duree: "55 minutes"
periode: "P1 – Entrer dans le Math'Lab"
univers_principal: "Chercher"
collection: "Recherche coopérative"
rituel: "KANG-03 – Les pages du livre"
version: "Renforcée"
competences:
  - Organiser un dénombrement
  - Chercher plusieurs possibilités sans doublon
  - Exploiter le résultat d'un autre expert
  - Résoudre une situation à contraintes
  - Justifier l'unicité d'une réponse
  - Coopérer et vérifier une solution collective
statut: "Version 2 – énigmes renforcées"
---

# S10 – Le coffre des quatre verrous

## Idée générale

Un coffre du Math'Lab est protégé par quatre symboles :

- Carré ;
- Cercle ;
- Étoile ;
- Triangle.

Chaque expert reçoit une énigme différente.

Les deux premières cartes produisent directement un chiffre :

- **Carré** : dénombrement de carrés ;
- **Cercle** : dénombrement organisé de chemins.

Les deux autres cartes dépendent des résultats précédents :

- **Étoile** utilise le chiffre du Cercle ;
- **Triangle** utilise le chiffre du Carré.

Les élèves doivent ensuite déterminer l'ordre des quatre symboles grâce à des contraintes logiques.

---

# Ressources associées

## Rituel

```text
05-Ressources/
└── 01-Rituels/
    └── Kangourou/
        └── KANG-03-Les-pages-du-livre.md
```

## Activité principale

```text
05-Ressources/
└── 02-Collections/
    └── Chercher/
        └── Recherche-cooperative/
            └── Coffre-quatre-verrous/
                ├── Coffre-quatre-verrous-Cartes-indices-renforcees.svg
                ├── Coffre-quatre-verrous-Fiche-equipe-renforcee.md
                ├── Coffre-quatre-verrous-Defis-avances-renforces.md
                └── Coffre-quatre-verrous-Reperes-enseignant-renforces.md
```

---

# Mission du jour

> Quatre experts, quatre énigmes et un seul code.  
> Aucun élève ne possède toutes les informations.  
> Résolvez votre carte, expliquez votre raisonnement, utilisez les résultats des autres et déterminez l'ordre unique du code.

## Règles

- Les cartes restent cachées pendant la recherche individuelle.
- Un résultat sans justification n'est pas accepté.
- Les essais doivent être conservés.
- Les cartes Étoile et Triangle ne peuvent être terminées sans coopération.
- Le code final ne doit pas être testé au hasard.
- L'équipe doit pouvoir expliquer pourquoi son ordre est unique.

---

# Organisation

Équipe idéale : quatre élèves.

| Expert | Nature de l'énigme |
|---|---|
| Carré | Compter tous les carrés d'une grille `3 × 3` |
| Cercle | Compter des chemins courts en évitant un passage interdit |
| Étoile | Former deux nombres avec quatre chiffres, grâce au résultat Cercle |
| Triangle | Former deux nombres avec quatre chiffres, grâce au résultat Carré |

Pour une équipe de trois, donner :

- Carré + Triangle au même élève ;
- ou Cercle + Étoile au même élève.

---

# Préparation de l'enseignant

## Matériel par équipe

- les quatre cartes renforcées découpées ;
- une fiche équipe ;
- du papier de brouillon ;
- quatre jetons portant les symboles ;
- une enveloppe représentant le coffre ;
- les défis avancés pour les groupes rapides.

## Code de validation

```text
3647
```

Ne pas l'afficher.

---

# Déroulement détaillé

## 1. Rituel Kangourou – 5 minutes

Utiliser :

**KANG-03 – Les pages du livre**

Faire verbaliser le classement entre nombres à un chiffre et nombres à deux chiffres.

---

## 2. Lancement – 4 minutes

Présenter les quatre symboles et distribuer les cartes face cachée.

> Votre carte peut être difficile.  
> Vous n'avez pas forcément toutes les données.  
> Préparez une explication qui permettra à l'équipe de vérifier votre résultat.

---

## 3. Recherche individuelle des experts – 12 minutes

Chaque expert travaille seul.

Il doit noter :

- ses essais ;
- sa méthode ;
- son résultat ou l'information qui manque ;
- une manière de vérifier.

### Relances possibles

#### Carré

- As-tu classé les carrés par taille ?
- As-tu compté le grand carré ?
- Comment éviter de compter deux fois le même carré ?

#### Cercle

- Combien de déplacements sont nécessaires ?
- Peux-tu coder un chemin avec `D` et `B` ?
- Quels chemins utilisent le passage interdit ?
- Comment prouver que ta liste est complète ?

#### Étoile et Triangle

- Quel résultat d'un autre expert attends-tu ?
- Quelle différence dois-tu obtenir ?
- Comment organiser les permutations des quatre chiffres ?
- As-tu utilisé chaque chiffre exactement une fois ?

---

## 4. Conseil des experts – 12 minutes

Chaque expert explique sa carte.

L'équipe complète :

| Symbole | Résultat intermédiaire | Chiffre du verrou | Justification |
|---|---:|---:|---|
| Carré | | | |
| Cercle | | | |
| Étoile | | | |
| Triangle | | | |

Résultats attendus :

```text
Carré = 4
Cercle = 6
Étoile = 3
Triangle = 7
```

Les experts Étoile et Triangle terminent leur recherche seulement après avoir reçu les chiffres nécessaires.

---

## 5. Déterminer l'ordre – 7 minutes

Donner les contraintes :

```text
1. Le Triangle vient immédiatement après le Carré.
2. Le Cercle n'est ni en première ni en dernière position.
3. L'Étoile est placée avant le Carré.
```

Les équipes utilisent les jetons-symboles.

Elles doivent établir l'ordre unique :

```text
Étoile – Cercle – Carré – Triangle
```

Le code est donc :

```text
3647
```

---

## 6. Vérification croisée – 8 minutes

Deux équipes comparent une seule carte à la fois.

Questions imposées :

- Comment avez-vous prouvé qu'il y avait 14 carrés ?
- Comment avez-vous retiré les chemins utilisant le passage interdit ?
- Quelles possibilités avez-vous testées pour Étoile ?
- Pourquoi la solution de Triangle est-elle unique ?
- Pourquoi le Cercle ne peut-il pas être en première position ?

Une équipe ne change pas un résultat uniquement parce que l'autre a trouvé autre chose : elle reprend le raisonnement.

---

## 7. Ouverture et défis avancés – 4 minutes

Une équipe qui propose `3647` avec les justifications reçoit le message :

> Coffre ouvert. Les quatre raisonnements étaient nécessaires.

Les groupes rapides commencent :

**Coffre-quatre-verrous-Defis-avances-renforces.md**

---

## 8. Bilan collectif – 3 minutes

Faire distinguer :

- trouver une réponse ;
- organiser une recherche ;
- prouver qu'il n'existe pas d'autre solution ;
- utiliser une information produite par un autre expert.

Synthèse :

> Une énigme est réellement résolue lorsque la réponse est trouvée, vérifiée et justifiée.

---

# Différenciation

## Aide légère

- Carré : fournir les catégories `1 × 1`, `2 × 2`, `3 × 3`.
- Cercle : faire écrire tous les chemins avec trois `D` et deux `B`.
- Étoile/Triangle : fournir un tableau d'essais pour les dizaines et unités.

## Aide intermédiaire

- Carré : donner `9 petits carrés`.
- Cercle : annoncer qu'il existe 10 chemins avant d'interdire le passage.
- Étoile : annoncer qu'il existe deux soustractions donnant 18 avant la contrainte « plus grand nombre pair ».
- Triangle : donner le chiffre des dizaines du plus petit nombre.

## Aide renforcée

Fournir les essais suivants à compléter :

```text
Étoile :
32 − 14 = ...
41 − 23 = ...

Triangle :
72 − 53 = ...
```

L'élève doit encore relier la réponse au symbole et l'expliquer.

---

# Observation de l'enseignant

Observer :

- le classement des carrés ;
- l'exhaustivité du dénombrement de chemins ;
- l'organisation des essais numériques ;
- l'utilisation des résultats des autres ;
- la distinction entre résultat intermédiaire et chiffre du verrou ;
- la justification de l'ordre final ;
- la circulation de la parole.

La réussite attendue est nettement supérieure à la version initiale : chaque groupe doit produire au moins deux raisonnements organisés et deux vérifications.

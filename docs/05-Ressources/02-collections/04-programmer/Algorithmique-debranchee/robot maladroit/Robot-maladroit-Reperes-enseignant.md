---
title: "Le robot maladroit – Repères enseignant"
niveau: "6e"
collection: "Programmer – Algorithmique débranchée"
seance_associee: "S04 – Le robot maladroit"
statut: "Version 1"
---

# Le robot maladroit – Repères enseignant

## Finalité

Cette première séance d'algorithmique débranchée doit faire émerger quatre idées :

1. une tâche est décomposée en instructions simples ;
2. les instructions sont exécutées dans l'ordre ;
3. le robot ne devine jamais l'intention du programmeur ;
4. un programme est testé puis corrigé.

L'objectif n'est pas d'introduire immédiatement un vocabulaire informatique abondant.

---

# Convention de lecture des plateaux

- La flèche indique la position et l'orientation initiales.
- Les cases noires sont interdites.
- L'étoile représente la batterie ou la station finale.
- Les cercles `A` et `B` sont des balises obligatoires.
- `TOURNE` modifie l'orientation sans déplacer le robot.
- `AVANCE` déplace le robot d'une seule case.

---

# Plateaux

## Plateau A

Mission : atteindre la batterie.

Un programme correct possible comporte :

```text
AVANCE
AVANCE
TOURNE À DROITE
AVANCE
AVANCE
TOURNE À GAUCHE
AVANCE
AVANCE
TOURNE À DROITE
AVANCE
STOP
```

Selon la lecture exacte du plateau imprimé, d'autres programmes corrects peuvent exister.

## Plateau B

Mission : passer par `A`, puis `B`, puis atteindre la station.

Avant la séance, exécuter soi-même le plateau imprimé pour vérifier le trajet minimal et noter une solution de référence.

Le but n'est pas d'imposer cette solution, mais de pouvoir :

- vérifier rapidement un programme ;
- identifier un déplacement impossible ;
- accompagner le défi d'efficacité.

---

# Progression des aides

## Aide 1 – Orientation

Demander :

> Dans quelle direction le robot regarde-t-il actuellement ?

Faire tourner physiquement le pion sans le déplacer.

## Aide 2 – Séparer tourner et avancer

Demander à l'élève de mimer :

- une rotation sur place ;
- puis un déplacement d'une case.

## Aide 3 – Tracer le trajet

Autoriser une ligne légère sur le quadrillage, puis demander de traduire chaque changement de direction en instruction.

## Aide 4 – Cartes d'instructions

Fournir des cartes :

```text
AVANCE
TOURNE À DROITE
TOURNE À GAUCHE
STOP
```

Les élèves les ordonnent avant de recopier.

## Aide 5 – Programme partiel

Donner les trois premières instructions correctes et laisser l'équipe poursuivre.

---

# Erreurs fréquentes

## Le robot tourne et avance en même temps

Rappeler :

> Une instruction produit une seule action.

## L'orientation n'est pas mise à jour

Après chaque rotation, faire replacer la flèche du pion.

## Les élèves exécutent l'intention

L'élève jouant le robot corrige spontanément un programme faux.

Rappeler :

> Le robot doit obéir, même si le résultat semble absurde.

## Plusieurs cases pour un seul `AVANCE`

Dans cette séance, `AVANCE` signifie toujours une seule case.

## Le programme n'est pas numéroté

La numérotation facilite l'identification du premier bug.

## Toute la séquence est effacée

Lorsqu'un bug apparaît, faire conserver la première version et modifier seulement les instructions nécessaires.

---

# Débogage : méthode à installer

Quand un programme échoue :

1. repartir du début ;
2. exécuter lentement chaque instruction ;
3. identifier la première instruction après laquelle le robot n'est plus au bon endroit ou dans la bonne direction ;
4. expliquer le bug ;
5. modifier le moins d'instructions possible ;
6. recommencer le test.

Formulation utile :

> On ne corrige pas au hasard. On cherche le premier moment où le programme ne fait plus ce qui était prévu.

---

# Points à observer

| Indicateur | Observation possible |
|---|---|
| Décomposition | L'élève traduit-il le trajet en actions simples ? |
| Ordre | Les instructions sont-elles numérotées et ordonnées ? |
| Orientation | Le sens du robot est-il actualisé après un virage ? |
| Exécution | Le robot suit-il littéralement le programme ? |
| Débogage | L'équipe identifie-t-elle la première erreur ? |
| Correction | La modification est-elle ciblée ? |
| Efficacité | Les élèves comparent-ils la longueur de deux programmes ? |
| Coopération | Les rôles sont-ils réellement répartis ? |

---

# Bilan conseillé

Faire comparer :

- un programme correct mais long ;
- un programme correct plus court ;
- un programme presque correct comportant un seul bug.

Questions :

- Un programme plus court est-il toujours meilleur ?
- Une seule instruction incorrecte peut-elle faire échouer tout le programme ?
- Pourquoi faut-il connaître l'orientation du robot ?
- Que signifie « tester » ?
- Que signifie « déboguer » ?

Synthèse possible :

> Un programme est une suite ordonnée d'instructions précises.  
> Pour le corriger, on cherche la première instruction qui produit un écart.

---

# Prolongements

- Ajouter l'instruction `RÉPÈTE`.
- Interdire les rotations à gauche.
- Écrire un programme pour une autre équipe.
- Concevoir un plateau possédant plusieurs trajets.
- Introduire plus tard les boucles et les conditions.

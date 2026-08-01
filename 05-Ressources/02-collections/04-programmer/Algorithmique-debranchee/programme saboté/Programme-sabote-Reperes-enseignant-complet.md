---
title: "Le programme saboté – Repères enseignant"
niveau: "6e"
collection: "Programmer – Algorithmique débranchée"
seance_associee: "S08 – Le programme saboté"
statut: "Version 1"
---

# Le programme saboté – Repères enseignant

## Finalité

Cette séance approfondit la notion de débogage introduite en S04.

Les élèves doivent distinguer :

- le **bug** : l'instruction incorrecte ou manquante ;
- l'**effet du bug** : la mauvaise position ou orientation ;
- les **conséquences** : toutes les erreurs visibles ensuite.

La priorité est de localiser le premier écart.

---

# Convention

- Le robot part de la case fléchée.
- `AVANCE` signifie une case.
- `TOURNE À DROITE` et `TOURNE À GAUCHE` sont des rotations sur place.
- Les cases noires sont interdites.
- La cible est représentée par une étoile.
- Le trajet attendu est indiqué en pointillés sur les plateaux enseignant ou peut être suivi visuellement.

---

# Défi 1 – Bug simple

## Programme fourni

```text
1. AVANCE
2. AVANCE
3. TOURNE À DROITE
4. AVANCE
5. TOURNE À DROITE
6. AVANCE
7. AVANCE
8. STOP
```

## Bug prévu

L'instruction 5 doit être :

```text
TOURNE À GAUCHE
```

et non :

```text
TOURNE À DROITE
```

## Effet

Le robot s'oriente dans la direction opposée et quitte immédiatement le trajet attendu à l'instruction suivante.

---

# Défi 2 – Mauvaise orientation

## Programme fourni

```text
1. AVANCE
2. TOURNE À GAUCHE
3. AVANCE
4. AVANCE
5. TOURNE À DROITE
6. AVANCE
7. TOURNE À DROITE
8. AVANCE
9. STOP
```

## Bug prévu

L'instruction 2 doit être :

```text
TOURNE À DROITE
```

## Point pédagogique

Les élèves voient que le déplacement faux apparaît à l'instruction 3, mais que la cause se situe à l'instruction 2.

---

# Défi 3A – Instruction en trop

## Programme fourni

```text
1. AVANCE
2. AVANCE
3. TOURNE À DROITE
4. AVANCE
5. AVANCE
6. AVANCE
7. TOURNE À GAUCHE
8. AVANCE
9. STOP
```

## Correction attendue

Supprimer l'une des instructions `AVANCE` successives qui conduit le robot une case trop loin.

Le numéro exact dépend de la présentation finale du plateau. Vérifier avant impression.

---

# Défi 3B – Instruction manquante

## Programme fourni

```text
1. AVANCE
2. TOURNE À DROITE
3. AVANCE
4. AVANCE
5. AVANCE
6. STOP
```

## Correction attendue

Ajouter une rotation avant le dernier déplacement.

Le sens exact dépend du plateau imprimé.

---

# Vérification avant utilisation

Le support SVG est original et les plateaux sont conçus pour faire travailler les types de bugs annoncés.

Avant la première utilisation :

1. imprimer le support ;
2. placer un pion sur chaque départ ;
3. exécuter chaque programme ;
4. noter la correction exacte correspondant à l'orientation imprimée ;
5. ajuster au besoin les programmes dans le fichier Markdown.

Cette vérification est importante, car une rotation dépend toujours de l'orientation initiale et du plateau.

---

# Méthode à installer

Faire utiliser systématiquement un tableau de suivi :

| Étape | Instruction | Case atteinte | Orientation |
|---:|---|---|---|
| départ | — | | |
| 1 | | | |
| 2 | | | |

Quand un écart apparaît :

- revenir à l'étape précédente ;
- vérifier la rotation ;
- distinguer la cause du déplacement faux ;
- modifier une seule chose à la fois.

---

# Progression des aides

## Aide 1 – Matérialiser l'orientation

Utiliser un pion-flèche très visible.

## Aide 2 – Faire verbaliser chaque état

Après chaque instruction :

> Où est le robot ?  
> Dans quelle direction regarde-t-il ?

## Aide 3 – Comparer au trajet attendu

Faire marquer les cases attendues au crayon léger.

## Aide 4 – Réduire la zone de recherche

Dire :

> Le premier bug se trouve entre les instructions 3 et 6.

## Aide 5 – Donner deux choix

Exemple :

> À l'instruction 5, faut-il tourner à droite ou à gauche ?

---

# Erreurs fréquentes

## Corriger la conséquence

Les élèves modifient une instruction tardive alors que le premier bug est antérieur.

## Refaire tout le programme

Rappeler qu'un programme presque correct doit être réparé localement.

## Effacer la première version

La comparaison des versions permet de comprendre la correction.

## Tester seulement à partir du bug

Une correction peut produire un nouvel effet plus tard. Il faut retester depuis le départ.

## Changer plusieurs instructions à la fois

On ne sait plus quelle modification a réellement réparé le programme.

---

# Points à observer

| Indicateur | Observation possible |
|---|---|
| Exécution | Les instructions sont-elles suivies littéralement ? |
| Orientation | Le sens est-il mis à jour après chaque rotation ? |
| Diagnostic | Le premier écart est-il localisé ? |
| Explication | L'équipe distingue-t-elle cause et conséquence ? |
| Correction | La modification est-elle minimale ? |
| Test | Le programme est-il repris depuis le début ? |
| Conservation | Les deux versions sont-elles gardées ? |
| Création | Le bug inventé par l'équipe est-il cohérent ? |

---

# Bilan conseillé

Écrire un exemple :

```text
Instruction 4 : mauvaise rotation
Instruction 5 : mauvais déplacement
Instruction 6 : collision
```

Demander :

> Quel est le bug ?  
> Quelles sont les conséquences ?

Faire émerger :

- le bug est l'instruction 4 ;
- les erreurs observées aux instructions 5 et 6 sont des conséquences.

Synthèse :

> La première erreur explique souvent toutes celles qui suivent.

---


---

# Situations avancées ajoutées à la séance

## Défi 4 – Les deux sabotages

### Plateau

- départ : case en bas à gauche ;
- orientation initiale : nord ;
- cible : case en haut à droite ;
- un obstacle est placé au sud du premier virage attendu ;
- un second obstacle est placé au sud du deuxième virage attendu.

### Programme saboté

```text
1.  AVANCE
2.  AVANCE
3.  TOURNE À DROITE
4.  AVANCE
5.  AVANCE
6.  TOURNE À DROITE
7.  AVANCE
8.  AVANCE
9.  TOURNE À DROITE
10. AVANCE
11. AVANCE
12. TOURNE À DROITE
13. AVANCE
14. AVANCE
15. TOURNE À DROITE
16. AVANCE
17. AVANCE
18. STOP
```

### Premier bug

L'instruction 6 doit être :

```text
TOURNE À GAUCHE
```

Avec `TOURNE À DROITE`, le robot s'oriente vers le sud et rencontre l'obstacle à l'instruction 7.

### Second bug

Après correction de l'instruction 6, le programme progresse jusqu'à l'instruction 12.

L'instruction 12 doit également être :

```text
TOURNE À GAUCHE
```

Avec `TOURNE À DROITE`, le robot s'oriente vers le sud et rencontre le second obstacle à l'instruction 13.

### Programme corrigé

```text
1.  AVANCE
2.  AVANCE
3.  TOURNE À DROITE
4.  AVANCE
5.  AVANCE
6.  TOURNE À GAUCHE
7.  AVANCE
8.  AVANCE
9.  TOURNE À DROITE
10. AVANCE
11. AVANCE
12. TOURNE À GAUCHE
13. AVANCE
14. AVANCE
15. TOURNE À DROITE
16. AVANCE
17. AVANCE
18. STOP
```

### Point pédagogique

Le premier bug empêche physiquement le robot d'atteindre la partie du programme où se trouve le second.

Il faut donc :

1. corriger le premier bug ;
2. recommencer depuis le départ ;
3. poursuivre l'exécution ;
4. découvrir le second bug.

Cette situation montre qu'un programme peut contenir plusieurs erreurs successives.

---

## Défi 5 – Le détour fantôme

### Mission

Le robot part à gauche, orienté vers l'est, et doit rejoindre la cible située cinq cases plus loin.

Le programme atteint bien la cible, mais il comporte un détour inutile.

### Programme fourni

```text
1.  AVANCE
2.  AVANCE
3.  TOURNE À GAUCHE
4.  AVANCE
5.  TOURNE À DROITE
6.  AVANCE
7.  TOURNE À DROITE
8.  AVANCE
9.  TOURNE À DROITE
10. AVANCE
11. TOURNE À DROITE
12. TOURNE À DROITE
13. AVANCE
14. AVANCE
15. AVANCE
16. STOP
```

### Analyse du bloc inutile

Avant l'instruction 3, le robot se trouve sur la troisième case de la ligne du bas et regarde vers l'est.

Les instructions 3 à 12 lui font :

- monter d'une case ;
- avancer d'une case vers la droite ;
- redescendre ;
- revenir à gauche ;
- effectuer les rotations nécessaires pour regarder de nouveau vers l'est.

Après l'instruction 12, le robot se trouve donc :

- sur la même case ;
- dans la même orientation.

Les instructions 3 à 12 peuvent être supprimées sans modifier le résultat final.

### Programme raccourci

```text
1. AVANCE
2. AVANCE
3. AVANCE
4. AVANCE
5. AVANCE
6. STOP
```

### Comparaison

- programme initial : 16 instructions, `STOP` compris ;
- programme raccourci : 6 instructions, `STOP` compris ;
- gain : 10 instructions.

### Point pédagogique

Le programme initial n'est pas faux : il atteint la cible.

Il est cependant inefficace.

Cette situation permet de distinguer :

- **correction** : rendre un programme fonctionnel ;
- **optimisation** : rendre un programme plus court, plus lisible ou plus efficace.


# Prolongements détaillés

## 1. Le bug unique créé par les élèves

### Durée

5 à 10 minutes.

### Consigne

À partir d'un programme correct, l'équipe modifie exactement une instruction :

- remplacer `TOURNE À DROITE` par `TOURNE À GAUCHE` ;
- supprimer un `AVANCE` ;
- ajouter un `AVANCE` ;
- déplacer une rotation.

Une autre équipe doit retrouver la modification.

### Validation

Le défi est valide si :

- le programme original fonctionne ;
- une seule modification a été faite ;
- le bug produit un effet observable ;
- la correction est unique ou clairement justifiée.

---

## 2. Le programme à deux corrections

### Durée

10 à 15 minutes.

### Principe

Proposer un programme qui peut être réparé de plusieurs façons.

Les élèves comparent les solutions.

### Questions

- Quelle correction modifie le moins le programme ?
- Quelle version contient le moins d'instructions ?
- Quelle version est la plus facile à lire ?
- Deux programmes différents peuvent-ils être aussi corrects l'un que l'autre ?

---

## 3. La chaîne de calcul sabotée

### Durée

10 minutes.

### Exemple 1

```text
Départ : 12
+ 8 → × 3 → − 15 → ÷ 5
```

Version affichée :

```text
12 → 20 → 60 → 35 → 7
```

Le premier résultat incorrect est `35`, car :

```text
60 − 15 = 45
```

Les résultats suivants sont des conséquences de cette première erreur.

### Exemple 2

```text
Départ : 25
× 4 → − 30 → ÷ 7 → + 6
```

Version sabotée :

```text
25 → 100 → 70 → 11 → 17
```

Le bug se trouve à l'étape `70 ÷ 7`.

### Objectif

Transférer la méthode :

```text
repérer la première erreur → comprendre son effet → corriger → recalculer la suite
```

---

## 4. Concevoir un plateau-défi

### Durée

20 à 30 minutes.

### Production attendue

Chaque équipe crée :

- un quadrillage de `5 × 5` ou `6 × 6` ;
- une case de départ ;
- une orientation initiale ;
- une cible ;
- deux ou trois obstacles ;
- un trajet correct ;
- un programme saboté contenant un seul bug ;
- une correction réservée à l'enseignant.

### Contraintes

- le trajet doit être réalisable ;
- le programme doit comporter entre 6 et 15 instructions ;
- le bug ne doit pas provoquer une sortie immédiate du plateau ;
- une autre équipe doit pouvoir expliquer précisément la correction.

---

## 5. Introduire les boucles

À utiliser lors d'une séance ultérieure.

### Programme correct

```text
RÉPÈTE 4 FOIS
    AVANCE
    TOURNE À DROITE
```

Le robot trace un carré.

### Bugs possibles

- `RÉPÈTE 3 FOIS` ;
- `TOURNE À GAUCHE` ;
- placer `TOURNE À DROITE` après la boucle ;
- mettre deux fois `AVANCE` dans la boucle ;
- oublier la rotation.

### Idée essentielle

Une erreur placée dans une boucle est répétée plusieurs fois.

---

## 6. Passer à Scratch

À programmer après plusieurs séances d'algorithmique débranchée.

### Transposition possible

Créer un déplacement simple dans Scratch, puis saboter :

- le nombre de pas ;
- l'angle de rotation ;
- l'ordre de deux blocs ;
- le nombre de répétitions ;
- la position initiale ;
- le bloc `s'orienter à`.

### Méthode conservée

```text
1. Lancer le programme.
2. Observer le premier écart.
3. Identifier le bloc responsable.
4. Modifier un seul bloc.
5. Relancer depuis le début.
```

---

## 7. Un programme contenant deux bugs

### Durée

10 à 15 minutes.

Réserver ce défi aux groupes solides.

### Consigne

Le programme contient exactement deux erreurs.

Les élèves doivent :

1. repérer et corriger le premier bug ;
2. retester depuis le début ;
3. repérer le second bug ;
4. conserver les trois versions :
   - programme initial ;
   - programme après la première correction ;
   - programme final.

### Vigilance

Les deux bugs doivent être suffisamment espacés pour que le premier ne rende pas le second impossible à observer.

---

## 8. Correction minimale ou réécriture complète ?

### Situation

Donner un programme long comportant une seule erreur.

Deux élèves proposent :

- de remplacer une instruction ;
- de réécrire tout le programme.

### Débat

- Les deux solutions fonctionnent-elles ?
- Laquelle permet de mieux comprendre le bug ?
- Pourquoi conserver le programme initial ?
- Dans quel cas une réécriture complète pourrait-elle être préférable ?

### Conclusion attendue

Pour apprendre à déboguer, on privilégie d'abord la correction minimale. Une réécriture peut toutefois être utile si le programme est devenu illisible ou inutilement complexe.

---

## 9. Capsule vidéo « Comment déboguer ? »

### Durée

Une séance de communication ultérieure.

### Format

2 à 3 minutes.

### Plan conseillé

1. Présenter le plateau et l'objectif.
2. Lire le programme.
3. Exécuter jusqu'au premier écart.
4. Nommer l'instruction responsable.
5. Expliquer son effet.
6. Montrer la correction minimale.
7. Retester le programme.

### Répartition possible

- un narrateur ;
- un élève qui joue le robot ;
- un contrôleur ;
- un cadreur ou responsable du support.

### Critères

- le bug est clairement visible ;
- l'explication distingue cause et conséquence ;
- la vidéo ne dépasse pas trois minutes ;
- le programme final est testé.

Cette capsule peut rejoindre :

```text
10-Patrimoine-MathLab/
└── Videos/
    └── Algorithmique/
```

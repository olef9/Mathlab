---
title: "S08 – Le programme saboté"
niveau: "6e"
duree: "55 minutes"
periode: "P1 – Entrer dans le Math'Lab"
univers_principal: "Programmer"
collection: "Algorithmique débranchée"
rituel: "CAN-02 – Calculs en chaîne"
competences:
  - Exécuter précisément une suite d'instructions
  - Repérer la première instruction incorrecte
  - Expliquer l'effet d'un bug
  - Corriger un programme en modifiant le moins possible
  - Comparer plusieurs corrections
statut: "Version 1"
---

# S08 – Le programme saboté

## Idée générale

Le robot du Math'Lab reçoit plusieurs programmes déjà écrits, mais certains ont été sabotés.

Les élèves ne doivent pas inventer immédiatement un nouveau trajet. Ils doivent :

1. exécuter le programme exactement ;
2. repérer le premier moment où le robot quitte le trajet attendu ;
3. identifier l'instruction responsable ;
4. proposer une correction minimale ;
5. tester la nouvelle version.

Cette séance prolonge `S04 – Le robot maladroit`, mais elle se concentre sur le **débogage**.

---

# Ressources associées

## Rituel

```text
05-Ressources/
└── 01-Rituels/
    └── Course-aux-nombres/
        └── CAN-02-Calculs-en-chaine.md
```

## Activité principale

```text
05-Ressources/
└── 02-Collections/
    └── Programmer/
        └── Algorithmique-debranchee/
            └── Programme-sabote/
                ├── Programme-sabote-Plateaux.svg
                ├── Programme-sabote-Defis-avances.svg
                ├── Programme-sabote-Fiche-eleve.md
                └── Programme-sabote-Reperes-enseignant.md
```

---

# Mission du jour

> Quelqu'un a modifié les programmes du robot du Math'Lab.  
> Certains trajets contiennent un seul bug, d'autres plusieurs.  
> Votre équipe doit retrouver les erreurs, les expliquer et réparer les programmes sans tout réécrire.

## Instructions disponibles

- `AVANCE`
- `TOURNE À DROITE`
- `TOURNE À GAUCHE`
- `STOP`

## Règles

- Le robot exécute les instructions une par une.
- Il ne devine jamais l'intention du programmeur.
- Dès que le robot n'est plus au bon endroit ou dans la bonne direction, on note le numéro de l'instruction.
- On conserve le programme original.
- On modifie le moins d'instructions possible.
- Toute correction doit être testée du début à la fin.

---

# Organisation

Les élèves travaillent par équipes de trois ou quatre.

Rôles :

- **lecteur** : annonce les instructions ;
- **robot** : déplace le pion ;
- **contrôleur** : compare avec le trajet attendu ;
- **débogueur** : note le bug et la correction.

Les rôles tournent à chaque défi.

---

# Préparation de l'enseignant

## Matériel par équipe

- un exemplaire de `Programme-sabote-Plateaux.svg` ;
- un pion-flèche ;
- une fiche élève ;
- un crayon à papier ;
- une gomme ;
- éventuellement des cartes d'instructions.

## Avant la séance

- imprimer les plateaux en A4 paysage ;
- découper ou préparer un pion orienté ;
- tester les programmes de référence ;
- imprimer le support avancé pour les groupes rapides ;
- prévoir un affichage agrandi d'un défi pour le bilan.

---

# Déroulement détaillé

## 1. Course aux nombres – 5 minutes

Utiliser :

**CAN-02 – Calculs en chaîne**

Correction rapide. Faire verbaliser une stratégie seulement.

---

## 2. Rappel : qu'est-ce qu'un bug ? – 4 minutes

Faire rappeler les idées de S04 :

- une instruction est exécutée dans l'ordre ;
- tourner ne signifie pas avancer ;
- un robot ne corrige pas spontanément ;
- un bug doit être localisé.

Écrire au tableau :

> Le premier bug est la première instruction après laquelle le programme ne correspond plus au trajet attendu.

---

## 3. Défi 1 – Un seul bug visible – 8 minutes

Les équipes utilisent le plateau A et le programme A.

Consigne :

> Exécutez le programme sans rien modifier.  
> Arrêtez-vous au premier écart.  
> Notez le numéro du bug, son effet et une correction possible.

L'objectif est de comprendre la méthode de débogage.

---

## 4. Mise en commun méthodologique – 5 minutes

Comparer les réponses.

Faire formuler la méthode commune :

1. repartir du début ;
2. suivre chaque instruction ;
3. vérifier la position et l'orientation ;
4. arrêter au premier écart ;
5. corriger localement ;
6. retester tout le programme.

---

## 5. Défi 2 – Mauvais virage – 9 minutes

Les équipes utilisent le plateau B.

Le programme conduit presque au bon endroit, mais une rotation est incorrecte.

Les élèves doivent :

- identifier le premier bug ;
- expliquer pourquoi il produit une mauvaise orientation ;
- remplacer une seule instruction ;
- tester la correction.

---

## 6. Défi 3 – Instruction en trop ou instruction manquante – 10 minutes

Les équipes utilisent le plateau C.

Deux versions sont proposées :

- une version comportant une instruction en trop ;
- une version comportant une instruction manquante.

Chaque équipe traite au moins une version.

Question centrale :

> Est-il toujours nécessaire de remplacer une instruction, ou peut-on parfois en supprimer ou en ajouter une ?

---

## 7. Réserve de difficulté – Deux situations avancées – 8 à 15 minutes

Ces situations ne sont pas obligatoires pour toutes les équipes. Elles servent à éviter qu'un groupe rapide termine trop tôt.

Utiliser le support :

**Programme-sabote-Defis-avances.svg**

### Défi 4 – Les deux sabotages

Le programme contient exactement **deux bugs**.

Particularité : le second bug ne peut être observé qu'après correction du premier.

Les élèves doivent conserver trois versions :

1. programme initial ;
2. programme après la première correction ;
3. programme final.

Ils doivent expliquer pourquoi le premier bug cachait le second.

### Défi 5 – Le détour fantôme

Le programme atteint correctement la cible, mais il contient un long détour inutile.

Les élèves doivent :

- repérer le bloc d'instructions inutile ;
- montrer que le robot revient au même endroit dans la même orientation ;
- supprimer ce bloc ;
- comparer la longueur des deux programmes.

Cette situation introduit l'idée d'**efficacité** : un programme peut fonctionner tout en étant inutilement long.

### Gestion possible

- groupe en difficulté : s'arrêter après le défi 2 ou 3 ;
- groupe dans le rythme : traiter seulement le défi 4 ;
- groupe rapide : traiter les défis 4 et 5 ;
- groupe très rapide : créer ensuite un sabotage pour une autre équipe.

---

## 8. Défi facultatif – Créer un bug pour une autre équipe

Chaque équipe choisit un programme correct parmi les défis précédents.

Elle modifie exactement **une instruction** pour produire un bug.

Elle donne ensuite ce programme saboté à une autre équipe, qui doit :

- repérer le bug ;
- expliquer son effet ;
- restaurer le programme.

La modification doit rester raisonnable et vérifiable.

---

## 9. Bilan collectif – 6 minutes

Questions possibles :

- Pourquoi faut-il chercher le premier bug et non la dernière erreur visible ?
- Une erreur de rotation peut-elle provoquer plusieurs erreurs ensuite ?
- Quelle différence existe entre remplacer, ajouter et supprimer une instruction ?
- Pourquoi faut-il conserver la première version ?
- Une correction qui fonctionne est-elle toujours la meilleure ?

Formulation de synthèse :

> Déboguer, ce n'est pas recommencer au hasard.  
> C'est repérer le premier écart, comprendre sa cause et corriger le moins possible.

---

# Trace de fin de séance

```text
Le premier bug du défi choisi se trouvait à l'instruction n° ______.

Cette instruction provoquait :
______________________________________________________

Nous avons corrigé le programme en :
☐ remplaçant une instruction
☐ supprimant une instruction
☐ ajoutant une instruction

Notre correction exacte :
______________________________________________________

Pourquoi faut-il retester depuis le début ?
______________________________________________________

Si nous avons traité un défi avancé :

☐ nous avons corrigé deux bugs successifs ;
☐ nous avons supprimé un détour inutile.

Ce que ce défi nous a appris :
______________________________________________________
```

---

# Différenciation

## Aide légère

Faire utiliser un pion comportant une grande flèche d'orientation.

## Aide intermédiaire

Donner un tableau :

| Instruction | Position | Orientation |
|---:|---|---|
| Départ | | |
| 1 | | |
| 2 | | |
| 3 | | |

## Aide renforcée

- signaler une zone de trois instructions contenant le bug ;
- ou donner le trajet attendu au crayon ;
- ou faire exécuter le programme par l'enseignant très lentement.

## Défi supplémentaire

- trouver deux corrections différentes ;
- prouver laquelle modifie le moins le programme ;
- créer un programme avec exactement deux bugs indépendants ;
- écrire une règle générale pour déboguer ;
- produire une courte démonstration destinée à une future capsule vidéo.

---

# Observation de l'enseignant

Observer notamment :

- l'exécution littérale ;
- la mise à jour de l'orientation ;
- l'identification du premier écart ;
- la distinction entre cause et conséquence ;
- la précision de l'explication ;
- la capacité à corriger localement ;
- la conservation des versions ;
- la qualité du test final.

La réussite ne consiste pas seulement à obtenir un programme correct, mais à être capable d'expliquer précisément ce qui était faux.


---

# Prolongements possibles

## Prolongement immédiat – Le bug unique

Durée : 5 à 10 minutes.

Une équipe écrit un programme correct, puis modifie exactement une instruction.

L'équipe voisine doit :

1. exécuter le programme ;
2. repérer le premier écart ;
3. identifier l'instruction sabotée ;
4. restaurer le programme initial.

Objectif : distinguer clairement le bug de ses conséquences.

## Prolongement différencié – Deux corrections possibles

Durée : 10 minutes.

Proposer un programme qui peut être réparé de deux manières différentes.

Les élèves comparent les corrections selon trois critères :

- nombre d'instructions modifiées ;
- longueur du programme final ;
- facilité de compréhension.

Objectif : comprendre qu'un programme peut être correct sans être le plus efficace.

## Prolongement de création – Concevoir un défi

Durée : 20 à 30 minutes.

Chaque équipe crée :

- un petit plateau ;
- un point de départ orienté ;
- une cible ;
- un programme contenant exactement un bug ;
- une fiche de correction réservée à l'enseignant.

Le défi est ensuite échangé avec une autre équipe.

Objectif : passer de l'exécution à la conception d'un problème algorithmique.

## Prolongement avec les calculs – La chaîne sabotée

Durée : 10 à 15 minutes.

Exemple :

```text
Départ : 8
× 5 → + 7 → ÷ 3 → − 2
```

Une étape ou un résultat est volontairement faux.

Les élèves doivent repérer la première erreur puis corriger la chaîne.

Objectif : transférer la méthode de débogage à une situation numérique.

## Prolongement avec les boucles

À utiliser après l'introduction de l'instruction `RÉPÈTE`.

Exemple :

```text
RÉPÈTE 4 FOIS
    AVANCE
    TOURNE À DROITE
```

Proposer un programme où :

- le nombre de répétitions est faux ;
- une instruction est placée hors de la boucle ;
- la rotation est dans le mauvais sens.

Objectif : préparer les futures séances sur les boucles.

## Prolongement numérique – Passage à Scratch

À utiliser plus tard dans l'année.

Reproduire un des bugs dans Scratch :

- mauvais nombre de pas ;
- mauvaise orientation ;
- bloc placé dans le mauvais ordre ;
- bloc oublié ;
- bloc dupliqué.

Les élèves appliquent la même méthode :

1. exécuter ;
2. observer ;
3. repérer le premier écart ;
4. modifier un seul bloc ;
5. retester.

Objectif : montrer que le débogage appris sans ordinateur reste valable en programmation visuelle.

## Prolongement « Communiquer » – Capsule de débogage

Durée : une séance ultérieure ou un atelier court.

Un groupe prépare une vidéo de 2 à 3 minutes :

1. présentation du programme saboté ;
2. exécution jusqu'au premier bug ;
3. explication de la cause ;
4. correction minimale ;
5. test final.

La vidéo ne doit pas montrer toutes les réponses des autres défis.

Objectif : produire une ressource pour le patrimoine du Math'Lab.

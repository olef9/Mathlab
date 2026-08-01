---
title: "S04 – Le robot maladroit"
niveau: "6e"
duree: "55 minutes"
periode: "P1 – Entrer dans le Math'Lab"
univers_principal: "Programmer"
collection: "Algorithmique débranchée"
rituel: "CAN-01 – Départ express"
competences:
  - Décomposer un déplacement en instructions élémentaires
  - Écrire une suite d'instructions dans un ordre précis
  - Tester un programme et repérer une erreur
  - Corriger et améliorer un programme
  - Coopérer et expliquer une stratégie
statut: "Version 1"
---

# S04 – Le robot maladroit

## Idée générale

Les élèves doivent guider un robot sur un quadrillage en utilisant un nombre limité d'instructions.

Le robot est « maladroit » : il exécute exactement ce qui est écrit, sans deviner l'intention de l'équipe. Une instruction imprécise ou placée dans le mauvais ordre provoque donc une erreur.

Cette séance introduit l'algorithmique sans ordinateur :

- une action complexe est décomposée en actions simples ;
- l'ordre des instructions est essentiel ;
- un programme doit être testé ;
- une erreur peut être repérée puis corrigée.

---

# Ressources associées

## Rituel

```text
05-Ressources/
└── 01-Rituels/
    └── Course-aux-nombres/
        └── CAN-01-Depart-express.md
```

## Activité principale

```text
05-Ressources/
└── 02-Collections/
    └── Programmer/
        └── Algorithmique-debranchee/
            └── Robot-maladroit/
                ├── Robot-maladroit-Plateaux.svg
                ├── Robot-maladroit-Fiche-eleve.md
                └── Robot-maladroit-Reperes-enseignant.md
```

---

# Mission du jour

> Le robot du Math'Lab doit transporter une batterie jusqu'à la station de recharge.  
> Malheureusement, il n'interprète rien : il exécute chaque instruction exactement comme elle est écrite.  
> Écrivez un programme assez précis pour qu'il atteigne sa destination sans toucher un obstacle.

## Instructions autorisées

- **AVANCE** : avancer d'une case dans la direction du robot ;
- **TOURNE À DROITE** : pivoter d'un quart de tour sans changer de case ;
- **TOURNE À GAUCHE** : pivoter d'un quart de tour sans changer de case ;
- **STOP** : arrêter le programme.

## Règles

- Le robot commence sur la case indiquée et dans le sens de la flèche.
- Il ne peut pas traverser un obstacle.
- Il ne peut pas sortir du quadrillage.
- Il exécute les instructions dans l'ordre.
- L'exécutant ne doit jamais corriger spontanément le programme.
- En cas d'erreur, le programme est arrêté, analysé puis modifié.

---

# Organisation

Les élèves travaillent par équipes de trois ou quatre.

Rôles possibles :

- **programmeur** : écrit les instructions ;
- **robot** : exécute littéralement le programme avec le pion ;
- **contrôleur** : vérifie chaque étape ;
- **rapporteur** : note les erreurs et les corrections.

Les rôles tournent entre les missions.

---

# Préparation de l'enseignant

## Matériel par équipe

- un exemplaire de `Robot-maladroit-Plateaux.svg` ;
- un pion ou une petite flèche en papier ;
- une fiche élève ;
- un crayon à papier ;
- une gomme ;
- éventuellement des cartes d'instructions découpées.

## Avant la séance

- vérifier que le pion tient dans les cases ;
- imprimer les plateaux en A4 paysage ;
- prévoir un exemplaire agrandi pour la mise en commun ;
- rappeler que « tourner » ne signifie pas avancer.

---

# Déroulement détaillé

## 1. Course aux nombres – 5 minutes

Utiliser :

**CAN-01 – Départ express**

Correction très rapide, sans détailler toutes les procédures.

---

## 2. Lancement : le robot trop littéral – 5 minutes

Faire venir un élève volontaire.

Donner volontairement une consigne vague :

> Avance un peu, tourne, puis va jusqu'au tableau.

L'élève ou l'enseignant joue le robot et demande :

- Combien de pas ?
- Dans quel sens faut-il tourner ?
- Quand dois-je m'arrêter ?

Faire émerger l'idée :

> Une machine ne devine pas. Une instruction doit être précise.

Présenter ensuite les quatre instructions autorisées.

---

## 3. Mission 1 – Programmer un trajet simple – 10 minutes

Les équipes travaillent sur le plateau A.

Consigne :

> Écrivez d'abord tout le programme sans déplacer le robot.  
> Ensuite seulement, un autre élève l'exécutera.

Étapes :

1. observer le départ, l'orientation et la cible ;
2. écrire le programme ;
3. confier le programme au « robot » ;
4. arrêter l'exécution dès la première erreur ;
5. corriger le programme.

L'objectif est d'atteindre la batterie.

---

## 4. Mise en commun courte – 5 minutes

Comparer deux programmes corrects.

Questions :

- Les programmes sont-ils identiques ?
- Ont-ils le même nombre d'instructions ?
- Où les erreurs sont-elles apparues ?
- Quelle différence existe entre tourner et avancer ?

Faire écrire au tableau un exemple de programme numéroté.

---

## 5. Mission 2 – Passer par les balises – 14 minutes

Sur le plateau B, le robot doit :

1. passer par la balise `A` ;
2. passer ensuite par la balise `B` ;
3. atteindre la station de recharge ;
4. éviter tous les obstacles.

Les rôles changent.

Les équipes doivent conserver :

- la première version du programme ;
- l'endroit du premier bug ;
- la version corrigée.

Relances possibles :

- Dans quelle direction regarde le robot après ce virage ?
- Ton dessin représente-t-il une rotation ou un déplacement ?
- À quelle instruction le robot quitte-t-il le trajet prévu ?
- Peux-tu supprimer une instruction sans changer le résultat ?
- Deux programmes différents peuvent-ils réussir la même mission ?

---

## 6. Défi d'efficacité – 7 minutes

Lorsque le programme fonctionne :

> Trouvez un programme correct utilisant le moins d'instructions possible.

Les élèves comptent les instructions sans confondre :

- une rotation ;
- un déplacement ;
- l'instruction `STOP`.

Ne pas annoncer immédiatement la longueur minimale.

---

## 7. Bilan collectif – 7 minutes

Faire verbaliser :

- l'importance de l'ordre ;
- la différence entre une intention et une instruction ;
- le rôle du test ;
- la valeur d'une erreur bien repérée ;
- la possibilité de plusieurs programmes corrects.

Introduire le vocabulaire :

- **programme** : suite ordonnée d'instructions ;
- **exécuter** : réaliser les instructions ;
- **bug** : erreur produisant un résultat inattendu ;
- **déboguer** : repérer puis corriger cette erreur.

Formulation de synthèse :

> Programmer, ce n'est pas seulement donner des ordres.  
> C'est écrire une suite précise, la tester et la corriger.

---

# Trace de fin de séance

```text
Notre programme de la mission 2 comportait ______ instructions.

Le premier bug se trouvait à l'instruction n° ______.

Ce bug provoquait :
______________________________________________________

Notre correction :
______________________________________________________

Une règle importante pour programmer :
______________________________________________________
```

---

# Différenciation

## Aide légère

Faire placer une petite flèche sur le pion pour conserver son orientation.

## Aide intermédiaire

Permettre aux élèves d'utiliser des cartes d'instructions qu'ils déplacent avant de recopier le programme.

## Aide renforcée

- fournir les trois premières instructions ;
- ou faire tracer au crayon le trajet souhaité avant de le traduire en programme ;
- ou retirer temporairement un obstacle.

## Défi supplémentaire

- interdire `TOURNE À GAUCHE` et demander de réussir uniquement avec des rotations à droite ;
- créer un nouveau parcours pour une autre équipe ;
- écrire un programme contenant volontairement un seul bug ;
- comparer deux programmes et prouver lequel est le plus court.

---

# Observation de l'enseignant

Observer notamment :

- la prise en compte de l'orientation initiale ;
- la distinction entre rotation et déplacement ;
- l'ordre des instructions ;
- la capacité à faire exécuter un programme sans l'interpréter ;
- le repérage précis du bug ;
- la qualité de la correction ;
- la coopération dans la répartition des rôles.

La réussite principale n'est pas d'obtenir le bon trajet au premier essai. Elle réside dans la capacité à tester, localiser une erreur et améliorer le programme.

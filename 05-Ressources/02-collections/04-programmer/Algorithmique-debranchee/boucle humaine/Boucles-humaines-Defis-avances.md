---
title: "Les boucles humaines – Défis avancés"
niveau: "6e"
seance_associee: "S16 – Les boucles humaines"
statut: "Version 1"
---

# Défis avancés

## Défi 1 – Le triangle symbolique

On dispose d'un robot capable d'exécuter :

```text
AVANCE 3
TOURNE DE 120° À GAUCHE
```

Écris une boucle permettant de tracer un triangle équilatéral symbolique.

### Solution

```text
RÉPÈTE 3 FOIS
    AVANCE 3
    TOURNE DE 120° À GAUCHE
FIN DE BOUCLE
```

---

# Défi 2 – Développer une boucle

Développe entièrement :

```text
RÉPÈTE 3 FOIS
    AVANCE 1
    TOURNE À DROITE
    AVANCE 1
FIN DE BOUCLE
STOP
```

## Réponse

```text
AVANCE 1
TOURNE À DROITE
AVANCE 1
AVANCE 1
TOURNE À DROITE
AVANCE 1
AVANCE 1
TOURNE À DROITE
AVANCE 1
STOP
```

Attention : il n'y a pas de séparation automatique entre deux répétitions.

---

# Défi 3 – Deux boucles équivalentes ?

Comparer :

## Programme A

```text
RÉPÈTE 4 FOIS
    AVANCE 1
FIN DE BOUCLE
```

## Programme B

```text
RÉPÈTE 2 FOIS
    AVANCE 2
FIN DE BOUCLE
```

Questions :

- obtiennent-ils la même position finale ?
- exécutent-ils le même nombre de déplacements élémentaires ?
- peut-on les considérer comme équivalents si `AVANCE 2` est une instruction autorisée ?

## Conclusion attendue

Ils atteignent la même position et peuvent être considérés comme équivalents pour ce robot.

---

# Défi 4 – Deux erreurs

Programme prévu pour parcourir un carré de trois cases de côté :

```text
RÉPÈTE 3 FOIS
    TOURNE À DROITE
    AVANCE 2
FIN DE BOUCLE
STOP
```

Il contient exactement deux erreurs.

## Correction

```text
RÉPÈTE 4 FOIS
    AVANCE 3
    TOURNE À DROITE
FIN DE BOUCLE
STOP
```

Erreurs :

- nombre de répétitions ;
- longueur du déplacement.

L'ordre des instructions doit également être discuté selon l'orientation et le point de départ retenus. Avec le départ standard sur un sommet orienté le long du premier côté, `AVANCE` doit précéder `TOURNE`.

---

# Défi 5 – Avant, pendant, après

Le robot doit :

1. prendre une clé au départ ;
2. parcourir un carré ;
3. déposer la clé au retour.

Écris un programme utilisant une seule boucle.

## Solution

```text
PRENDS LA CLÉ
RÉPÈTE 4 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
DÉPOSE LA CLÉ
STOP
```

La prise et le dépôt ne doivent pas être répétés.

---

# Défi 6 – Création

Crée un programme comprenant :

- une instruction avant la boucle ;
- une boucle de deux ou trois instructions ;
- une instruction après la boucle ;
- un nombre de répétitions compris entre 3 et 6 ;
- un trajet vérifiable sur un quadrillage.

Prépare ensuite :

- le plateau ;
- le départ et l'orientation ;
- le programme ;
- la position finale attendue ;
- une version sabotée comportant un seul bug.

Une autre équipe doit tester le défi.

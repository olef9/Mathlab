---
title: "Les boucles humaines – Repères enseignant"
niveau: "6e"
seance_associee: "S16 – Les boucles humaines"
statut: "Version 1"
---

# Repères enseignant – Les boucles humaines

## Place dans la progression

Cette séance prolonge :

- S04 – Le robot maladroit ;
- S08 – Le programme saboté.

Les élèves connaissent déjà :

- l'exécution littérale ;
- l'orientation ;
- l'ordre des instructions ;
- le premier écart ;
- la correction minimale.

La nouveauté est la structure :

```text
RÉPÈTE n FOIS
    séquence
FIN DE BOUCLE
```

---

# Notions essentielles

## Séquence

Suite ordonnée d'instructions.

## Répétition

Nouvelle exécution complète de la séquence.

## Nombre de répétitions

Nombre de fois où la totalité du contenu de la boucle est exécutée.

## Corps de la boucle

Instructions situées entre :

```text
RÉPÈTE
```

et :

```text
FIN DE BOUCLE
```

## Programmes équivalents

Programmes différents produisant le même comportement dans la situation étudiée.

---

# Mission A – Correction

Programme développé :

```text
AVANCE 1
AVANCE 1
AVANCE 1
AVANCE 1
AVANCE 1
STOP
```

Programme comprimé :

```text
RÉPÈTE 5 FOIS
    AVANCE 1
FIN DE BOUCLE
STOP
```

Le programme avec boucle réduit la répétition visuelle, même si le robot exécute toujours cinq déplacements.

---

# Mission B – Correction

Programme :

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
STOP
```

## Après chaque répétition

| Répétition | Position | Orientation |
|---:|---|---|
| 1 | coin inférieur droit | nord |
| 2 | coin supérieur droit | ouest |
| 3 | coin supérieur gauche | sud |
| 4 | coin inférieur gauche | est |

Le robot retrouve donc :

- sa position ;
- son orientation.

---

# Mission C – Correction

Programme :

```text
RÉPÈTE 4 FOIS
    AVANCE 2
    PRENDS LE JETON
    TOURNE À GAUCHE
FIN DE BOUCLE
STOP
```

Le quatrième jeton se trouve sur la case de départ, atteinte après le quatrième déplacement.

## Point pédagogique

Le robot peut revenir sur une case déjà visitée et y réaliser une action nouvelle.

---

# Mission D – Corrections

## D1

Programme incorrect :

```text
RÉPÈTE 3 FOIS
    AVANCE 2
    TOURNE À GAUCHE
FIN DE BOUCLE
```

Après trois répétitions, le robot est au quatrième sommet, orienté vers le sud.

Correction :

```text
3 → 4
```

## D2

Programme incorrect :

```text
RÉPÈTE 4 FOIS
    AVANCE 2
FIN DE BOUCLE
TOURNE À GAUCHE
```

Le robot avance huit cases en ligne droite, puis tourne une seule fois.

Correction :

déplacer la rotation dans le corps de la boucle.

## D3

Programme incorrect :

```text
RÉPÈTE 4 FOIS
    TOURNE À GAUCHE
    AVANCE 2
FIN DE BOUCLE
```

Avec le départ standard orienté vers l'est, le robot tourne d'abord vers le nord. Il parcourt donc un carré décalé par rapport à celui demandé.

Correction :

```text
AVANCE 2
TOURNE À GAUCHE
```

---

# Exécution d'une boucle

Pour éviter les erreurs, le lecteur peut annoncer :

```text
Répétition 1 sur 4.
AVANCE 2.
TOURNE À GAUCHE.
Fin de la répétition 1.

Répétition 2 sur 4.
...
```

Le contrôleur déplace un jeton sur une bande numérotée :

```text
1 – 2 – 3 – 4
```

---

# Aides progressives

## Aide 1 – Surlignage

Colorier chaque occurrence d'une même séquence avec la même couleur.

## Aide 2 – Cartes physiques

Former un paquet représentant le corps de la boucle.

Reposer le paquet au début après chaque répétition.

## Aide 3 – Tableau d'exécution

| Répétition | Instruction | Position | Orientation |
|---:|---|---|---|
| | | | |

## Aide 4 – Développer avant de comprimer

Un élève peut écrire toutes les instructions, puis encadrer le motif.

## Aide 5 – Une seule instruction

Commencer par :

```text
RÉPÈTE 5 FOIS
    AVANCE
```

avant les boucles à plusieurs instructions.

---

# Erreurs fréquentes

## Répéter seulement la dernière instruction

Le robot doit reprendre depuis la première instruction du corps de boucle.

## Oublier la rotation

La répétition des seuls déplacements ne produit pas un polygone.

## Placer une action après la boucle

Elle n'est alors exécutée qu'une fois.

## Confondre nombre de côtés et longueur d'un côté

Dans le carré :

```text
4 = nombre de répétitions
2 = longueur de chaque déplacement
```

## Tourner avant d'avancer

Le trajet peut avoir la même forme mais ne pas occuper les cases demandées.

## Arrêter après avoir atteint visuellement la cible

Le robot doit terminer tout le programme.

---

# Comparer les programmes

Programme développé et programme avec boucle :

- produisent le même trajet ;
- exécutent les mêmes actions ;
- n'ont pas la même longueur écrite ;
- ne sont pas également faciles à modifier.

Pour transformer le carré en hexagone, la boucle rend la modification du nombre de répétitions plus visible.

---

# Défis avancés – Points de vigilance

## Triangle symbolique

Le robot doit accepter une rotation de `120°`.

Sur le quadrillage habituel, cette rotation n'est pas réalisable exactement. Le défi est conceptuel ou doit être exécuté avec une corde formant un triangle.

## Deux boucles équivalentes

La notion d'équivalence dépend du langage autorisé.

Si `AVANCE 2` est une commande primitive, les deux programmes peuvent être comparés directement.

## Deux erreurs

Le défi doit être exécuté sur un plateau clairement orienté pour éviter une ambiguïté sur l'ordre `AVANCE` puis `TOURNE`.

## Création

Refuser les défis impossibles à vérifier ou les programmes sans position finale définie.

---

# Prolongements

## Passage futur à Scratch

Traduire :

```text
RÉPÈTE 4 FOIS
    AVANCE 50 PAS
    TOURNE DE 90°
```

Le sens de la boucle reste identique.

## Boucle et pavage

Reproduire une tuile plusieurs fois :

```text
RÉPÈTE 6 FOIS
    TRACE LA TUILE
    DÉPLACE-TOI VERS LA DROITE
```

## Boucle et calcul

Créer une suite numérique par répétition d'une opération.

## Patrimoine Math'Lab

Conserver les meilleurs défis créés dans :

```text
10-Patrimoine-MathLab/
└── Algorithmique/
    └── Boucles/
```

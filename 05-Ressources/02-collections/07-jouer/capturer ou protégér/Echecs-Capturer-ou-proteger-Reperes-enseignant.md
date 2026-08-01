---
title: "Échecs – Capturer ou protéger ? – Repères enseignant"
niveau: "6e"
seance_associee: "S11 – Échecs : capturer ou protéger ?"
statut: "Version 1"
---

# Repères enseignant – Capturer ou protéger ?

## Objectif de la première séance d'échecs

L'objectif n'est pas de conduire une partie complète.

La séance installe quatre réflexes :

1. repérer les attaques ;
2. chercher les défenseurs ;
3. prévoir une reprise ;
4. comparer le bilan matériel.

Les positions sont volontairement réduites. Les rois sont présents pour conserver l'apparence d'une position d'échecs, mais la recherche porte principalement sur les échanges de pièces.

---

# Valeur des pièces

| Pièce | Valeur |
|---|---:|
| Pion | 1 |
| Cavalier | 3 |
| Fou | 3 |
| Tour | 5 |
| Dame | 9 |

Le roi n'a pas de valeur d'échange : sa perte termine la partie.

Préciser que ces valeurs sont approximatives. Une position réelle peut justifier un choix différent, mais elles sont suffisantes pour les situations de la séance.

---

# Position A – La tour oubliée

## Pièces

Blancs :

```text
Roi g1
Fou c4
```

Noirs :

```text
Roi h8
Tour f7
```

Trait aux Blancs.

## Analyse

Le fou placé en `c4` se déplace en diagonale :

```text
c4 – d5 – e6 – f7
```

Il peut donc jouer :

```text
Fxf7
```

La tour n'est pas protégée dans cette position.

Les Blancs gagnent une tour de valeur 5 et conservent leur fou.

## Réponse attendue

Capturer.

## Point pédagogique

Commencer par une situation où la capture est clairement favorable permet d'installer la méthode sans difficulté excessive.

---

# Position B – Le pion empoisonné

## Pièces

Blancs :

```text
Roi g1
Dame d1
```

Noirs :

```text
Roi g8
Tour d8
Pion d7
```

Trait aux Blancs.

## Analyse

La dame blanche peut jouer :

```text
Dxd7
```

Elle gagne un pion de valeur 1.

La tour noire placée en `d8` peut immédiatement répondre :

```text
Txd7
```

Les Blancs perdent alors leur dame de valeur 9.

Bilan :

```text
+1 − 9 = −8
```

## Réponse attendue

Renoncer à la capture.

## Point pédagogique

Une pièce peut sembler offerte alors qu'elle est protégée par une pièce située juste derrière elle.

---

# Position C – Le cavalier attaqué

## Pièces

Blancs :

```text
Roi g1
Cavalier e4
Pions f2 et h2
```

Noirs :

```text
Roi g8
Fou b7
```

Trait aux Blancs.

## Analyse

Le fou noir suit la diagonale :

```text
b7 – c6 – d5 – e4
```

Le cavalier blanc est donc attaqué.

### Coup `f3`

Le pion se place en `f3`.

Un pion blanc attaque en diagonale vers le haut de l'échiquier :

```text
e4 et g4
```

Le pion protège donc le cavalier en `e4`.

Si les Noirs jouent :

```text
Fxe4
```

les Blancs peuvent répondre :

```text
fxe4
```

### Coup `h3`

Le pion placé en `h3` attaque seulement `g4`.

Il ne protège pas `e4`.

## Réponse attendue

Jouer `f3`.

## Point pédagogique

Protéger une pièce ne signifie pas empêcher toute capture. Cela signifie pouvoir reprendre l'attaquant.

---

# Position D – L'échange favorable

## Pièces

Blancs :

```text
Roi g1
Fou d3
```

Noirs :

```text
Roi g8
Tour h7
```

Trait aux Blancs.

## Analyse

Le fou suit la diagonale :

```text
d3 – e4 – f5 – g6 – h7
```

Il peut jouer :

```text
Fxh7+
```

Le signe `+` indique que le roi noir est attaqué.

Le roi noir peut répondre :

```text
Rxh7
```

Dans la notation française utilisée ici, `R` désigne le roi. Pour éviter la confusion avec la tour, faire verbaliser :

> Le roi noir capture le fou en h7.

Bilan matériel :

```text
tour gagnée : +5
fou perdu : −3
bilan : +2
```

## Réponse attendue

La capture est favorable.

## Point pédagogique

Une pièce protégée peut être capturée si l'échange final est avantageux.

---

# Défi E – Deux attaquants contre un défenseur

## Pièces

Blancs :

```text
Roi g1
Tour e1
Dame h4
```

Noirs :

```text
Roi g8
Tour e7
Dame e8
```

Trait aux Blancs.

## Suite

```text
1. Txe7
```

La tour blanche capture la tour noire.

Si les Noirs reprennent :

```text
1... Dxe7
```

la dame blanche peut répondre :

```text
2. Dxe7
```

Bilan :

- Blancs perdent une tour : `−5` ;
- Noirs perdent une tour et une dame : `+5 + 9`.

Bilan net :

```text
+9
```

## Idée

La tour noire possède un défenseur, mais les Blancs disposent de deux attaquants.

---

# Défi F – Quelle pièce capturer ?

## Pièces

Blancs :

```text
Roi g1
Cavalier e5
```

Noirs :

```text
Roi g8
Dame d7
Tour f7
```

Trait aux Blancs.

Le cavalier blanc attaque simultanément :

```text
d7 et f7
```

### Capture de la tour

```text
Cxf7
```

Le roi noir peut répondre :

```text
Rxf7
```

Bilan approximatif :

```text
tour gagnée 5 − cavalier perdu 3 = +2
```

### Capture de la dame

```text
Cxd7
```

La tour noire peut répondre :

```text
Txd7
```

Bilan :

```text
dame gagnée 9 − cavalier perdu 3 = +6
```

## Réponse attendue

Capturer la dame en `d7`.

## Point pédagogique

Lorsque plusieurs captures sont possibles, comparer le bilan final et non seulement la première pièce visible.

---

# Aides progressives

## Aide 1 – Tracer les lignes d'attaque

Autoriser l'élève à suivre les diagonales ou les lignes avec une règle.

## Aide 2 – Déplacer physiquement

Reconstituer la position sur un échiquier.

## Aide 3 – Nommer les défenseurs

Faire entourer la pièce visée puis demander :

> Quelle pièce adverse pourrait capturer l'attaquant sur cette case ?

## Aide 4 – Tableau du bilan

| Blancs gagnent | Blancs perdent | Bilan |
|---:|---:|---:|
| | | |

## Aide 5 – Limiter la suite

Faire analyser seulement :

```text
capture → reprise
```

sans chercher d'autres coups.

---

# Erreurs fréquentes

## Regarder uniquement la pièce capturée

Faire systématiquement demander :

> Et ensuite, que peut jouer l'adversaire ?

## Confondre attaquée et perdue

Une pièce attaquée peut être déplacée ou protégée.

## Croire qu'une pièce protégée est intouchable

La position D montre qu'un échange peut rester favorable.

## Utiliser la valeur du roi

Le roi ne peut pas être échangé comme une pièce ordinaire.

## Un joueur confirmé donne directement la réponse

Lui confier la responsabilité d'expliquer :

- la ligne d'attaque ;
- la reprise ;
- le bilan.

---

# Prolongements

## Création d'une position

Les élèves rapides créent une position comportant :

- deux rois ;
- entre trois et six autres pièces ;
- une capture tentante ;
- une reprise possible ;
- une décision unique et justifiable.

Ils fournissent :

- la position ;
- la question ;
- la suite principale ;
- le bilan matériel.

## Partie limitée

Lors d'une séance ultérieure, jouer une mini-partie avec :

- roi ;
- trois pions ;
- une tour ou un fou.

Après chaque capture, le joueur doit annoncer :

> Cette pièce est-elle protégée ?

## Patrimoine Math'Lab

Conserver les meilleures positions créées dans :

```text
10-Patrimoine-MathLab/
└── Echecs/
    └── Positions-defis/
```

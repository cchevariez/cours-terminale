---
tags:
  - sciences/terminale-bac-pro
  - fiche-methode
---

# Fiche méthode : Notation scientifique

## Introduction

En sciences, il est fréquent de travailler avec des nombres très grands ou très petits. La notation scientifique est un moyen de simplifier l'écriture et les calculs avec ces nombres.

## 1. Qu'est-ce que la notation scientifique ?

Un nombre écrit en notation scientifique est de la forme :
$$N = a \times 10^{n}$$
où :
- $a$ est un nombre réel tel que $1 \leq |a| < 10$.
- $n$ est un entier relatif (positif ou négatif).

**Exemples :**
- $5000$ s'écrit $5 \times 10^{3}$ en notation scientifique.
- $0,0072$ s'écrit $7,2 \times 10^{-3}$ en notation scientifique.

> [!exercice] Exercice 1
> Écrire les nombres suivants en notation scientifique :
> 1. $123\,000$
> 2. $0,00056$
> 3. $45$
> 4. $0,89$
> 5. $7\,890\,000$

## 2. Passer d'une écriture décimale à la notation scientifique

**Méthode :**
1. Identifier la position de la virgule dans le nombre initial.
2. Déplacer la virgule pour obtenir un nombre $a$ tel que $1 \leq |a| < 10$.
3. Compter le nombre de positions $n$ que la virgule a été déplacée :
   - Si on déplace la virgule vers la gauche, $n$ est positif.
   - Si on déplace la virgule vers la droite, $n$ est négatif.
4. Écrire le nombre sous la forme $a \times 10^{n}$.

**Exemple : convertir $0,000345$ en notation scientifique**
- Déplacer la virgule pour avoir un nombre entre 1 et 10 : $3,45$
- La virgule a été déplacée de 4 positions vers la droite, donc $n = -4$
- Donc, $0,000345 = 3,45 \times 10^{-4}$

> [!exercice] Exercice 2 — QCM
> Sélectionnez la notation scientifique correcte pour les nombres suivants :
> 1. $67\,800$
>    - A) $6,78 \times 10^{4}$
>    - B) $6,78 \times 10^{5}$
>    - C) $6,78 \times 10^{3}$
>    - D) $0,678 \times 10^{5}$
> 2. $0,0045$
>    - A) $4,5 \times 10^{-2}$
>    - B) $4,5 \times 10^{-3}$
>    - C) $45 \times 10^{-4}$
>    - D) $0,45 \times 10^{-2}$

## 3. Opérations avec des nombres en notation scientifique

### 3.1. Multiplication

Pour multiplier deux nombres en notation scientifique :
$$(a \times 10^{n}) \times (b \times 10^{m}) = (a \times b) \times 10^{n+m}$$

**Exemple :** $(2 \times 10^{3}) \times (3 \times 10^{4}) = 6 \times 10^{7}$

### 3.2. Division

Pour diviser deux nombres en notation scientifique :
$$\dfrac{a \times 10^{n}}{b \times 10^{m}} = \left( \dfrac{a}{b} \right) \times 10^{n - m}$$

**Exemple :** $\dfrac{8 \times 10^{5}}{2 \times 10^{2}} = 4 \times 10^{3}$

### 3.3. Addition et soustraction

Pour additionner ou soustraire des nombres en notation scientifique :
1. S'assurer que les exposants de 10 sont identiques.
2. Additionner ou soustraire les coefficients $a$.

**Exemple :** $(5 \times 10^{3}) + (3 \times 10^{3}) = (5 + 3) \times 10^{3} = 8 \times 10^{3}$

Si les exposants sont différents, il faut les ajuster :
$$(2 \times 10^{4}) + (3 \times 10^{3}) = (2 \times 10^{4}) + (0,3 \times 10^{4}) = (2 + 0,3) \times 10^{4} = 2,3 \times 10^{4}$$

> [!exercice] Exercice 3
> Calculer les opérations suivantes et donner le résultat en notation scientifique :
> 1. $(6 \times 10^{5}) \times (2 \times 10^{3})$
> 2. $\dfrac{9 \times 10^{6}}{3 \times 10^{2}}$
> 3. $(4 \times 10^{-2}) + (6 \times 10^{-2})$
> 4. $(5 \times 10^{4}) - (2 \times 10^{3})$

## 4. Application en chimie : concentrations molaires et dilutions

La notation scientifique est particulièrement utile en chimie pour exprimer des concentrations molaires et effectuer des dilutions.

### 4.1. Concentration molaire

La concentration molaire $C$ est définie par :
$$C = \dfrac{n}{V}$$
où :
- $n$ est la quantité de matière en moles (mol).
- $V$ est le volume de la solution en litres (L).

**Exemple :** calculer la concentration molaire d'une solution contenant $0,0025$ mol de soluté dans un volume de 500 mL.
- Convertir le volume en litres : $500$ mL $= 0,5$ L
- Calculer $C$ : $C = \dfrac{0,0025}{0,5} = 0,005$ mol/L
- Écrire en notation scientifique : $0,005$ mol/L $= 5 \times 10^{-3}$ mol/L

> [!exercice] Exercice 4
> Une solution contient $3 \times 10^{-4}$ mol de soluté dans un volume de 250 mL.
> 1. Convertir le volume en litres.
> 2. Calculer la concentration molaire $C$ en mol/L.
> 3. Exprimer le résultat en notation scientifique.

### 4.2. Dilutions

Lors d'une dilution, la relation entre les concentrations et les volumes avant et après dilution est donnée par :
$$C_{i} \times V_{i} = C_{f} \times V_{f}$$
où :
- $C_{i}$ : concentration initiale
- $V_{i}$ : volume initial
- $C_{f}$ : concentration finale
- $V_{f}$ : volume final

**Exemple :** on souhaite diluer 10 mL d'une solution de concentration $2 \times 10^{-2}$ mol/L pour obtenir une solution de concentration $5 \times 10^{-3}$ mol/L. Quel est le volume final $V_f$ ?
- Appliquer la formule : $C_{i} \times V_{i} = C_{f} \times V_{f}$
- Calculer : $V_{f} = \dfrac{C_{i} \times V_{i}}{C_{f}} = \dfrac{(2 \times 10^{-2}) \times 10 \times 10^{-3}}{5 \times 10^{-3}}$
- Simplifier : $V_{f} = \dfrac{(2 \times 10^{-2}) \times (1 \times 10^{-2})}{5 \times 10^{-3}}$
- Calculer : $V_{f} = \dfrac{2 \times 10^{-4}}{5 \times 10^{-3}} = 0,04$ L
- Convertir en mL : $0,04$ L $= 40$ mL

> [!exercice] Exercice 5
> Vous disposez d'une solution mère de concentration $1 \times 10^{-1}$ mol/L. Vous souhaitez préparer 100 mL d'une solution fille de concentration $2 \times 10^{-2}$ mol/L.
> 1. Calculer le volume $V_i$ de la solution mère à prélever.
> 2. Exprimer le résultat en millilitres.

## 5. Exercices de synthèse

> [!exercice] Exercice 6
> 1. Exprimer les nombres suivants en notation scientifique :
>    - $0,000078$
>    - $6\,500\,000$
>    - $0,32$
> 2. Calculer les opérations suivantes :
>    - $(3 \times 10^{2}) \times (4 \times 10^{-5})$
>    - $\dfrac{9 \times 10^{-6}}{3 \times 10^{-2}}$
>    - $(7 \times 10^{3}) + (2 \times 10^{2})$
> 3. En chimie, on a besoin de préparer 250 mL d'une solution de concentration $5 \times 10^{-3}$ mol/L à partir d'une solution de concentration $2 \times 10^{-2}$ mol/L.
>    - Calculer le volume de solution initiale à prélever.
>    - Quel volume d'eau faut-il ajouter pour obtenir le volume final souhaité ?

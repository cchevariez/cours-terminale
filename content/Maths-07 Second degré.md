---
chapitre: 7
tags:
  - maths/terminale-bac-pro
---

# Second degré

## Définition

> [!definition] Définition — Équation du second degré
> On appelle équation du second degré toute équation de la forme $ax^2+bx+c=0$ où $a,b$ et $c$ sont des nombres et $x$ une inconnue.

> [!definition] Définition — Racine d'une équation
> On appelle racine d'une équation toute valeur de $x$ qui satisfait l'équation $ax^2+bx+c=0$.

> [!exercice] Exercice 1
> Parmi ces équations, identifier les équations du second degré. Si les équations sont du second degré, donner les valeurs de $a,b$ et $c$.
> 1. $6x^2-3x-9=0$
> 2. $3x - 4 =0$
> 3. $2x^2 + 6 =0$
> 4. $-2x^2+6x-9=0$
> 5. $3x^2 +7x = 12$
> 6. $4x^2 -5x +30 = 6x -2$
> 7. $-2x^2 -2x -22 = 3x^2 -2x +12$

## Méthode de résolution

### Méthode graphique

> [!methode] Méthode — Résolution graphique
> Nous allons résoudre graphiquement les équations :
> - $2x^2-5x+2 = 0$
> - $4x^2-12x+9 = 0$
> - $x^2+x+1 = 0$
>
> 1. Dans un premier temps, nous allons construire les représentations graphiques des fonctions :
>    - $f(x) = 2x^2-5x+2$
>    - $g(x) = 4x^2-12x+9$
>    - $h(x) = x^2+x+1$
>
> ![[graphesecdeg.png]]
>
> 2. Résoudre graphiquement les équations :
>    - $2x^2-5x+2 = 0$
>    - $4x^2-12x+9 = 0$
>    - $x^2+x+1 = 0$
>
>    Décrire votre méthode.

### Méthode algébrique

> [!methode] Méthode — Résolution algébrique (discriminant)
> Pour résoudre une équation du type $ax^2+bx+c=0$, il faut dans un premier temps calculer le discriminant noté $\Delta$ tel que $\Delta = b^2 - 4ac$.
> - Si $\Delta < 0$, l'équation n'a pas de solution.
> - Si $\Delta = 0$, alors il y a une racine (solution) qui est $\dfrac{-b}{2a}$.
> - Si $\Delta > 0$, alors il y a deux racines $x_1 = \dfrac{-b + \sqrt{\Delta}}{2a}$ et $x_2 = \dfrac{-b - \sqrt{\Delta}}{2a}$.
>
> 1. Résoudre l'équation $2x^2-5x+2 = 0$.
> 2. Résoudre l'équation $4x^2-12x+9 = 0$.
> 3. Résoudre l'équation $x^2+x+1 = 0$.

> [!exercice] Exercice 2
> Résoudre les équations suivantes :
> 1. $6x^2-3x-9=0$
> 2. $2x^2 + 6 =0$
> 3. $-2x^2+6x-9=0$
> 4. $3x^2 +7x = 12$
> 5. $4x^2 -5x +30 = 6x -2$
> 6. $-2x^2 -2x -22 = 3x^2 -2x +12$

## Exercices

> [!exercice] Exercice 3
> La distance de freinage $d$ d'une voiture dépend de la vitesse d'un véhicule. Elle s'exprime par la relation :
> $$d = 0,007v^2+0,8v$$
> où $v$ désigne la vitesse en km/h et $d$ la distance de freinage en m.
> 1. Calculer la distance $d$ lorsqu'on roule à 90 km/h.
> 2. Résoudre l'équation $0,007v^2+0,8v = 50$.
> 3. Donner une interprétation du résultat obtenu à la question précédente.

> [!exercice] Exercice 4
> Une entreprise produit et vend des composants électroniques. Sa capacité mensuelle de production est comprise entre 2 000 et 18 000 pièces. On suppose que toute la production est commercialisée. $x$ est le nombre de pièces produites, en milliers, les coûts de production sont donnés en fonction de $x$ par $p(x)= 2x^2-26x+102$. Le PVHT d'un composant est de 14 €.
> 1. Exprimer, en fonction de $x$, le CA $c(x)$ de l'entreprise.
> 2. Expliquer pourquoi la fonction $c(x)-p(x)$ traduit la rentabilité correspondant à la fabrication de $x$ milliers de composants électroniques.
> 3. On admet que le bénéfice mensuel de l'entreprise est modélisé par la fonction $f$ définie sur $[2;18]$ par $f(x)=-2x^2+40x-102$ où $x$ est le nombre de milliers de pièces produites. Un tracé de sa courbe représentative est donné ci-dessous.
>
> ![[graphsecond2.png]]
>
>    1. Déterminer graphiquement le seuil de rentabilité.
>    2. Retrouver ce résultat par le calcul en résolvant $f(x)=0$.

---
tags:
  - maths/terminale-bac-pro
  - fiche-methode
---

# Équations de droites et intersections

## Équation de droite

> [!definition] Définition — Équation de droite
> Une équation de droite est une équation permettant de décrire l'ensemble des points appartenant à cette droite. Cette équation est de la forme $y=ax+b$ où $x$ et $y$ sont des coordonnées de point et $a$ et $b$ deux nombres.

> [!exemple] Exemple
> Soit $D$ la droite d'équation $y=0,5x+2$.
>
> ![[droite.png]]
>
> Les points $A$ et $B$ appartiennent à la droite, en effet leurs coordonnées vérifient l'équation de la droite.
> - Pour $A(1;2,5)$ si on remplace $x$ par 1 (abscisse de $A$) dans l'équation on obtient $y=0,5 \times 1+2=2,5$ ce qui correspond à l'ordonnée de $A$.
> - Pour $B(-5;0,5)$ on peut répéter le même raisonnement.
> - $C(2;1)$ n'appartient pas à la droite, en effet si on remplace $x$ par 2 dans l'équation de la droite on obtient $y=0,5 \times 2 + 2 = 3$ ce qui ne correspond pas à l'ordonnée de $C$.

> [!exercice] Exercice 1
> On reprend la droite $D$ d'équation $y=0,5x+2$.
> 1. Le point $D(10;7)$ appartient-il à $D$ ?
> 2. Le point $E(-3;0,5)$ appartient-il à $D$ ?
> 3. Le point $F(-10;-4)$ appartient-il à $D$ ?
> 4. Déterminer le point de $D$ dont l'abscisse est égale à 12.
> 5. Déterminer le point de $D$ dont l'ordonnée est égale à -5.

## Intersection de deux droites

On peut calculer les coordonnées du point d'intersection de deux droites en résolvant un système.

> [!remarque] Remarque
> Si deux droites ont le même coefficient directeur (valeur de $a$), elles sont parallèles. Il n'y a donc pas de point d'intersection.

> [!exemple] Exemple
> Soit $D$ la droite d'équation $y=6x-8$ et $D'$ la droite d'équation $y=-4x+12$. Afin de déterminer le point d'intersection nous allons résoudre le système suivant :
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 6x - 8\\
> y &=& -4x + 12
> \end{array}
> \right.
> $$
> On garde la première ligne telle quelle. Et on remplace le $y$ de la deuxième ligne par l'expression en $x$ de la première.
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 6x - 8\\
> 6x - 8 &=& -4x + 12
> \end{array}
> \right.
> $$
> On garde toujours la première ligne en résolvant l'équation de la deuxième ligne.
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 6x - 8\\
> 10x &=& 20
> \end{array}
> \right.
> $$
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 6x - 8\\
> x &=& 2
> \end{array}
> \right.
> $$
> Puis on injecte la valeur de $x$ dans la première ligne.
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 6 \times 2 - 8\\
> x &=& 2
> \end{array}
> \right.
> $$
> $$
> \left\{
> \begin{array}{r c l}
> y &=& 4\\
> x &=& 2
> \end{array}
> \right.
> $$
> On obtient donc les coordonnées du point d'intersection qui sont $(2;4)$.

> [!exercice] Exercice 2
> Déterminer les coordonnées du point d'intersection des droites suivantes :
> - $D$ : $y=7x-6$ et $D'$ : $y=-2x-7$
> - $D$ : $y=-2,5x-3$ et $D'$ : $y=-7x+12$

---
chapitre: 3
tags:
  - maths/terminale-bac-pro
---

# Statistiques à deux variables

## Activité d'introduction

Les États-Unis sont encore de loin la première puissance économique mondiale. Mais pas pour toujours. L'économie chinoise progresse trois fois plus vite que celle des États-Unis. Résultat : la Chine devrait détrôner les États-Unis en 2032. (Source : L'Expansion)

**Problématique :** Cette prévision est-elle exacte ?

![[usachina.jpg]]

Pour répondre à cette question vous disposez des données suivantes :

| Année | USA — PIB en billion de $ | Chine — PIB en billion de $ |
|---|---|---|
| 2000 | 10,2848 | 1,2053 |
| 2001 | 10,6218 | 1,3322 |
| 2002 | 10,9775 | 1,4619 |
| 2003 | 11,5107 | 1,6499 |
| 2004 | 12,2748 | 1,9417 |
| 2005 | 13,0937 | 2,2686 |
| 2006 | 13,8559 | 2,7298 |
| 2007 | 14,4776 | 3,5231 |
| 2008 | 14,7186 | 4,5584 |
| 2009 | 14,4187 | 5,0594 |
| 2010 | 14,9644 | 6,0397 |
| 2011 | 15,5179 | 7,4924 |
| 2012 | 16,1632 | 8,4616 |
| 2013 | 16,7681 | 9,4906 |
| 2014 | 17,419 | 10,3546 |

1. Représenter sur le même axe l'évolution du PIB américain et chinois.
2. Généralement le PIB d'un pays croît tous les ans. Y a-t-il une ou des exceptions dans le graphique que vous avez construit ? Si oui, donner une explication à ces exceptions.
3. À votre avis le PIB chinois va-t-il dépasser le PIB américain ? (Justifier votre réponse)
4. Construire une méthode de votre cru pour répondre à la problématique.

| Compétences | Capacités |
|---|---|
| **S'approprier** | Comprendre la problématique liée au problème. |
| **Analyser / Raisonner** | Reconnaître les cas où un ajustement linéaire est pertinent.<br>Émettre une hypothèse réaliste en fonction des données. |
| **Réaliser** | Calculer les coordonnées du point moyen $G$.<br>Déterminer l'équation de la droite d'ajustement.<br>Tracer un nuage de points. |
| **Valider** | Valider une hypothèse en utilisant l'ajustement linéaire. |
| **Communiquer** | Répondre à la problématique en utilisant le vocabulaire adéquat. |

## Réaliser

> [!definition] Définition — Statistique à deux variables
> Lorsque l'on étudie conjointement deux caractères quantitatifs, on obtient une série statistique quantitative à deux variables. Les valeurs prises par le premier caractère sont notées $x_1,x_2,\ldots,x_n$ et celles prises par le deuxième caractère sont notées $y_1,y_2,\ldots,y_n$.

> [!remarque] Remarque
> On dit qu'une série est chronologique lorsque l'on étudie les valeurs prises par un caractère au cours du temps.

> [!definition] Définition — Nuage de points
> Dans un repère, l'ensemble des points de coordonnées $(x_i;y_i)$ forment le nuage de points représentant cette série statistique à deux variables.

> [!definition] Définition — Ajustement affine ou régression linéaire par la méthode des moindres carrés
> Effectuer un ajustement affine d'un nuage de points consiste à déterminer une fonction affine $y=ax+b$ dont la droite représentative $d$ passe « au plus près » de tous les points.

> [!remarque] Remarque
> Un tutoriel sur la régression linéaire est disponible sur lms.zone. Vous devez savoir faire les manipulations décrites de façon autonome.

> [!travail] Travail
> En utilisant le tableau des compétences, reprendre les données pour les PIB chinois et américain et répondre à la problématique en utilisant la régression linéaire. Vous répondrez ensuite aux questions d'appropriation et d'analyse suivantes :
> 1. Pour le PIB chinois, votre régression linéaire vous a donné une équation de droite de la forme $y = ax+b$, que représentent $x$ et $y$ dans ce contexte ?
> 2. Par le calcul, déterminer une estimation du PIB américain en 2050. Vous expliquerez les étapes de votre démarche.
> 3. Par le calcul, déterminer une estimation de l'année où le PIB américain aura dépassé 25 billions de dollars. Vous expliquerez les étapes de votre démarche.

## Analyser - raisonner

> [!activite] Activité
> Reprenons l'exemple précédent où l'on étudie la taille d'un bébé en fonction de son âge.
>
> | Âge en mois $(x_i)$ | 3 | 6 | 9 | 12 | 15 |
> |---|---|---|---|---|---|
> | Taille en cm $(y_i)$ | 59 | 65 | 70 | 74 | 77 |
>
> 1. En utilisant ces données, on veut estimer la taille d'un bébé de 17 mois et de 20 mois. Quelle méthode et quels outils utiliseriez-vous pour obtenir cette estimation ?
> 2. Effectuer votre estimation.
> 3. Combien de mois avez-vous ?
> 4. En utilisant les mêmes outils, estimer votre taille. Que constatez-vous ? Trouver une explication.
> 5. Établir une règle permettant de distinguer les cas où la régression linéaire est fonctionnelle.

> [!exercice] Exercice 1
> Voici une série de trois nuages de points. Classer, par pertinence, l'utilisation d'une régression linéaire.
>
> Nuage 1 : ![[nuage1.png]]
> Nuage 2 : ![[nuage2.png]]
> Nuage 3 : ![[nuage3.png]]

## Valider

> [!exercice] Exercice 2
> Reprendre l'activité d'introduction (PIB de la Chine et des USA) et répondre à la problématique en utilisant la régression linéaire.
> 1. Expliquer dans un premier temps votre plan d'action (les étapes de votre démarche).
> 2. Réaliser cette démarche.

> [!exercice] Exercice 3
> Une esthéticienne souhaite proposer à ses clients plusieurs forfaits comprenant dix séances. Elle fait réaliser un sondage afin de connaître le nombre de clients intéressés en fonction du montant du forfait. Les résultats sont présentés dans le tableau ci-dessous.
>
> | Montant du forfait en euros $(x_i)$ | 280 | 300 | 320 | 350 | 370 | 400 | 430 | 460 | 480 | 510 |
> |---|---|---|---|---|---|---|---|---|---|---|
> | Nombre de clients $(y_i)$ | 47 | 44 | 40 | 38 | 35 | 28 | 25 | 22 | 17 | 14 |
>
> 1. Représenter le nuage de points associé à cette série.
> 2. Donner les coordonnées du point moyen $G$.
> 3. Expliquer votre démarche pour estimer le nombre de clients intéressés par un forfait à 540 €.
> 4. Effectuer votre estimation.

> [!exercice] Exercice 4
> Le graphique suivant présente l'évolution du prix d'un paquet de cigarettes.
>
> ![[cigarette.jpg]]
>
> **Problématique :** Quel sera le prix d'un paquet en 2025 ?
>
> 1. Une régression linéaire vous paraît-elle pertinente pour répondre à cette problématique ? Justifier votre réponse.
> 2. Répondre à la problématique.

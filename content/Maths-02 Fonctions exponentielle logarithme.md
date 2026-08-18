---
chapitre: 2
tags:
  - maths/terminale-bac-pro
---

# Fonctions exponentielle logarithme

## Lien avec les suites

> [!activite] Activité
> Un épargnant place un capital $u_1$ de 18 000 € à intérêt composé au taux annuel de 1,5%.
> 1. Calculer la valeur acquise $u_2$ au bout d'un an de placement.
> 2. Calculer la valeur acquise $u_3$ au bout de deux ans de placement.
> 3. Caractériser la suite formée par les valeurs acquises du placement.
> 4. Déterminer la raison $q$ de la suite.
> 5. Quelle équation faudrait-il résoudre afin de déterminer au bout de combien de temps la valeur acquise dépassera 40 000 € ?
> 6. Savez-vous résoudre ce type d'équation ?

## Fonctions exponentielles de base $q$

> [!rituel] Rituel
> Trouver les valeurs à inscrire dans les carrés.
> 1. $2^4 \times 2^5 = 2^\square$
> 2. $\dfrac{2^4}{2^5} = 2^\square$
> 3. $(2^3)^4 = 2^\square$

> [!correction] Correction
> 1. $2^9$
> 2. $2^{-1}$
> 3. $2^{12}$

> [!definition] Définition — Fonction exponentielle de base $q$
> Soit $q$ un nombre strictement positif donné. La suite de terme général $u_n=q^n$ pour tout entier naturel $n$ est une suite géométrique de raison $q$.
>
> La fonction exponentielle de base $q$ est le prolongement de cette suite géométrique à l'ensemble des réels. Elle est définie par $f(x)=q^x$ avec $q>0$.

> [!activite] Activité
> Voici une application GeoGebra permettant de visualiser la fonction $f(x)=q^x$ en fonction de différentes valeurs de $q$.
>
> <iframe src="https://www.geogebra.org/classic/z5yr9xgd?embed" width="800" height="400" allowfullscreen style="border: 1px solid #e4e4e4;border-radius: 4px;" frameborder="0"></iframe>
>
> [Ouvrir l'application GeoGebra](https://www.geogebra.org/classic/z5yr9xgd)
>
> Faire varier la valeur de $q$ et en déduire les propriétés sur les variations de la fonction $f(x)=q^x$.
>
> En faisant le parallèle avec vos connaissances, trouvez-vous ces observations logiques (justifier) ?

> [!exercice] Exercice 1
> Dresser le tableau de variation des fonctions suivantes :
> 1. $f(x)= 0,5^x$
> 2. $f(x)= 1,5^x$
> 3. $f(x)= 1^x$

> [!rituel] Rituel
> Résoudre les équations suivantes :
> 1. $6x+3=15$
> 2. $4(x+6) = 11$

> [!correction] Correction
> 1. $6x=12 \Rightarrow x=2$
> 2. $4x+24=11 \Rightarrow 4x=-13 \Rightarrow x=-13/4$

> [!travail] Travail
> En vous inspirant du programme Python du chapitre précédent, réaliser un programme permettant de résoudre l'équation $1,2^x = 6$. La précision de votre solution doit être au centième (0,01 près).

## Le logarithme népérien

John Neper (1550-1617) est un mathématicien écossais. À son époque, l'astronomie, la navigation et le commerce demandaient d'effectuer des opérations de plus en plus complexes. Il a eu l'idée géniale de transformer la multiplication en addition (plus simple à calculer) en utilisant une fonction. Il nomma cette fonction logarithme et la nota $\ln$.

> [!propriete] Propriété
> Soit $a$ et $b$ deux nombres strictement positifs alors :
> $$\ln(a \times b) = \ln(a) + \ln(b)$$

> [!activite] Activité
> Utiliser la propriété précédente sur les expressions suivantes :
> 1. $\ln(a^4) =$
> 2. $\ln(a^n) =$
> 3. $\ln(\dfrac{1}{a}) =$
> 4. $\ln(a) - \ln(b) =$
> 5. $7\ln(a) =$

> [!exercice] Exercice 2
> Résoudre les équations suivantes :
> 1. $1,2^x=6$
> 2. $1200\times1,02^x = 2000$


> ![[resolution_equation_logarithme.mp4]]

> [!exercice] Exercice 3
> Vous placez un capital de 20 000 euros au taux annuel de 1,8%.
> 1. Caractériser la suite formée par votre valeur acquise au fil des années.
> 2. Calculer votre valeur acquise au bout de 7 années de placement.
> 3. **Problématique :** Vous désirez savoir combien de temps il vous faut pour atteindre une valeur acquise supérieure à 26 000 euros.
>    1. Traduire la problématique sous la forme d'une équation.
>    2. Résoudre l'équation obtenue.
>    3. Répondre à la problématique.

> [!rituel] Rituel
> Développer les expressions suivantes :
> 1. $A = -4(6x+3)$
> 2. $B = (x-4)(6x+3)$

> [!correction] Correction
> 1. $A=-24x-12$
> 2. $B = 6x^2 + 3x -24x -12 = 6x^2 -21x -12$

> [!travail] Travail
> Votre conseiller financier vous propose deux placements :
> - Placement A : Capital de base 10 000 euros avec un taux annuel de 1,2%
> - Placement B : Capital de base 14 000 euros avec un taux annuel de 0,8%
>
> **Problématique :** Vous désirez savoir à partir de quand la valeur acquise du placement A devient supérieure à celle du placement B.
>
> Contraintes : pour ce travail, vous n'avez pas le droit à un outil numérique pour la partie réaliser. En revanche votre partie valider devra contenir une validation faisant appel à GeoGebra ou un tableur.

> [!travail] Travail
> Reprendre le TP précédent et modifier le programme Python du TP4 pour répondre à la problématique. Vous recopierez votre code ci-dessous.
>
> [Vidéo d'aide pour le TP6](https://youtu.be/wxjvZh4okL0)
>
> Code du TP4 :
> ```python
> raison = 1.2
> objectif = 6
>
> precision = 0.01
> x = 0
>
> while raison**x < objectif:
>   print(x, "-", raison**x)
>   x = x + 0.01
>
> print("Objectif atteint pour x = ", x)
> ```


> [!exercice] Exercice 4
> 1. Quelles sont les deux propriétés fondamentales du logarithme ?
> 2. À quoi sert le logarithme ?
> 3. Résoudre $5,4^{x-1} = 1250$. Commenter vos opérations à chaque ligne.
> 4. On vous propose deux placements :
>    - Placement A : Capital 1200 € taux annuel 1,2%
>    - Placement B : Capital 1700 € taux annuel 0,9%
>
>    Écrire la partie analyser correspondant à ce problème.
> 5. Résoudre l'équation correspondant au problème précédent.

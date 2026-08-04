---
chapitre: 4
tags:
  - maths/terminale-bac-pro
---

# Statistiques à deux variables — Régressions et modèles non linéaires

## Droite de régression

En première, nous avons étudié les statistiques à deux variables. La méthode utilisée était la droite de régression. Cette droite, passant au plus près des données, permettait d'extrapoler un phénomène et ainsi de donner un modèle prévisionnel. Mais ce modèle n'est pas sans failles :

> [!definition] Définition — Coefficient de détermination $R^2$
> Le coefficient de détermination $R^2$ est un indice permettant de juger de la qualité d'une régression. Si cet indice est proche de 1 alors la régression est de bonne qualité, plus il est proche de 0 moins la qualité de la régression est bonne.

> [!exercice] Exercice 1
> Voici une série de trois nuages de points. Si on fait une régression linéaire sur chacun d'eux, quelles seront à votre avis les valeurs de $R^2$ (proche de 0, proche de 1 ou entre 0 et 1) ?
>
> Nuage 1 : ![[nuage1.png]]
> Nuage 2 : ![[nuage2.png]]
> Nuage 3 : ![[nuage3.png]]

> [!travail] Travail
> Voici l'évolution du CA d'Amazon depuis 2004 (année 1).
>
> ![[caamazon.png]]
>
> **Problématique :** On souhaiterait obtenir une estimation de l'année où le CA d'Amazon dépassera le PIB actuel de la France, soit 2920 milliards de dollars.
>
> 1. Dans GeoGebra, tracer le nuage de points correspondant à l'évolution du CA d'Amazon. Donner les principales étapes de cette réalisation.
> 2. Effectuer une régression linéaire et noter la valeur de $R^2$. Donner les principales étapes de cette réalisation.
> 3. Donner un avis critique sur cette régression.
> 4. Sous GeoGebra, choisir la régression ayant la meilleure qualité en justifiant votre choix.
> 5. Donner une estimation du CA d'Amazon en 2030.
> 6. Répondre à la problématique.

## Exercice simple de rappel : régression linéaire

On étudie l'évolution des ventes annuelles (en milliers d'unités) d'un modèle de voiture entre 2015 et 2020 :

| Année | 2015 | 2016 | 2017 | 2018 | 2019 | 2020 |
|---|---|---|---|---|---|---|
| Ventes (milliers) | 120 | 133 | 149 | 160 | 178 | 192 |

> [!exercice] Exercice 2
> 1. Réalisez la régression linéaire avec GeoGebra. Indiquez l'équation obtenue ainsi que la valeur du coefficient $R^2$.
> 2. Qualifiez la qualité de cette régression en interprétant la valeur obtenue de $R^2$.
> 3. Utilisez votre modèle pour estimer :
>    - les ventes attendues pour l'année 2022 ;
>    - l'année à laquelle les ventes atteindraient 250 milliers d'unités.

## Choix du modèle : régression exponentielle

Voici des données réelles concernant la consommation électrique annuelle (en GWh) d'une ville :

| Année | 2010 | 2011 | 2012 | 2013 | 2014 | 2015 |
|---|---|---|---|---|---|---|
| Consommation (GWh) | 50 | 72 | 105 | 150 | 210 | 290 |

> [!exercice] Exercice 3
> 1. Tracez le nuage de points sous GeoGebra et réalisez une régression exponentielle. Justifiez pourquoi ce modèle est préférable au modèle linéaire (utilisez la valeur de $R^2$).
> 2. Avec votre modèle exponentiel, estimez :
>    - la consommation en 2018 ;
>    - l'année où la consommation atteindra 500 GWh.

## Exercices évolués

**Exercice 4 : Comparaison de placements financiers**

Deux investissements sont comparés entre 2010 et 2015 :

| Année | 2010 | 2011 | 2012 | 2013 | 2014 | 2015 |
|---|---|---|---|---|---|---|
| Investissement A (€) | 1000 | 1080 | 1166,4 | 1259,7 | 1360,5 | 1469,4 |
| Investissement B (€) | 1000 | 1070 | 1160 | 1270 | 1380 | 1520 |

**Remarque :** L'investissement A suit une suite géométrique de formule : $U_n = U_1 \times q^{n-1}$.

> [!exercice] Exercice 4
> 1. Réalisez une régression exponentielle pour modéliser l'investissement B et donnez la formule obtenue.
> 2. Déterminez l'année où l'investissement B dépassera l'investissement A.

**Exercice 5 : Comparaison de deux populations de bactéries**

On étudie deux cultures de bactéries :

| Temps (heures) | 0 | 2 | 4 | 6 | 8 | 10 |
|---|---|---|---|---|---|---|
| Population A (millions) | 1 | 2 | 4 | 8 | 16 | 32 |
| Population B (millions) | 1 | 1,8 | 3,5 | 6,8 | 13 | 25 |

**Remarque :** La population A suit une suite géométrique $U_n = U_1 \times q^{n-1}$.

> [!exercice] Exercice 5
> 1. Réalisez une régression exponentielle sur la population B et indiquez la formule obtenue.
> 2. Déterminez au bout de combien d'heures les deux populations atteindront la même taille.

## Fiche Méthode : Statistiques à deux variables

**Objectifs de la fiche**
- Savoir choisir la régression la plus adaptée grâce au coefficient $R^2$
- Maîtriser la régression exponentielle
- Maîtriser la régression logarithmique
- Déterminer le point d'intersection entre une suite géométrique et une régression exponentielle

### Méthode 1 : Choisir la meilleure régression grâce à $R^2$

> [!propriete] Propriété — Règle fondamentale
> Le coefficient de détermination $R^2$ mesure la qualité d'une régression :
> - $R^2$ proche de **1** $\Rightarrow$ régression de **bonne qualité**
> - $R^2$ proche de **0** $\Rightarrow$ régression de **mauvaise qualité**
>
> **Stratégie :** tester plusieurs types de régression et choisir celle dont le $R^2$ est le plus proche de 1.

> [!methode] Méthode — Étapes sous GeoGebra
> 1. Entrer les données dans le tableur.
> 2. Sélectionner les données et créer le nuage de points.
> 3. Tester différentes régressions : ajustement polynomial, ajustement exponentiel, ajustement logarithmique.
> 4. Comparer les valeurs de $R^2$ affichées.
> 5. Choisir la régression avec le $R^2$ le plus élevé.

### Méthode 2 : Régression exponentielle

> [!propriete] Propriété — Quand utiliser une régression exponentielle ?
> La régression exponentielle est adaptée quand les données suivent une **croissance (ou décroissance) de plus en plus rapide**.
>
> **Forme de l'équation :** $y = a \times b^x$ ou $y = a \times e^{kx}$
>
> **Applications typiques :**
> - Croissance de populations
> - Évolution d'investissements avec intérêts composés
> - Propagation de phénomènes (épidémies, viral...)

> [!exemple] Exemple — Croissance d'une population de bactéries
> **Données :**
>
> | Temps (h) | 0 | 1 | 2 | 3 | 4 | 5 |
> |---|---|---|---|---|---|---|
> | Population (milliers) | 2 | 3,2 | 5,1 | 8,2 | 13 | 21 |
>
> **Étape 1 :** Sous GeoGebra, tracer le nuage de points.
>
> **Étape 2 :** Utiliser l'ajustement exponentiel.
>
> **Résultat obtenu :** $y = 2 \times 1,6^x$ avec $R^2 = 0,998$
>
> **Étape 3 :** Utilisation du modèle.
>
> **Question 1 :** Estimer la population à $t = 7$ heures.
>
> **Question 2 :** À quel moment la population atteint-elle 50 milliers ?

### Méthode 3 : Régression logarithmique

> [!propriete] Propriété — Quand utiliser une régression logarithmique ?
> La régression logarithmique est adaptée quand les données suivent une **croissance rapide au début puis de plus en plus lente**.
>
> **Forme de l'équation :** $y = a + b \times \ln(x)$
>
> **Applications typiques :**
> - Apprentissage (progrès rapides au début puis plateaux)
> - Rendements décroissants
> - Phénomènes de saturation

> [!exemple] Exemple — Temps de réponse d'un athlète
> **Données :** évolution du temps de réponse (en ms) après $x$ semaines d'entraînement.
>
> | Semaines | 1 | 2 | 4 | 8 | 16 | 32 |
> |---|---|---|---|---|---|---|
> | Temps (ms) | 300 | 275 | 250 | 225 | 200 | 175 |
>
> **Étape 1 :** Sous GeoGebra, tracer le nuage de points.
>
> **Étape 2 :** Utiliser l'ajustement logarithmique.
>
> **Résultat obtenu :** $y = 300 - 36 \times \ln(x)$ avec $R^2 = 0,995$
>
> **Étape 3 :** Utilisation du modèle.
>
> **Question 1 :** Estimer le temps de réponse après 10 semaines d'entraînement.
>
> **Question 2 :** Au bout de combien de semaines le temps de réponse atteint-il 150 ms ?

### Méthode 4 : Intersection entre suite géométrique et régression exponentielle

> [!propriete] Propriété — Rappel : suite géométrique
> Une suite géométrique de premier terme $U_1$ et de raison $q$ a pour formule :
> $$U_n = U_1 \times q^{n-1}$$

> [!methode] Méthode — Trouver l'intersection
> **Problème :** trouver quand une suite géométrique $U_n = U_1 \times q^{n-1}$ et une régression exponentielle $f(x) = a \times b^x$ se croisent.
>
> **Étapes :**
> 1. Écrire les deux équations :
>    - Suite géométrique : $U_n = U_1 \times q^{n-1}$
>    - Régression exponentielle : $f(x) = a \times b^x$
> 2. Poser l'égalité : $U_1 \times q^{n-1} = a \times b^n$
> 3. Résoudre graphiquement sous GeoGebra : tracer les deux courbes, utiliser l'outil `Intersection` pour trouver le point de croisement.
> 4. Ou résoudre algébriquement en utilisant les logarithmes.

> [!exemple] Exemple complet — Comparaison de deux investissements
> **Situation :**
> - Investissement A (suite géométrique) : $U_1 = 1200$ €, raison $q = 1,05$ (5% par an) $\Rightarrow U_n = 1200 \times 1,05^{n-1}$
> - Investissement B (régression exponentielle obtenue) : $f(x) = 800 \times 1,12^x$
>
> **Question :** à partir de quelle année l'investissement B dépasse-t-il A ?
>
> **Résolution :**
> 1. On pose l'égalité : $1200 \times 1,05^{n-1} = 800 \times 1,12^n$
> 2. Simplification : $\dfrac{1200}{1,05} \times 1,05^n = 800 \times 1,12^n$
> 3. $1142,86 \times 1,05^n = 800 \times 1,12^n$
> 4. $\dfrac{1142,86}{800} = \left(\dfrac{1,12}{1,05}\right)^n$
> 5. $1,4286 = 1,0667^n$
> 6. $\ln(1,4286) = n \times \ln(1,0667)$
> 7. $n = \dfrac{\ln(1,4286)}{\ln(1,0667)} \approx 5,5$
>
> **Conclusion :** l'investissement B dépasse A au bout d'environ **6 ans**.
>
> Sous GeoGebra : tracer $f(x) = 1200 \times 1,05^{x-1}$ et $g(x) = 800 \times 1,12^x$, puis utiliser l'outil Intersection.

> [!exemple] Exemple 2 — Populations de bactéries
> **Situation :**
> - Population A (suite géométrique) : $U_1 = 100$, raison $q = 2$ (doublement chaque heure) $\Rightarrow U_n = 100 \times 2^{n-1}$
> - Population B (régression exponentielle) : $f(x) = 150 \times 1,8^x$
>
> **Question :** à quel moment A dépasse-t-elle B ?

### Résumé : tableau récapitulatif

| Type | Équation | Allure | Utilisation |
|---|---|---|---|
| Linéaire | $y = ax + b$ | Droite | Évolution régulière constante |
| Exponentielle | $y = a \times b^x$ | Courbe accélérée | Croissance/décroissance rapide |
| Logarithmique | $y = a + b\ln(x)$ | Courbe qui ralentit | Phénomènes de saturation |

> [!remarque] Remarque — À retenir
> 1. Toujours comparer les $R^2$ pour choisir le meilleur modèle.
> 2. Régression exponentielle : croissance/décroissance qui s'accélère.
> 3. Régression logarithmique : croissance qui ralentit.
> 4. Intersection : poser l'égalité et résoudre avec les logarithmes ou graphiquement.

## Validation des résultats en utilisant Python

En reprenant les données de l'exemple 2 (populations de bactéries), compléter le programme suivant afin de valider votre résultat.

```python
# Suite geometrique
u1 =
q =

u_courant = u1

n =

while u_courant  150*1.8**n :
  print("Population A inferieure a Population B")
  u_courant   q
  n   1

print("La populatoin A a depasse la population B a l heure ", n)
```

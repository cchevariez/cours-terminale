---
chapitre: 13
tags:
  - maths/terminale-bac-pro
---

# Exercices complémentaires

## Suites géométriques

> [!exercice] Exercice 1
> Une boutique de mode lance une campagne publicitaire sur les réseaux sociaux. Le premier jour, la publication est vue par 150 personnes. Chaque jour suivant, le nombre de vues augmente de 40%.
> 1. Montrer que le nombre de vues forme une suite géométrique. Préciser le premier terme $u_1$ et la raison $q$.
> 2. Calculer le nombre de vues au bout de 7 jours.
> 3. Calculer le nombre total de vues sur les 7 premiers jours.

> [!exercice] Exercice 2
> Une chaîne de magasins connaît une croissance de son chiffre d'affaires. En 2024, le chiffre d'affaires mensuel était de 80 000 €. Chaque mois, il augmente de 3%.
> 1. Exprimer le chiffre d'affaires du mois $n$ en fonction de $n$ (où $n=1$ correspond à janvier 2024).
> 2. Calculer le chiffre d'affaires prévu pour décembre 2024.
> 3. Calculer le chiffre d'affaires total de l'année 2024.

> [!exercice] Exercice 3
> Une application mobile de livraison perd des utilisateurs actifs. On observe les données suivantes :
> - Semaine 1 : 12 000 utilisateurs
> - Semaine 2 : 10 800 utilisateurs
> - Semaine 3 : 9 720 utilisateurs
>
> 1. Vérifier que le nombre d'utilisateurs forme une suite géométrique. Calculer la raison $q$.
> 2. Exprimer $u_n$ en fonction de $n$.
> 3. Combien d'utilisateurs actifs restera-t-il à la semaine 8 ?
> 4. En dessous de combien d'utilisateurs l'application ne sera-t-elle plus rentable si le seuil est fixé à 5 000 utilisateurs ?

> [!exercice] Exercice 4
> Un magasin d'électronique propose un plan de financement pour un smartphone à 800 €. Le client peut payer en plusieurs fois avec les conditions suivantes : premier versement de 200 €, puis chaque mois suivant, il paie 90% du montant du mois précédent.
> 1. Calculer les trois premiers versements : $u_1$, $u_2$ et $u_3$.
> 2. Montrer que la suite des versements forme une suite géométrique de raison $q = 0,9$.
> 3. Exprimer $u_n$ en fonction de $n$.
> 4. Calculer le montant du 6ème versement.
> 5. Calculer la somme totale payée sur les 10 premiers versements. Le client aura-t-il remboursé la totalité ?

## Corrections

**Correction exercice 1 :**

1. Cette suite est géométrique car pour passer d'un terme au terme suivant, on multiplie toujours par le même nombre 1,4.
2. Pour calculer le nombre de vues au bout de 7 jours : $u_n = u_1 \times q^{n-1}$, donc $u_7 = 150 \times (1,4)^6 = 1\,129,5$. Au bout de 7 jours, la publication aura environ 1 130 vues.
3. Pour calculer le nombre total de vues sur les 7 premiers jours : $S_n = u_1 \times \dfrac{1-q^n}{1-q}$, donc $S_7 = 150 \times \dfrac{1-(1,4)^7}{1-1,4} = 3\,577,5$. Le nombre total de vues sur les 7 premiers jours est d'environ 3 578 vues.

**Correction exercice 2 :**

1. Le chiffre d'affaires forme une suite géométrique car chaque mois il est multiplié par 1,03. $u_n = u_1 \times q^{n-1}$ avec $u_1 = 80\,000$ et $q = 1,03$, donc $u_n = 80\,000 \times (1,03)^{n-1}$.
2. Pour calculer le chiffre d'affaires de décembre 2024 (mois $n = 12$) : $u_{12} = 80\,000 \times (1,03)^{11} = 110\,720€$.
3. Pour calculer le chiffre d'affaires total de l'année 2024 : $S_{12} = u_1 \times \dfrac{1-q^{12}}{1-q} = 80\,000 \times \dfrac{1-(1,03)^{12}}{1-1,03} = 1\,136\,000€$.

**Correction exercice 3 :**

1. Vérifions que le nombre d'utilisateurs forme une suite géométrique : $\dfrac{u_2}{u_1} = \dfrac{10\,800}{12\,000} = 0,9$ et $\dfrac{u_3}{u_2} = \dfrac{9\,720}{10\,800} = 0,9$. Le quotient est constant, donc $(u_n)$ est géométrique de raison $q = 0,9$.
2. $u_n = u_1 \times q^{n-1} = 12\,000 \times (0,9)^{n-1}$
3. Pour la semaine 8 : $u_8 = 12\,000 \times (0,9)^7 = 12\,000 \times 0,478 = 5\,736$ utilisateurs.
4. Pour trouver quand l'application passera sous les 5 000 utilisateurs : $12\,000 \times (0,9)^{n-1} < 5\,000 \Rightarrow (0,9)^{n-1} < \dfrac{5\,000}{12\,000}$. En résolvant : $n > 9,5$. Donc à partir de la semaine 10, l'application ne sera plus rentable.

**Correction exercice 4 :**

1. Les trois premiers versements : $u_1 = 200€$, $u_2 = 200 \times 0,9 = 180€$, $u_3 = 180 \times 0,9 = 162€$.
2. Le quotient $\dfrac{u_{n+1}}{u_n} = 0,9$ est constant. La suite $(u_n)$ est géométrique de raison $q = 0,9$.
3. $u_n = u_1 \times q^{n-1} = 200 \times (0,9)^{n-1}$
4. Le 6ème versement : $u_6 = 200 \times (0,9)^5 = 200 \times 0,590 = 118€$.
5. Somme des 10 premiers versements : $S_{10} = u_1 \times \dfrac{1-q^{10}}{1-q} = 200 \times \dfrac{1-(0,9)^{10}}{1-0,9} = 200 \times \dfrac{1-0,349}{0,1} = 200 \times 6,51 = 1\,302€$. Le client aura payé 1 302 € sur 10 versements, ce qui est supérieur au prix initial de 800 €.

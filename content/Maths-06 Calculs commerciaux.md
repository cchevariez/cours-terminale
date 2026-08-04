---
chapitre: 6
tags:
  - maths/terminale-bac-pro
---

# Calculs commerciaux

> [!rituel] Rituel
> Répondre aux questions suivantes :
> 1. Déterminer le 20ème terme d'une suite géométrique de premier terme 4 et de raison 1,02.
> 2. Résoudre l'équation $6x-3=44$.

> [!correction] Correction
> 1. $4 \times 1,02^{19} = 5,8$
> 2. $6x-3 = 44 \Rightarrow 6x = 47 \Rightarrow x = 47/6$

## S'approprier : vocabulaire des emprunts

Les investissements sont généralement financés par des emprunts, qui sont ensuite remboursés par annuités ou mensualités. Une annuité est constituée de l'amortissement de l'emprunt (part remboursée) + l'intérêt qui est calculé sur la somme prêtée au cours de la période.

Pour se familiariser avec ce vocabulaire, voici un exemple de remboursement d'un emprunt à amortissement constant.

> [!exemple] Exemple
> Le 1er janvier un emprunt de 20 000 € est contracté auprès de la banque.
> - Durée 4 ans
> - Taux 5%
>
> L'amortissement est constant et l'annuité dégressive :
>
> ![[amor1.png]]
>
> 1. Déterminer comment chaque somme pointée d'une flèche a été calculée.
> 2. À partir de cet exemple nous allons construire les formules de calcul. On note :
>    - $t$ : le taux d'intérêt
>    - $A_n$ : l'amortissement l'année $n$
>    - $C_n$ : le capital restant dû l'année $n$
>    - $I_n$ : le montant des intérêts l'année $n$
>    - $a_n$ : le montant des annuités l'année $n$
>
>    1. Déterminer la formule de $I_n$ en fonction de $C_n$ et de $t$.
>    2. Déterminer la formule de $a_n$ en fonction de $A_n$ et de $I_n$.
> 3. Expliquer ce qu'est une annuité et ce qu'elle représente pour le client d'une banque.
> 4. À votre avis, pourquoi les emprunts à amortissement constant ne sont-ils pas plébiscités par la clientèle d'une banque ?

## Emprunts à annuités constantes

Afin de gérer plus facilement leurs comptes, la clientèle préfère souscrire à un prêt à annuité constante. En voici un exemple :

> [!exemple] Exemple
> Emprunt de 20 000 € contracté auprès de la banque.
> - Durée 4 ans
> - Taux 5%
>
> L'amortissement est variable, l'annuité est constante.
>
> ![[amor2.png]]
>
> 1. Compléter les valeurs manquantes.
> 2. Quelle valeur vous semble sortir de nulle part ?

Pour déterminer l'annuité constante d'un emprunt nous utilisons la formule :
$$a = \dfrac{C \times t}{1-(1+t)^{-n}}$$
- $C$ étant le capital emprunté
- $t$ le taux d'intérêt
- $n$ la durée de placement

> [!exercice] Exercice 1
> À l'aide de cette formule, retrouver le montant de l'annuité de l'exemple précédent.

> [!exercice] Exercice 2
> Écrire une méthode permettant de construire :
> 1. Un tableau de remboursement d'un prêt à amortissement constant.
> 2. Un tableau de remboursement d'un prêt à annuité constante.

## Emprunts et algorithmique

> [!rituel] Rituel
> Répondre aux questions suivantes :
> 1. Résoudre $1,02^x=1,3$.
> 2. Combien faut-il de temps à un placement à 2% par an pour augmenter un capital de 30% ?

> [!correction] Correction
> 1. $x = \ln(1,3)/\ln(1,02) = 13,25$
> 2. Cette situation correspond à la question précédente, il faudra donc 13,25 ans.

Voici un programme Python permettant de dresser un tableau pour des remboursements à amortissements constants.

```python
import numpy as np
# On recueille les donnees aupres de l utilisateur

capital = float(input("Quel est le capital emprunte ? "))
duree = int(input("Quelles est la duree de l'emprunt ? "))
t = float(input("Quel est le taux d'interet ? "))

# On cree les colonnes de donnees (vide - empty pour le moment)

capital_restant_du = np.empty(duree)
interet = np.empty(duree)
amortissement = np.empty(duree)
annuite = np.empty(duree)
valeur_nette = np.empty(duree)

# On initialise la valeur du capital
capital_restant_du[0] = capital

for i in range(duree):
  if i>0:
    capital_restant_du[i] = valeur_nette[i-1]

  interet[i] = capital_restant_du[i]*t/100
  amortissement[i] = capital/duree
  annuite[i] = interet[i] + amortissement[i]
  valeur_nette[i] = capital_restant_du[i]-amortissement[i]
  print("Annee ", i+1, capital_restant_du[i], interet[i], amortissement[i], annuite[i], valeur_nette[i])
```

Ce code est disponible sur lms.zone dans le cours emprunts.

> [!exercice] Exercice 3
> Pour répondre aux questions suivantes, vous pouvez faire des recherches sur internet. Dans le code précédent :
> 1. Quel est le rôle de la fonction `input` ?
> 2. Expliquer la ligne `capital_restant_du[0] = capital`.
> 3. Que fait la fonction `range(duree)` ?
> 4. Expliquer ce que fait la boucle `for` ?

> [!travail] Travail
> On souhaite à présent adapter ce code pour qu'il puisse calculer des tableaux de remboursement à annuités constantes.
> 1. Reprendre le code et entourer les lignes en vert à conserver et en rouge les lignes à modifier.
> 2. Modifier, ci-dessous, les lignes le nécessitant.
> 3. Aller sur replit.com et coder cette version alternative.
> 4. Quelle méthode pouvez-vous utiliser afin de valider l'efficacité de votre programme ?

> [!rituel] Rituel
> Répondre aux questions suivantes :
> 1. Résoudre $6x-4 = 51$.
> 2. Résoudre $1,2^x=2$.

> [!correction] Correction
> 1. $6x-4=51 \Rightarrow 6x = 55 \Rightarrow x = 55/6$
> 2. $1,2^x=2 \Rightarrow x = \ln(2)/\ln(1,2) = 3,8$

> [!exercice] Exercice 4
> On souhaite emprunter 450 000 euros sur 10 ans au taux annuel de 3%.
> 1. Construire et compléter le tableau de remboursement de ce prêt à annuités constantes.
> 2. Vérifier à l'aide de votre programme Python votre tableau.
> 3. Déterminer le coût de ce prêt.

## Taux mensuel équivalent

> [!activite] Activité
> On considère un placement de capital 10 000 euros au taux annuel de 3%.
> 1. Donner le taux mensuel équivalent au taux annuel de 3%.
> 2. Calculer la valeur acquise de votre placement au bout d'un an avec le taux annuel et le taux mensuel.
> 3. Comparer vos deux résultats.

> [!definition] Définition — Fonction exponentielle
> La fonction exponentielle notée $e^x$ ou $\exp(x)$ est la fonction réciproque de la fonction logarithme. On a donc :
> $$e^{\ln(x)} = x$$

> [!exercice] Exercice 5
> Reprenons l'énoncé de l'activité précédente. On considère un placement de capital 10 000 euros au taux annuel de 3%.
> 1. On désire déterminer le taux mensuel équivalent à un taux annuel de 3%. Écrire une équation permettant de résoudre ce problème.
> 2. Résoudre ce problème grâce à l'outil exponentiel.

> [!exercice] Exercice 6
> On considère un placement de capital 10 000 euros au taux annuel de 5%.
> 1. Donner le taux mensuel équivalent au taux annuel de 5%.
> 2. Donner le taux trimestriel équivalent au taux annuel de 5%.
> 3. Donner le taux semestriel équivalent au taux annuel de 5%.

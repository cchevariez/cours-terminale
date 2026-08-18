---
chapitre: 1
tags:
  - maths/terminale-bac-pro
---

# Suites numériques

## S'approprier

| Compétences | Capacités |
|---|---|
| **S'approprier** | Comprendre la problématique liée au problème. |
| **Analyser / Raisonner** | À partir de l'énoncé, identifier la nature d'une suite et ses propriétés.<br>Émettre une hypothèse raisonnable. |
| **Réaliser** | Calculer un terme d'une suite géométrique.<br>Réaliser la somme d'une suite géométrique. |
| **Valider** | Valider une hypothèse en utilisant les propriétés des suites. |
| **Communiquer** | Communiquer les résultats trouvés en utilisant le vocabulaire adéquat. |

> [!rituel] Rituel
> Effectuer les calculs suivants :
> 1. 20% de 510 :
> 2. Quel pourcentage de la classe représente 12 élèves sur une classe en comptant 27 ?
> 3. Si j'augmente un prix de 15% je le multiplie par :

> [!correction] Correction
> 1. $(20/100) \times 510 = 102$
> 2. $(12/27) \times 100 = 44,4\%$
> 3. $1,15$

> [!travail] Travail
> Dans un ordinateur ou un téléphone, les calculs sont effectués par un ou plusieurs processeurs. La puissance est directement proportionnelle au nombre de transistors qui le compose. En 1965, Gordon Moore (co-fondateur d'Intel), a prédit que la puissance des processeurs doublerait tous les deux ans. Cette prédiction s'est révélée exacte et a été appelée la loi de Moore.
>
> ![[cpu.jpg|400]]
>
> En 2015, afin de protéger ses données, une entreprise crypte ces dernières. Pour casser le cryptage, il faut un ordinateur possédant plus de 5000 milliards de transistors. En 2015, les processeurs possédaient 8 milliards de transistors.
>
> **Problématique :** L'entreprise souhaiterait savoir pour combien de temps ses données sont-elles sécurisées ? Votre argumentaire devra être appuyé par une représentation graphique réalisée avec l'outil de votre choix.
>
> 1. **Appropriation :** Déterminer le nombre de transistors en 2017, 2019.
> 2. **Validation :** En demandant à une IA de résoudre ce problème, cette dernière vous propose le programme Python suivant. Vous pouvez exécuter ce code en suivant le lien ci-dessous. Votre travail consiste à commenter ce code (ligne commençant par `#`) afin de comprendre son fonctionnement.
>
> ```python
> #
>
> nb_transistor_initial = 8
> annee_de_depart = 2015
> nb_transistor_cilble = 5000
>
> #
>
> nb_transistor_courant = nb_transistor_initial
> annee_courante = annee_de_depart
>
> #
>
> while nb_transistor_courant < nb_transistor_cilble:
>     nb_transistor_courant = nb_transistor_courant * 2
>     annee_courante = annee_courante + 2
>     print("fichier securise ", annee_courante)
>     print("nb transistors ", nb_transistor_courant)
>
> #
>
> print("Le fichier n est plus securise ", annee_courante)
> print("nb transistors ", nb_transistor_courant)
> ```
>
> Tester en ligne : [console.basthon.fr](https://console.basthon.fr/?script=eNqVj0EKwjAQRfc5xdBurLqIQkFEb-AdSlpHOhCmJUnx-iYlVQlRNGSTmf__-ymF4LZxRrEl6wbTEJMjpeEMB6GYEZtruKMyzs_2clcnho50q9HvaimlEGUa2A2TfwRzFhQhURVyEuocee_JM_LBJ8gVOgrw57cqy3wN-9n1odJzsIm60RC7VXGjric0YLGbDFmEYps4qnc5t_Bi2yDOtqnmj0fPBWGhMKB1MOrJfgX-CXsAyUS28Q)
>
> <iframe src="https://console.basthon.fr/?script=eNqVj0EKwjAQRfc5xdBurLqIQkFEb-AdSlpHOhCmJUnx-iYlVQlRNGSTmf__-ymF4LZxRrEl6wbTEJMjpeEMB6GYEZtruKMyzs_2clcnho50q9HvaimlEGUa2A2TfwRzFhQhURVyEuocee_JM_LBJ8gVOgrw57cqy3wN-9n1odJzsIm60RC7VXGjric0YLGbDFmEYps4qnc5t_Bi2yDOtqnmj0fPBWGhMKB1MOrJfgX-CXsAyUS28Q" width="1000" height="500" style="border:1px solid #e4e4e4;border-radius:4px;" frameborder="0"></iframe>

> [!exercice] Exercice 1
> Une entreprise en 2026 a un CA d'affaire de 650 000 €. Les prévisions de cette entreprise donnent une augmentation du CA de 6% par an.
>
> Problématique : Suivant ce modèle de prévision, l'entreprise souhaiterait déterminer en quelle année son CA sera supérieur à 1,5 millions d'euros.
>
> 1. Déterminer le CA prévisionnel de l'entreprise en 2027 et en 2028.
> 2. Reprendre le code précédent et l'adapter au problème actuel. Recopier le code construit.
> 3. Répondre à la problématique.

## Définitions et propriétés

> [!rituel] Rituel
> Compléter :
> 1. Si on diminue un prix de 15%, on le multiplie par :
> 2. Sachant que le taux de TVA est de 20%, quel est le prix HT d'un article dont le TTC est 47 euros ?
> 3. Résoudre $2x+3=22$

> [!correction] Correction
> 1. $0,85$
> 2. $47/1,2 = 39,17$
> 3. $2x = 19 \Rightarrow x = 19/2 = 9,5$

> [!definition] Définition — Suite géométrique
> Dans une suite géométrique, on passe d'un terme au suivant en multipliant toujours par le même nombre $q$ que l'on appelle raison.
>
> ![[schemageom.png|400]]

> [!propriete] Propriété
> Pour une suite géométrique $(u_n)$ de premier terme $u_1$ et de raison $q$ on a :
> $$u_n = u_1 \times q^{(n-1)}$$

> [!exercice] Exercice 2
> Pour chacune des suites de nombres suivantes, déterminer s'il s'agit d'une suite géométrique. Si oui, préciser la raison $q$ ; si non, justifier pourquoi.
> 1. $2 \ ; \ 6 \ ; \ 18 \ ; \ 54 \ ; \ 162$
> 2. $4 \ ; \ 9 \ ; \ 14 \ ; \ 19 \ ; \ 24$
> 3. $5 \ ; \ 10 \ ; \ 25 \ ; \ 40$

> [!exercice] Exercice 3
> On considère une suite géométrique de raison $1,15$ et de premier terme $u_1 = 4$.
> 1. Déterminer la valeur de $u_{15}$.
> 2. Déterminer la valeur de $u_{30}$.
> 3. Déterminer la valeur de $u_{50}$.

> [!travail] Travail
> Réaliser le tableau suivant :
>
> <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQjRdD0gN8soQLbQGhb7xkXZFy3GMaxKUhtlunTHHLurcmEBiJTBgJJQhHmvCPoBy-aGNZsaC1m6CrB/pubhtml?gid=0&amp;single=true&amp;widget=true&amp;headers=false" width="1000" height="500" style="border:1px solid #e4e4e4;border-radius:4px;" frameborder="0"></iframe>
>
> Une vidéo coup de pouce pour la réalisation de ce tableau est disponible au besoin : [Vidéo — construire le tableau](https://youtu.be/it-xmev2LGE)
>
> À l'aide de votre tableau, conjecturer une propriété permettant de savoir, en fonction des valeurs de $u_1$ et de $q$, si une suite géométrique est croissante ou décroissante. Attention, en bac pro on se limite à l'étude des suites géométriques où le premier terme et la raison sont positifs.

> [!rituel] Rituel
> Répondre aux questions suivantes :
> 1. Développer $A=6(x+3)$
> 2. Développer $B=2x(4x-3)$
> 3. Développer $C=(2x-1)(4x-3)$

> [!correction] Correction
> 1. $A=6x+18$
> 2. $B=8x^2-6x$
> 3. $C=8x^2-6x-4x+3=8x^2-10x+3$

> [!propriete] Propriété
> La somme $S_n$ des $n$ premiers termes d'une suite géométrique de premier terme $v_1$ et de raison $q$ est donnée par la formule :
> $$S_n=v_1 \times \dfrac{1-q^n}{1-q}$$

> [!exercice] Exercice 4
> On considère une suite géométrique de raison $1,02$ et de premier terme $u_1=200$.
> 1. Déterminer la somme des 50 premiers termes de $(u_n)$.

> [!exercice] Exercice 5
> Une entreprise artisanale a vendu 150 pièces lors de sa première année d'activité. Grâce au bouche-à-oreille, ses ventes augmentent de 25% chaque année.
> 1. Justifier que le nombre de pièces vendues chaque année forme une suite géométrique et préciser sa raison.
> 2. Déterminer le nombre total de pièces vendues au cours des 8 premières années d'activité.

## Analyser-Raisonner-Communiquer

> [!rituel] Rituel
> Résoudre les équations produit nul suivantes :
> 1. $(x-2)(3x+9)=0$
> 2. $(2x+1)(4x-3)+(2x+1)(8x-6)=0$ (factoriser par facteur commun avant de résoudre)

> [!correction] Correction
> 1. Un produit de facteurs est nul si l'un au moins des facteurs est nul :
>    $x-2=0$ ou $3x+9=0$
>    $x=2$ ou $x=-3$
> 2. On reconnaît le facteur commun $(2x+1)$ :
>    $(2x+1)(4x-3)+(2x+1)(8x-6)=(2x+1)\big[(4x-3)+(8x-6)\big]=(2x+1)(12x-9)$
>    $(2x+1)(12x-9)=0 \Rightarrow 2x+1=0$ ou $12x-9=0$
>    $x=-\dfrac{1}{2}$ ou $x=\dfrac{3}{4}$

> [!exercice] Exercice 6
> Un objet coûte actuellement 200 euros. Le taux d'inflation moyen est de 2,2% par an. On suppose que l'inflation se maintiendra à ce taux annuel. On note $P_1$ le prix actuel et $P_n$ le prix de l'objet l'année $n$.
> 1. Déterminer, en justifiant, la nature de la suite $(P_n)$.
> 2. Déterminer le coût de l'objet l'année 5 et l'année 20.
> 3. À l'aide du tableau réalisé dans le TP2, déterminer dans combien d'années le prix de l'article dépassera 300 euros.

> [!travail] Travail
> La vente de matériel informatique par internet affiche en France une croissance moyenne de 20% chaque année depuis 2015. En 2025 le chiffre d'affaires des ventes en ligne est de 2 milliards d'euros. La vente en magasin physique croît quant à elle de 4% par an et son CA est de 8 milliards d'euros.
>
> **Problématique :** En quelle année le CA des ventes en ligne dépassera-t-il celui des ventes en magasin physique ?
>
> Dans votre partie valider, vous reprendrez le programme Python en page 8 et adapterez le code afin de répondre à votre problématique. [Vidéo coup de pouce pour le code](https://youtu.be/zxRllpIaqt8)

> [!exercice] Exercice 7
> Un véhicule acheté neuf au prix de 18 300 € perd 12% de sa valeur par an. On note $P_1$ la valeur de la voiture la première année, $P_2$ sa valeur la deuxième année, etc.
> 1. Déterminer les caractéristiques de cette suite $(P_n)$.
> 2. Déterminer la valeur de la voiture au bout de 5 ans et de 10 ans d'utilisation.
> 3. Déterminer à partir de quelle année la valeur de la voiture est inférieure à la moitié de sa valeur initiale.

> [!rituel] Rituel
> Soit $f$ une fonction définie sur $\mathbb{R}$ par $f(x) = 2x^2 - 3x + 1$.
> 1. Calculer $f(2)$ et $f(-1)$.
> 2. Résoudre l'équation $f(x) = 1$.

> [!correction] Correction
> Question 1 : Calculer $f(2)$ et $f(-1)$.
> - $f(2) = 2(2)^2 - 3(2) + 1 = 8 - 6 + 1 = 3$
> - $f(-1) = 2(-1)^2 - 3(-1) + 1 = 2 + 3 + 1 = 6$
>
> Question 2 : Résoudre l'équation $f(x) = 1$.
> $2x^2 - 3x + 1 = 1 \Rightarrow 2x^2 - 3x = 0 \Rightarrow x(2x-3) = 0$
>
> Donc $x = 0$ ou $x = 3/2$. Les antécédents de 1 par $f$ sont 0 et 3/2.

> [!travail] Travail
> À la naissance de leur premier petit-fils Rémi, des grands-parents décident de lui ouvrir un compte rémunéré à 4,5% dans le but de lui financer son permis de conduire. Actuellement le coût d'un permis est de 1 350 €. Les grands-parents considèrent que ce coût augmentera de 2% par an jusqu'à sa majorité. Quel capital les grands-parents doivent-ils placer à la naissance de leur petit-fils pour qu'à sa majorité Rémi puisse s'offrir son permis ?
> 1. Déterminer une méthode permettant de répondre au problème. Vous préciserez les outils utilisés.
> 2. Répondre à la problématique.

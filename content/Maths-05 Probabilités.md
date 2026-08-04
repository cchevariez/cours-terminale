---
chapitre: 5
tags:
  - maths/terminale-bac-pro
---

# Probabilités

## S'approprier

> [!activite] Activité
> Un voleur vole une carte bleue. Ne connaissant pas le code, il décide tout de même de retirer de l'argent avec cette dernière.
> 1. Sachant qu'un code de carte bleue est composé de quatre chiffres, déterminer quel est le nombre de codes possibles.
> 2. En déduire la probabilité de réussite de ce voleur.
>
> Si vous êtes le genre de personne à cacher d'une main le clavier des distributeurs de banque pour éviter qu'on vous pique votre code secret grâce à une petite caméra planquée dans un coin : bravo ! Mais cela ne suffit plus vraiment car des chercheurs ont mis au point une technique assez simple, à base de caméra thermique, qui permet, simplement en filmant le clavier du distributeur, de deviner le code utilisé par la personne qui vient juste de passer.
>
> ![[thermique.jpg]]
>
> 1. En utilisant cette technique, déterminer quel est le nombre de codes possibles.
> 2. En déduire la probabilité de réussite de ce voleur high-tech.

> [!definition] Définition — Univers
> On appelle univers l'ensemble des issues possibles d'une expérience aléatoire. On appelle aussi cardinal de l'univers le nombre de ces issues.

> [!definition] Définition — Évènement
> Un événement est une partie de l'univers, formée d'une ou de plusieurs issues possibles. On appelle cardinal d'un évènement le nombre de ses issues.

> [!exercice] Exercice 1
> En reprenant ces définitions et l'activité précédente, répondre aux questions suivantes :
> 1. Quel est l'univers dans le cas du voleur n'utilisant pas de caméra ? Quel est le cardinal de cet univers ?
> 2. Même question dans le cas du voleur utilisant une caméra ?

> [!activite] Activité
> À la rentrée scolaire, on fait une enquête dans les classes de terminale baccalauréat professionnel. 30% des élèves ont 17 ans, 45% ont 18 ans et les autres 19 ans et plus. De plus on a déterminé que 3/4 des élèves de 17 ans souhaitent poursuivre en BTS, ainsi que les 2/3 des élèves de 18 ans et la moitié des élèves de 19 ans et plus.
> 1. Compléter l'arbre des issues possibles.
>
> ![[arbre.png]]
>
> 2. On choisit un étudiant au hasard.
>    1. Quelle est la probabilité de choisir un étudiant de 18 ans ayant envie de poursuivre en BTS ?
>    2. Quelle est la probabilité de choisir un étudiant de 17 ans n'ayant pas envie de poursuivre en BTS ?
>    3. Quelle est la probabilité de choisir un étudiant qui souhaite poursuivre en BTS ?
>    4. Quelle est la probabilité de choisir un étudiant de 17 ou 18 ans choisissant de poursuivre en BTS ?

> [!definition] Définition — Intersection
> Soit deux évènements $A$ et $B$. On appelle intersection de l'évènement $A$ et $B$, l'évènement $C$ où $A$ **et** $B$ se réalisent. On note :
> $$C = A \cap B$$

> [!definition] Définition — Union
> Soit deux évènements $A$ et $B$. On appelle union de l'évènement $A$ et $B$, l'évènement $C$ où $A$ **ou** $B$ se réalise. On note :
> $$C = A \cup B$$

> [!definition] Définition — Incompatible
> Soit deux évènements $A$ et $B$. $A$ et $B$ sont dits incompatibles si :
> $$A \cap B = \varnothing$$

> [!definition] Définition — Contraire
> Soit un évènement $A$. On note $\overline{A}$ l'évènement contraire de $A$. On a :
> $$p(\overline{A}) = 1 - p(A)$$

> [!exercice] Exercice 2
> En reprenant les définitions et l'activité précédente, on note :
> - $A$ : on choisit un étudiant de 17 ans.
> - $B$ : on choisit un étudiant de 18 ans.
> - $C$ : on choisit un étudiant de 19 ans et plus.
> - $D$ : on choisit un étudiant qui désire poursuivre en BTS.
> - $E$ : on choisit un étudiant qui ne désire pas poursuivre en BTS.
>
> 1. Exprimer sous forme de phrase $A \cup B$, puis calculer $p(A \cup B)$.
> 2. Exprimer sous forme de phrase $A \cap E$, puis calculer $p(A \cap E)$.
> 3. Exprimer sous forme de phrase $A \cap C$, puis calculer $p(A \cap C)$.
> 4. Exprimer sous forme de phrase $A \cup B \cup C$, puis calculer $p(A \cup B \cup C)$.
> 5. Exprimer sous forme de phrase $\overline{A}$, puis calculer $p(\overline{A})$.
> 6. Exprimer sous forme de phrase $\overline{A \cup B}$, puis calculer $p(\overline{A \cup B})$.

> [!exercice] Exercice 3
> À la sortie d'une rencontre de football opposant Paris à Marseille, des supporters attendent les joueurs pour des autographes. Une première personne sort des vestiaires. On considère l'évènement A « la personne qui sort est un arbitre » et B « la personne qui sort est un joueur de Marseille ».
> 1. Les évènements A et B sont-ils compatibles ?
> 2. Si on considère que seuls des arbitres ou des joueurs peuvent sortir des vestiaires, quel est l'évènement contraire de B ?

> [!propriete] Propriété
> Soit $A$ et $B$ deux événements indépendants alors :
> $$p(A \cap B) = p(A) \times p(B)$$

> [!propriete] Propriété
> Soit $A$ et $B$ deux évènements du même univers alors :
> $$p(A \cup B) = p(A) + p(B) - p(A \cap B)$$

> [!activite] Activité
> Une étude statistique, menée auprès d'un échantillon représentatif de familles concernant l'équipement de cuisine, a donné les résultats suivants :
> - 80% ont un four à micro-ondes
> - 30% ont un lave-vaisselle
> - 15% n'ont ni four à micro-ondes ni lave-vaisselle
>
> On choisit une famille de l'échantillon au hasard. On note $M$ l'évènement « la famille possède un micro-ondes » et $L$ l'évènement « la famille possède un lave-vaisselle ».
> 1. Que représente l'évènement $\overline{M}$ ? Que représente l'évènement $M \cup L$ ?
> 2. Calculer $p(M \cup L)$.

> [!exercice] Exercice 4
> On tire au hasard une carte dans un jeu de 52 cartes.
> 1. Quelle est la probabilité d'obtenir un cœur ?
> 2. Quelle est la probabilité d'obtenir une figure ?
> 3. Quelle est la probabilité d'obtenir une figure qui soit un cœur ?
> 4. En utilisant la formule $p(A \cup B) = p(A) + p(B) - p(A \cap B)$, déterminer quelle est la probabilité d'obtenir un cœur ou une figure.

> [!exercice] Exercice 5
> Les organismes de Sécurité sociale peuvent effectuer des contrôles aléatoires auprès des salariés lorsqu'ils sont en arrêt de travail pour raison médicale. Un médecin, assermenté par la Sécurité sociale, se rend au domicile du malade pour vérifier les raisons de son arrêt. Dans un département, il existe 3 médecins pour 50 000 salariés.
> 1. Le pourcentage de salariés en arrêt de travail est en moyenne de 6%. Combien de salariés sont potentiellement arrêtés pour raison médicale ?
> 2. Si le contrôle par les médecins se fait de façon aléatoire, quelle est la probabilité pour un salarié en arrêt de travail d'être contrôlé si un médecin peut voir 10 salariés par jour ?
> 3. Dans 90% des cas les médecins de la Sécurité sociale confirment l'arrêt de travail prescrit par le médecin traitant. Quelle est la probabilité pour que l'on demande à un salarié de reprendre le travail suite à un contrôle ?

> [!exercice] Exercice 6
> Une gare SNCF possède deux guichets A et B dont l'un au moins des deux est ouvert. On considère les évènements A et B suivants :
> - $A$ : « le guichet A est ouvert »
> - $B$ : « le guichet B est ouvert »
>
> Une étude statistique a permis d'établir les probabilités suivantes : $p(A) = 0,75$ et $p(B) = 0,5$.
> 1. Donner la signification de $A\cup B$ et déterminer $p(A\cup B)$.
> 2. Calculer la probabilité que les deux guichets soient ouverts. On utilisera la formule $p(A \cup B) = p(A) + p(B) - p(A \cap B)$.

> [!exercice] Exercice 7
> **Problématique :** combien faut-il de personnes dans un groupe pour avoir plus de 50% de chance que deux personnes aient le même jour d'anniversaire ? Pour répondre à cette problématique nous ne prendrons pas en compte les années bissextiles et nous considérons que les naissances sont réparties uniformément sur toute l'année.
> 1. Déterminer la probabilité que deux personnes ne soient pas nées le même jour puis en déduire la probabilité que deux personnes soient nées le même jour.
> 2. Déterminer la probabilité que trois personnes ne soient pas nées le même jour puis en déduire la probabilité que trois personnes soient nées le même jour.
> 3. Déterminer la probabilité que quatre personnes ne soient pas nées le même jour puis en déduire la probabilité que quatre personnes soient nées le même jour.
> 4. À l'aide d'un tableur, répondre à la problématique.

> [!exercice] Exercice 8
> L'objectif de cet exercice est de calculer des probabilités concernant la confiance qu'accordent les Français aux médicaments homéopathiques. Voici les résultats d'un sondage téléphonique réalisé auprès de 1 000 personnes entre le 5 et le 11 janvier de l'an dernier :
> - 770 personnes font confiance aux médicaments homéopathiques ;
> - 350 personnes ont utilisé au moins une fois des médicaments homéopathiques ;
> - 80% des personnes ayant utilisé au moins une fois des médicaments homéopathiques leur font confiance.
>
> 1. Compléter ci-dessous le tableau récapitulant les résultats de ce sondage.
>
> ![[tabproba.png]]
>
> 2. On choisit une personne au hasard parmi les personnes interrogées et on considère les deux évènements suivants :
>    - Événement A : « la personne choisie fait confiance aux médicaments homéopathiques » ;
>    - Événement B : « la personne choisie n'a jamais utilisé de médicaments homéopathiques ».
>
>    1. Calculer la probabilité $P(A)$ de l'événement A et la probabilité $P(B)$ de l'événement B.
>    2. Définir par une phrase l'événement contraire de l'événement A, noté $\overline{A}$.
>    3. Calculer la probabilité $p(\overline{A})$.
>    4. Trois traductions de l'événement C « la personne choisie ne fait pas confiance aux médicaments homéopathiques ou n'en a jamais utilisé » sont proposées ci-dessous :
>       - cet événement est traduit par $A \cap B$
>       - cet événement est traduit par $A \cup \overline{B}$
>       - cet événement est traduit par $\overline{A} \cup B$
>
>       Recopier la seule proposition exacte.
>    5. Calculer la probabilité $p(\overline{A}\cap B)$.
>    6. En déduire la probabilité de l'évènement C.

> [!exercice] Exercice 9
> Une entreprise fabrique 20 000 sièges pour voitures par an dans deux usines. La production de l'usine A est de 12 000 sièges par an et celle de l'usine B, 8 000 sièges par an. Des contrôles qualité ont montré que 2% des sièges fabriqués dans l'usine A et 1% des sièges fabriqués dans l'usine B sont défectueux. L'objectif de cet exercice est de calculer la probabilité $p$ qu'un siège prélevé au hasard dans la production soit défectueux. On considère les événements suivants :
> - évènement A : « le siège prélevé provient de l'usine A »
> - évènement B : « le siège prélevé provient de l'usine B »
> - évènement D : « le siège prélevé est défectueux »
>
> 1. Calculer la probabilité $p(A)$.
> 2. Définir en une phrase l'évènement $\overline{D}$.
> 3. Donner la probabilité $p_1$ pour que le siège prélevé soit défectueux s'il provient de l'usine A.
> 4. Compléter l'arbre des probabilités ci-dessous.
>
> ![[arbreproba.png]]
>
> 5. Calculer la probabilité $p$ qu'un siège prélevé au hasard soit défectueux.

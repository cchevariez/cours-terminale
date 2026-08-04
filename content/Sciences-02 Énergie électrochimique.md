---
chapitre: 2
tags:
  - sciences/terminale-bac-pro
---

# Énergie électrochimique

> [!activite] Activité — Comprendre les indications sur une batterie
> Voici la description de la batterie pour vélo « PowerTube Vertical BOSCH ».
>
> ![[battvelo.jpg]]
>
> Les caractéristiques :
> - Type de montage : dans le cadre
> - Tension : 36 V
> - Capacité : 20 Ah
> - Quantité d'énergie : 720 Wh
> - Masse : 4,4 kg
> - Temps de recharge : recharge à 50% en env. 2,1 h / recharge à 100% en env. 6 h
>
> 1. Donner le symbole et l'unité des différentes grandeurs de cette documentation.
> 2. La formule de la quantité d'énergie ($E$) est : $E = U \times Q$. À l'aide des informations sur la batterie, vérifier cette égalité.
> 3. Cette batterie est reliée à un moteur ayant une puissance $P = 500$ W.
>    1. Que signifie le symbole $W$ ?
>    2. On rappelle la formule $P = U \times I$. Déterminer l'intensité que doit délivrer la batterie afin de faire fonctionner le moteur.
>    3. En supposant que l'utilisateur ne fournit aucun effort, quel sera le temps d'utilisation de cette batterie avant que cette dernière ne soit vide ?
>    4. À présent, l'utilisateur fournit une puissance de 200 W, déterminer l'autonomie de la batterie.

## Grandeurs et formules

$$Q = I \times t$$

L'unité légale pour la capacité est le coulomb (C) : $1\text{Ah} = 3600\text{C}$.

**Convertir** la capacité de la batterie « PowerTube Vertical BOSCH » en coulomb.

$$E = U \times Q = U \times I \times t$$

## La pile

C'est en 1800 que les prémices de la pile électrique apparaissent dans le monde. En effet, le savant physicien italien, Alessandro Volta, s'intéresse de près aux expériences menées par Luigi Galvani en 1786.

Luigi Galvani testait la machine de Ramsden, une machine conçue vers 1768, pour générer des étincelles mécaniquement à l'aide d'une manivelle, sur les cadavres de grenouilles. Cette machine produisait des petits sursauts au niveau des muscles des cadavres.

Alessandro Volta décide d'aller plus loin dans ces recherches. Pensant que l'empilage de différents métaux (zinc, cuivre et feutre imbibé d'eau salée) peut produire de l'électricité, il invente alors la pile électrique. La création de la pile électrique est bien là.

Ce procédé est toujours l'actuel procédé qui fait fonctionner nos piles aujourd'hui, à savoir deux extrémités (anode et cathode, ou les électrodes) et le liquide conducteur appelé l'électrolyte.

> [!rituel] Rituel
> Compléter le tableau suivant avec les bonnes unités :
> 1. La tension électrique se mesure en ... avec l'appareil appelé ...
> 2. Une lampe de 60 W branchée sur une tension de 230 V est parcourue par une intensité de ...

> [!correction] Correction
> 1. Volt (V) — voltmètre
> 2. $I = P/U = 60/230 = 0,26$ A

> [!travail] Travail — Fabriquons une pile !
> Matériel :
> - 2 lames de cuivre
> - 1 lame de zinc
> - 1 lame de fer
> - 1 multimètre
> - 2 fils de connexion
> - 2 pinces crocodiles
> - 1 solution de chlorure de sodium saturée
>
> 1. Quel est le nom commun du chlorure de sodium ?
> 2. Réaliser le montage ci-dessous :
>
> ![[pileA.png]]
>
> 3. Dans cette position, que mesure le multimètre ?
> 4. Interchanger les lames afin de compléter le tableau suivant :
>
> ![[pileB.png]]
>
> 5. Dans quelles expériences peut-on parler de pile ?
> 6. Vos mesures sont-elles en accord avec la classification électrochimique ci-dessous ?
>
> ![[pileC.png]]
>
> 7. La lame de fer correspond-elle toujours à l'électrode négative ? Justifier votre réponse.

> [!rituel] Rituel
> 1. Une batterie a une capacité de 3000 mAh. Exprimer cette capacité en Ah.
> 2. Un radiateur électrique de 2000 W fonctionne pendant 3 heures. Calculer l'énergie consommée en kWh.

> [!correction] Correction
> 1. $3000$ mAh $= 3$ Ah
> 2. $E = P \times t = 2000 \text{ W} \times 3 \text{ h} = 6000$ Wh $= 6$ kWh

## Vocabulaire

Une pile est un convertisseur électrochimique constitué de trois éléments :
- Une électrode positive : la cathode
- Une électrode négative : l'anode
- Un électrolyte liquide ou gel contenant des ions

Une pile effectue une transformation d'énergie chimique en énergie électrique. La réaction produite est irréversible et limitée à la quantité d'ions présents dans l'électrolyte.

L'anode, ou borne négative, subit une oxydation (perte d'électrons) tandis que la cathode subit une réduction (gain d'électrons).

> [!activite] Activité
> Reprenons le TP précédent dans le cas d'une pile Zinc/Fer.
> 1. Que se passe-t-il au niveau de l'électrode de zinc ? Écrire la demi-équation correspondante.
> 2. Que se passe-t-il au niveau de l'électrode de fer ? Écrire la demi-équation correspondante.
> 3. Identifier l'anode et la cathode (justifier).

## L'oxydoréduction

### Notions d'oxydant et de réducteur

> [!definition] Définition — Réducteur
> Un réducteur est une espèce chimique capable de libérer un ou plusieurs électrons.

> [!exemple] Exemple
> $$Zn \rightarrow Zn^{2+} + 2e^{-}$$
> $$Cu \rightarrow Cu^{2+} + 2e^{-}$$
> $$Ag \rightarrow Ag^{+} + e^{-}$$

Quand une espèce subit une réduction, elle est mise en contact avec un réducteur. Une réduction est donc un gain d'électrons (qui ont été donnés par le réducteur).

> [!definition] Définition — Oxydant
> Un oxydant est une espèce chimique capable de capter un ou plusieurs électrons.

> [!exemple] Exemple
> $$Zn^{2+} + 2e^{-} \rightarrow Zn$$
> $$Cu^{2+} + 2e^{-} \rightarrow Cu$$
> $$Ag^{+} + e^{-} \rightarrow Ag$$

Quand une espèce subit une oxydation, elle est mise en contact avec un oxydant. Une oxydation est donc une perte d'électrons (qui ont été pris par l'oxydant).

> [!rituel] Rituel
> 1. Dans une pile, la borne positive est appelée ..., et la borne négative est appelée ...
> 2. Une pile de 1,5 V débite un courant de 0,5 A pendant 2 heures. Calculer l'énergie fournie en Wh.

> [!correction] Correction
> 1. Borne + : cathode — Borne − : anode
> 2. $E = P \times t = U \times I \times t = 1,5 \text{ V} \times 0,5 \text{ A} \times 2 \text{ h} = 1,5$ Wh

### Couples oxydant/réducteur

On peut toujours associer un réducteur avec un oxydant : ces deux espèces forment un « couple oxydant/réducteur ».

> [!exemple] Exemple
> Voici quelques exemples de couples :
> - couple cuivre : $Cu^{2+}/Cu$
> - couple zinc : $Zn^{2+}/Zn$
> - couple argent : $Ag^{+}/Ag$

Une réaction d'oxydoréduction est une réaction entre deux couples. Un couple va subir une réduction et l'autre une oxydation.

> [!exercice] Exercice 1
> Répondre par vrai ou faux.
> 1. Une réduction est un gain d'électrons.
> 2. Une espèce chimique capable de céder des électrons est un réducteur.
> 3. Les ions cuivre (II) ($Cu^{2+}$) et le métal fer ($Fe$) constituent un couple oxydant/réducteur.

> [!exercice] Exercice 2 — Classification électrochimique
> ![[miniclass.png]]
>
> 1. Quels sont les couples redox présents dans l'extrait de la classification électrochimique ci-contre ?
> 2. Parmi ces couples, quel est l'oxydant le plus fort ? Le réducteur le plus fort ?
> 3. À l'aide de quel(s) réducteur(s) peut-on réduire l'ion $Cu^{2+}$ ? L'ion $Ag^+$ ?

> [!travail] Travail — La pile de Daniell
> [Visionner la vidéo à partir de la sixième minute](https://www.youtube.com/watch?v=LyPxLJeHbjo)
>
> 1. Légender le schéma de l'expérience décrite. Vous rajouterez les fils du multimètre permettant à ce dernier de mesurer la tension de la pile.
>
> ![[daniell1.png]]
>
> 2. Dans cette pile, identifier l'anode et la cathode (justifier votre réponse).
> 3. Quelle réaction chimique va se produire à la cathode ?
> 4. Quelle réaction chimique va se produire à l'anode ?
> 5. Quels sont les deux couples en jeu dans cette pile ?
> 6. Donner l'équation d'oxydoréduction globale de cette pile.
> 7. Qu'est-ce qu'un électrolyte, et quel est son rôle au sein de cette pile ? Que se passerait-il si on ne disposait pas d'électrolyte ?
> 8. Réaliser l'expérience et mesurer la tension délivrée par cette pile.
> 9. Donner toutes les raisons pour lesquelles cette pile peut arrêter de fonctionner.

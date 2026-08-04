---
tags:
  - maths/terminale-bac-pro
  - sciences/terminale-bac-pro
  - moc
---

# Sommaire — Terminale Bac Pro

Ce vault regroupe le cours de **Mathématiques** et de **Sciences physiques et chimiques** de Terminale Bac Pro. Seul le cours proprement dit est repris ici — les évaluations (CCF, contrôles, corrigés) font l'objet d'un travail séparé, dans un autre dossier.

## Mathématiques

### Chapitres

0. [[Maths-00 Tableau des compétences]]
1. [[Maths-01 Suites numériques]]
2. [[Maths-02 Fonctions exponentielle logarithme]]
3. [[Maths-03 Statistiques à deux variables]]
4. [[Maths-04 Statistiques à deux variables — Régressions et modèles non linéaires]]
5. [[Maths-05 Probabilités]]
6. [[Maths-06 Calculs commerciaux]]
7. [[Maths-07 Second degré]]
8. [[Maths-08 Fonction dérivée]]
9. [[Maths-09 Rappels exp et ln]]
10. [[Maths-10 Étude de fonctions]]
11. [[Maths-11 Prix psychologique]]
12. [[Maths-12 Python — Activité 1]]
13. [[Maths-13 Exercices complémentaires]]

### Fiches méthode

- [[Maths-Fiche Régression à la calculatrice]]
- [[Maths-Fiche Équations de droites et intersections]]

### Contenus du LaTeX source non repris (brouillons/doublons)

Le fichier source `TCA.tex` contenait plusieurs versions successives d'un même chapitre (le professeur ayant retravaillé son cours sans supprimer les anciennes versions). Seule la version la plus aboutie de chaque chapitre a été convertie ; les autres sont signalées ici et laissées en commentaire dans [[Cours complet]] plutôt que d'être omises silencieusement :
- **Fonctions exponentielle logarithme** : un doublon strictement identique au chapitre 2 existait plus loin dans le fichier — ignoré.
- **Statistiques à deux variables** : une version tronquée (s'arrêtant avant les parties Analyser/Valider) existait en plus de la version complète reprise en chapitre 3 — ignorée.
- **Statistiques à deux variables : régressions et modèles non linéaires** : une version partielle, sans la Fiche Méthode ni la validation Python final, existait en plus de la version complète reprise en chapitre 4 — ignorée.
- **Fonction exponentiel et logarithme** : un fragment de 2 activités d'introduction, sans suite — brouillon abandonné, non repris.
- **Suites numériques - Logarithme** : chapitre commencé (rappels + reprise quasi identique du premier TP du chapitre 1) mais qui ne traite en réalité aucun logarithme malgré son titre — brouillon abandonné, non repris.

## Sciences

### Chapitres

1. [[Sciences-01 Combustion]]
2. [[Sciences-02 Énergie électrochimique]]
3. [[Sciences-03 Modes de transfert thermique]]
4. [[Sciences-04 Solutions acido-basiques]]
5. [[Sciences-05 La double dilution]]

### Fiches méthode

- [[Sciences-Fiche Dilution]]
- [[Sciences-Fiche Notation scientifique]]

### Contenus du LaTeX source non repris

- **Combustion** : une version plus ancienne et plus courte de ce chapitre (sans rituels, sans QR codes, sans les exercices complémentaires) existait en double dans `Tsciences.tex` — ignorée au profit de la version aboutie reprise en chapitre 1.
- **Evaluation chimie** : évaluation (CCF), hors périmètre de ce vault.

---

Vue tout-en-un par matière (concaténation des chapitres de cours par transclusion, façon `TCA.tex` / `Tsciences.tex`) : [[Cours complet]]

---

## À propos de ce vault

- **Périmètre** : uniquement le cours (Mathématiques + Sciences). Les évaluations, corrections et brouillons du support LaTeX d'origine sont volontairement laissés de côté, à traiter dans un dossier dédié ultérieurement.
- **Callouts** : chaque environnement du cours (définition, propriété, méthode, exemple, remarque, activité, travail, rituel, exercice, appel) est un callout Obsidian coloré, style *duoton* — voir `.obsidian/snippets/callouts-terminale.css`. L'environnement `appel` (« Appeler votre professeur »), absent du cours de Première, est nouveau à ce niveau.
- **Images** : stockées dans `/Users/cid/Mon Drive/Cours/Images/`, un dossier partagé entre tous les niveaux, relié à ce vault via le lien symbolique `Images/`.
- **Maths et chimie** : rendues nativement par le plugin *Extended MathJax* (la notation chimique `\ce{}` est supportée nativement par MathJax). Les unités `\SI{}{}`/`\si{}` (siunitx, non supportées nativement) ont été converties directement en texte simple lors de la conversion plutôt que laissées sous forme de macro — le cours source les utilisait avec des unités composées (`\si{\mol\per\liter}`) que la macro de compatibilité simple ne sait pas décomposer.
- **Plugins installés** : Latex Suite (raccourcis de saisie), Advanced Tables (édition des tableaux), Extended MathJax (macros).
- **Rituels et QR codes** : les rituels papier de ce cours utilisaient des QR codes encodant soit une correction cachée, soit un lien externe (vidéo, GeoGebra). Les corrections cachées ont été décodées (`zbarimg`) puis reconstituées en callout `[!correction]`, imprimé à l'envers (style « support papier », comme pour Première — il faut retourner la feuille pour lire la réponse) ; les liens externes ont été transformés en liens Markdown cliquables.
- **Doublons résolus** : voir les sections « Contenus du LaTeX source non repris » ci-dessus, pour Mathématiques et Sciences.

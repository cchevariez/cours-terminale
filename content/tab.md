

- Caractériser les suites (en justifiant) 
- Repérer dans l'énoncé les valeurs de $u_1$ et de $q$
- On va utiliser le terme général d'une suite géométrique $u_n=u_1 \times q^{n-1}$ 
- Dans un tableur, on va faire trois colonnes. Une colonne date, une colonne vente en ligne et une colonne vente physique
- On va réaliser le graphique correspondant et cherche le point d'intersection.
- Validation : Pour valider le résultat, on fera un programme Python



# Fiche synthèse : Suites géométriques

Définition : Une suite est géométrique si pour passer d'un terme au terme suivant, on multiplie toujours par le même nombre. Ce nombre est appelé la raison et est noté $q$ 

## Types de problème 

- Déterminer à partir de quel rang une suite atteint une valeur donnée.
	- **Exemple** : On place 1500 euros sur un livret à 2%. Au bout de combien temps, la valeur du livret atteindra 2000 euros.
	- **Analyse** :
		- Caractériser la suite : Donner la nature de la suite (géométrique ou arithmétique) en justifiant. 
		- On va utiliser le **terme général** de la suite : $u_n = u_1 \times q^{n-1}$ 
		- Trois possibilités :
			- Calculer $u_1$, $u_2$, $u_3$ etc... jusqu'à obtenir la valeur désirée (méthode très peu efficace)
			- Utiliser un tableur. En appliquant la formule des suites géométriques.
			- Programme Python avec une boucle while.

```python
# Initialisation des variables
u1 = 1500
q  = 1.02
annee = 2026

# Initialisation des variables courantes
u_courant = u1
annee_courante = annee

# Boucle

while u_courant < 2000 : 
	u_courant = u_courant * q
	annee_courante = anne_courante + 1

# On sort de la boucle - Objectif atteint
print("Annee ",annee_courante)

```

	-

- Déterminer le point d'intersection entre deux suites géométriques.
	- Analyse :
		- Caractériser les deux suites.
			- Option 1 : Dans un tableur faire trois colonnes :
				- Colonne 1 : Valeur de $n$ (1,2,3,....) ou les années
				- Colonne 2 : Valeurs de la première suites
				- Colonne 3 : Valeurs de la deuxièmes suites
			- Faire un graphique et repérer le point d'intersection

**Exemple** :  Travail p.8

**Attention :** On peut aussi vous demander de calculer un cumul. Dans ce cas il faut utiliser la formule :
$$ S_n = u_1 \times \frac{1-q^n}{1-q} $$Déterminer le montant des ventes la huitième année $\rightarrow u_8$ 
Déterminer le nombre de ventes au cours des huit premières années $\rightarrow S_8$ 












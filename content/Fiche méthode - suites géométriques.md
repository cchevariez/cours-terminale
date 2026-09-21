
**Définition** : Une suite est dite géométrique si pour passer d'un terme au terme suivant, on multiplie toujours par le même nombre.

**Terme général :**

$$ u_n = u_1 \times q^{n-1} $$ **Somme d'une suites géométrique**

$$ S_n = u_1 + u_2 + ... + u_n = u_1 \times \frac{1-q^n}{1-q}$$
**Questions types** 
- Déterminer quand une suite atteint une limite.
Exemple : On place 1500 € sur un livret à 2%, on souhaite déterminer en combien de temps on atteint un capital de 2000 €

Analyse : 
	- Caractériser la suite.
	- Sur un tableur, on fait deux colonnes. Une colonne année qui va de un en un. Une colonne capital dont la première valeur est 1500 et on multiplie la valeur précédente par 1,02
	- On repère en quelle année on atteint 2000 €

Variant : utilisation de Python

```python
annee = 2026
u1 = 1500
q = 1.02

u_courant = u1
annee_courante = annee

while u_courant < 2000 :
	u_courant = u_courant*q
	annee_courant = annee_courant + 1
	
print("Année ",annee_courant)
```


Point d'intersection entre deux suites géométriques

Exemple : On dispose de deux placements :
	- Placement A : Capital 2000€ intérêts 3%
	- Placement B : Capital 1200€ intérêts 5%
Problématique : Déterminer quand la valeur acquise du placement B dépasse celle du placement A.

Analyse : 
- Caractériser les suites
- Mise en place d'un tableur
### K neirest neighbord (K plus proche voisin)
KNN, ou k-Nearest Neighbors, est un algorithme d'apprentissage supervisé utilisé dans les domaines de la classification et de la régression. L'algorithme KNN est assez simple à comprendre et à mettre en œuvre, ce qui en fait l'un des premiers choix pour de nombreux problèmes d'apprentissage automatique. Contrairemant a d'autre algorithme, ce dernier ne nécissite pas de connaitre les paramatres du modèle  c'est basé une une logic intiuitive et simple á comprendre. 

##### Idée de l'algorithme
Supposons qu'il y a un ensemble de données déja étiquété(dont la cible est connus) $X \in \mathbb{R}^n \times \mathbb{R}^m$ et un nouvelle observation á prédire $x_i$.
L'idée de l'algorithme est basé sur la similiarité des données. Il suppose qu'il y a une similarité entre les points. Pour faire la prédiction il calcule la similarités entre $x_i$ (une observation) avec toutes les observations dans $X$, ensuite il renvoie les K(un nombre données)observations dans $X$ qui sont plus proche en terme de distance de $x_i$. En se basant sur leur étiquètte il renvoie l'étiquètte qui á le nombre d'occurrence le plus élevé. L'algorithm est utilisé á la fois pour un problème de classification et de regression

**Le retour pour chaque type**

1. **Classification :**
   - Dans le cas de la classification, l'algorithme KNN classe un nouvel exemple en fonction de la classe majoritaire parmi ses k plus proches voisins dans l'espace des caractéristiques.

2. **Régression :**
   - Pour la régression, l'algorithme KNN calcule la valeur moyenne (pour la régression simple) ou la valeur médiane (pour la régression pondérée) des k voisins les plus proches comme la prédiction de la valeur cible pour un nouvel exemple.

**Étapes de l'Algorithme :**

1. **Mesure de la Similarité :**
   - L'algorithme commence par mesurer la similarité entre l'exemple à classer et chaque exemple dans l'ensemble de données. Cette mesure de similarité est généralement calculée à l'aide d'une distance, comme la distance euclidienne ou la distance de Manhattan, entre les caractéristiques des exemples.

2. **Sélection des k Plus Proches Voisins :**
   - Les k exemples ayant la plus grande similarité avec l'exemple à classer sont sélectionnés comme les plus proches voisins.

3. **Classification ou Régression :**
   - Pour la classification, la classe majoritaire parmi les k voisins est attribuée à l'exemple à classer.
   - Pour la régression, la valeur moyenne ou médiane des valeurs cibles des k voisins est utilisée comme prédiction pour l'exemple à régresser.

**Paramètre k :**
   - Le choix de la valeur de k est crucial dans l'algorithme KNN. Une valeur trop petite de k peut rendre le modèle sensible au bruit, tandis qu'une valeur trop grande peut rendre le modèle moins sensible aux variations locales.

**Avantages de KNN :**
   - Facile à comprendre et à mettre en œuvre.
   - Ne nécessite pas d'hypothèses sur la distribution des données.
   - Peut être utilisé pour la classification et la régression.

**Inconvénients de KNN :**
   - Sensible à l'échelle des caractéristiques et à la dimensionnalité.
   - Peut être coûteux en termes de calcul pour de grands ensembles de données.
   - Nécessite de choisir judicieusement la valeur de k.

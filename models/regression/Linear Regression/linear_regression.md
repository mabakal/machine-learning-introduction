### Regression lineaire

La régression linéaire est une technique d'apprentissage supervisé utilisée pour modéliser la relation entre une variable dépendante continue $y$ et une ou plusieurs variables indépendantes $x$. L'objectif de la régression linéaire est de trouver la meilleure ligne droite (ou hyperplan dans le cas de régression linéaire multiple) qui représente au mieux la relation entre les variables.

##### Forme de la Régression Linéaire Simple
Prenons deux points $(x_i, y_i) \in \mathbb{R}^2$, on cherche á établir une relation entre ces deux points la régression linéaire est exprimée par l'équation d'une droite dont la formule est $h(x_i)=ax_i+b$ où 
$x$ est la variable dépendante qui est connue
$h(x_i)$ est la variable á prédire l'inconnue
$a$ le coefficient du model
$b$ l'intercepte du modèle
Cette équation produit une erreurs noté $\epsilon$ qui est $\epsilon = y_i - h(x_i)$ ou encore  $\epsilon = y_i - (ax_i+b)$. Pour rendre cette erreur positive, on va l'élever au carré ce qui va produire $\epsilon = (y_i - h(x_i))^2$. Ceci est l'erreur qui est produit par une seul observation, quelle est l'erreur produit par toutes les observations? Sur toutes les observations, $\epsilon =\sum_{i=1}^n (y_i - h(x_i))^2$ avec 
$X_i \in \mathbb{R}^{2n}$. On va chercher alors á minimiser cette erreure


##### Résolution analylitique

epsilon est une fonction du second dégrer on peux alors la dériver pour chercher les extremuim de la fonction.

$$\begin{cases}
    \frac{\partial \epsilon}{\partial a}= -2\sum{x_i*(y_i - (ax_i +b))} \\
    \frac{\partial \epsilon}{\partial b}= -2\sum{(y_i - (ax_i +b))}
\end{cases}$$
La résolution analytics va données:
$\text{b}=\hat{y} - a\hat{x}$
$\text{a}=\frac{\text{Cov}(X, Y)}{\text{Var}(X)}$


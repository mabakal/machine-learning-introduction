#### Les bases en machine learning

    Pour faire ces prémier pas en machine learning, il y a des bases que tu dois connaitre, une bonne maitrise de ces bases de permettras de comprendre l'apprentissage de tes futurs modèles, ou touché si ca ne fonctionne le modèle fonctionne mal. Je vais te les présenter d'une manière intuitive pour te facilité la compréhension. Je t'avais dit que machine learning est un ensemble de modèle, chaque modèle á des taches bien déterminer et que on peux classer ces modèles dans des catégories, superviser, non superviser ou réinforcement. 
    Supposons tu as un problème, tu veux construire un système intelligent en utilisant la machine learning, tu as á ta disposition un ensemble de données. Tu vas premier determiner á  quelle classe appartient ce problème. Est un problème de classification, regression etc? Il y a plusieurs classe d'algorithme, la selection de l'algorithme dépend de ton problème. Une fois la classe connue, tu sélectionne un algorithme, c'est le modèle. c'est quoi un modèle

##### La fonction d'hypothèse

    Il est très important de comprendre les données á disposition pour selectionner un bon modèle. Un modèle est une fonctionne mathématique **$H(x)$** dont les paramètres ne sont pas connue. Tu vas entrainer le modèle á determiner les paramètres du modèle. Tu as une données $(X,y) \in R^n$ où $X$ est la caractéristique et $y$ la valeur á prédir. Prenons un exemple simple
    Tu penses qu'il y a une relation linéaire entre tes données , mais tu ne connais pas les paramètres modèle. La fonction d'hypothèse dans ce cas est:
    $$ h(x) = a*X + b $$ oú $a$ et $b$ sont les paramètres du modèle qui appartiennent à $R^n$ et $X$ l'echantillons de données á ta disposition.

##### Fonction d'erreur
 
Tu as la fonction d'hypothèse $ h(x) = a*X + b $, cette fonction est utilisé pour faire la prédiction. En utilisant cette fonction hypothèse tu fait une prédiction sur une entré $x_i$ qui produit un $\hat{y}$. Ce dernier n'est pas la valeure réelle, mais plutot une prédiction, la valeur réelle est $y$. C'est une approximation, et qui parle d'approximation fait internvenir une erreurs. Dans notre cas on peux noté l'erreur comme $\epsilon = (y - \hat{y})$ (c'est pas toujours le cas, ça dépend du problème). C'est l'erreur d'une seule échantillons, c'est on parcours tous les échantillons on aura l'ensemble des erreurs qu'il va produire. 

##### La fonction de coût

C'est la fonction de toutes les erreurs, toutes les erreurs sont réunie dans cette fonction. Pour construire un bon modèle, il faut chercher á minimiser cette fonction. Si $\epsilon$ est une erreur, la fonction de cout sera par exemple $$ C = \sum_{i=1}^{n} \epsilon$$ 


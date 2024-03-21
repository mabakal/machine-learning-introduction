### Les bases en machine learning

Pour faire ces premiers pas en machine learning, il y a des bases que tu dois connaître. Une bonne maîtrise de ces bases te permettra de comprendre l'apprentissage de tes futurs modèles, ou de détecter si ton modèle fonctionne mal. Je vais te les présenter d'une manière intuitive pour te faciliter la compréhension.
Je t'avais dit que le machine learning est un ensemble de modèles, chaque modèle ayant des tâches bien déterminées, et qu'on peut classer ces modèles dans des catégories : supervisée, non supervisée ou par renforcement.
Supposons que tu as un problème : tu veux construire un système intelligent en utilisant un machine learning, et tu as à ta disposition un ensemble de données. Tu vas d'abord déterminer à quelle classe appartient ce problème. Est-ce un problème de classification, de régression, etc. ? Il existe plusieurs classes d'algorithmes, et la sélection de l'algorithme dépend de ton problème. Une fois la classe connue, tu sélectionnes un algorithme, qui est le modèle. Mais qu'est-ce qu'un modèle ? Ici je te présente ce que c'est qu'un modèle, comment il est construit. Si tu comprend ceci, tu pourras **comprendre les modèles existant et créer tes propre modèles**
#### La fonction d'hypothèse
Il est très important de comprendre les données à disposition pour sélectionner un bon modèle. Un modèle est une fonction mathématique $H(x)$ dont les paramètres ne sont pas connus. Tu vas entraîner le modèle à déterminer les paramètres du modèle. 
Tu dispose un echantillons de donnéEs $(X,y)$ où $X \in \mathbb{R}^n \times \mathbb{R}^n$ et $y \in \mathbb{R}^n$. Tu penses qu'il y a une relation linéaire entre tes données (__note bien, c'est ta fonction d'hypothèse__), mais tu ne connais pas les paramètres du modèle(__c'est ce que tu cherche à déterminer__). La fonction d'hypothèse dans ce cas est : $H(x_i) = ax_i +b$
Où $a$ et $b$ sont les paramètres du modèle qui appartiennent à $\mathbb{R}$ et $x_i \in \mathbb{R}^n$ est l'échantillon de données à ta disposition. $H(x) = aX +b$ est la fonction d'une relation linéaire.
#### Fonction d'erreur
Tu as la fonction d'hypothèse $h(x)=a*X + b$. Cette fonction est utilisée pour faire la prédiction. En utilisant cette fonction hypothèse, tu fais une prédiction sur une entrée $x_i$ qui produit un $\hat{y}$. Ce dernier n'est pas la valeur réelle, mais plutôt une prédiction ; la valeur réelle est $y_i$. C'est une approximation, et qui parle d'approximation, fait intervenir une erreur. Dans notre cas, on peut noter l'erreur comme $\epsilon=(y_i - \hat{y})^2$ (ce n'est pas toujours le cas, ça dépend du problème). C'est l'erreur d'un seul échantillon. Si on parcourt tous les échantillons, on aura l'ensemble des erreurs qu'il va produire.
#### La fonction de coût
C'est la fonction de toutes les erreurs elle est composé par les $\epsilon$. Pour construire un bon modèle, il faut chercher à minimiser cette fonction. Si $\epsilon$ est une erreur, la fonction de coût sera, par exemple : $\frac{1}{n}\sum_{i=1}^{n}{\epsilon_i}$, ce qui est encore equivalent á $\frac{1}{n}\sum_{i=1}^{n}{(y_i - \hat{y_i})^2}$, si on inclue les paramètres on trouveras $\frac{1}{n}\sum_{i=1}^{n}{(y_i - ax +b)^2}$. On peux encore faire mieux en transformant cette relation sous forme de produit matrixielle et la fonction de coût devient $C(\beta)=\frac{1}{n}(y - X*\beta)^2$ où $\beta \in \mathbb{R}^n$ et  $X \in \mathbb{R}^n \times \mathbb{R}^m$ et $y \in \mathbb{R}^n$. La question qui se pose maintenant est comment déterminer les paramètres de ton modèle? Dans notre exemple on peux déterminer ces paramètre en utilisant l'analyse mathématique. Généralement, les fonctions de coût sont un peux défiant. On utilise très souvent l'optimisation. Cette une branche de la mathématique á qui on confie les problèmes de maximixation ou de minimisation. Une methode de maximixation très utilisé en machine learning est la methode de gradiant descent. Je vous présent cette méthode et les variants [ici](gardient.md).
#### Fonction de mesure d'erreur
Tu as compris la methode du descent de gradient, c'est cette methode qui va te permettre de determiner les parametres  du modèle. En utilisant cette methode, tu vas trouver les paramètres qui correspond á tes données. Tu utilise ton modèle entrainer sur des nouvelles données, note que ton modèle ne sera pas parfait. Quelles sont les fonctions qui permettent de mésurer les erreurs de ton modèle? Dans notre cas tu essais de prédire une variable continue, tu peux donc évaluer les prédictions de ton modèle avec la fonction suivant, $\frac{1}{n}\sum_{i=1}^{n}{(y_i - \hat{y_i})^2}$ ca s'appelle d'ailleurs erreur quadratique moyenne ou Mean Square Error (MSE) en anglais. Il est utilisé pour mésurer les predictions continue. Plus cette fonction est proche de zéro, sur l'échelle de la valeur á pédire ton modèle est __bon__. Il y a plusieurs fonction de mésure d'erreur qui est utiliser, je te présente quelques uns [visite ici](measure_error_function.md).